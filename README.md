Shaun Jackman
=============

*PhD candidate in bioinformatics, programmer, engineer*

[GitHub](https://github.com/sjackman)
— [Twitter](http://twitter.com/sjackman)
— [Google Scholar](http://scholar.google.ca/citations?user=wFl3qXAAAAAJ)
— [Impactstory](https://impactstory.org/sjackman)
— [LinkedIn](http://www.linkedin.com/in/sjackman)
— [Resume](http://sjackman.ca/resume)
  [(PDF)](https://www.dropbox.com/s/d7mdj806squlmwz/Shaun%20Jackman.pdf)  
<sjackman@gmail.com>

I live in Vancouver, Canada, where I'm a PhD candidate studying bioinformatics at
the University of British Columbia with my supervisor, Inanc Birol. I work
with the genome sequencing data of a variety of species, including human and
the white spruce tree. I develop software that takes fragmented genome
sequencing data and attempts to reassemble the original genome from which the
short fragments were derived. My undergraduate degree is in computer
engineering. I'm a programmer, an avid traveller, a singer, and an experimental
amateur chef.

Projects
========

UniqTag
-------

[UniqTag][] is used to abbreviate gene sequences to unique and stable
identifiers. It selects a representative *k*-mer from the sequence of each gene
to be used as a systematic identifier for that gene. Unlike serial numbers,
these identifiers are stable between different assemblies and annotations of
the same data without requiring that previous annotations be lifted over by
sequence alignment.

[Shaun D. Jackman, Joerg Bohlmann, İnanç Birol (2015)][uniqtag-paper]
UniqTag: Content-derived unique and stable identifiers for gene annotation.
*PLOS ONE*, [doi:10.1371/journal.pone.0128026](http://dx.doi.org/10.1371/journal.pone.0128026).

[UniqTag]: https://github.com/sjackman/uniqtag
[uniqtag-paper]: https://github.com/sjackman/uniqtag-paper

ABySS
-----

![ABySS](abyss.png)

[ABySS][] is a genome sequence assembler that distributes the computation of
large genome sequence assembly over a cluster of computers using MPI.

[ABySS]: https://github.com/bcgsc/abyss

White spruce genome sequence assembly
-------------------------------------

![SMarTForests](smartforests.png)

The [SMarTForests][] project used [ABySS][] to assemble the genome of the white
spruce tree, which is twenty gigabases&mdash;seven times larger than the human
genome. I'm currently working on assembling and annotating the organellar
genomes of white spruce, the mitochondrion and chloroplast.

[SMarTForests]: http://www.smartforests.ca/

Presentations
================================================================================

[Automating Data-analysis Pipelines using R and Make](http://stat545-ubc.github.io/automation01_slides/)
and a [hands-on activity](http://stat545-ubc.github.io/automation04_make-activity.html)

[Open, reproducible science using Make, RMarkdown and Pandoc](http://sjackman.github.io/open-science/)

More slides on [Speaker Deck][] and [SlideShare][]

[SlideShare]: http://www.slideshare.net/shaunjackman
[Speaker Deck]: https://speakerdeck.com/sjackman
