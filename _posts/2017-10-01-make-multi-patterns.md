---
title: Multiple pattern rules using GNU Make
subtitle: How to emulate multiple wild cards in a pattern rule.
layout: post
---

Pattern rules in a Makefile can match a wild card. For example, the following rule removes consecutive duplicate entries from a text file with the extension `.txt` and creates a new file with the extension `.uniq.txt`.

```Makefile
%.uniq.txt: %.txt
	uniq $< >$@
```

```sh
yes hello | head > hello.txt
make hello.uniq.txt
wc -l hello.txt hello.uniq.txt
```

```
10 hello.txt
 1 hello.uniq.txt
11 total
```

Some useful commands take more than one input file, for example `comm` finds the lines that two sorted files have in common.

```Makefile
$a.$b.comm.txt: $a.txt $b.txt
	comm -12 $^ >$@
```

This rule is an explicit rule rather than a pattern rule. To use it, you have to specify the values of both `a` and `b`.

```sh
seq 10 29 >x.txt
seq 20 39 >y.txt
make a=x b=y x.y.comm.txt
wc -l x.txt y.txt x.y.comm.txt
```

```
20 x.txt
20 y.txt
10 x.y.comm.txt
50 total
```

I'll explain a few options to work around this deficiency and emulate pattern rules using GNU Make.

# 1. Use Biomake rather than GNU Make

Biomake

# 2. Parameterize one of the two wildcards

# 3. Expand one of the two wildcards

# 4. Use recursion
