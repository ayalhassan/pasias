Problems and Solutions in Applied Statistics
================
Ken Butler
2019-10-11

## Introduction

[This book](http://ritsokiguess.site/pasias/) will hold a collection of
problems, and my solutions to them, in applied statistics with R. These
come from my courses STAC32, STAC33 and STAD29 at the University of
Toronto Scarborough.

The problems were originally written in Sweave (that is, LaTeX with R
code chunks), using the `exam` document class, using data sets stolen
from numerous places (textbooks, websites etc). I wrote [a Perl
program](https://raw.githubusercontent.com/nxskok/pasias/master/convert.pl)
to strip out the LaTeX and turn each problem into R Markdown for this
book. You will undoubtedly see bits of LaTeX still embedded in the text.
I am trying to update my program to catch them, but I am sure to miss
some.

I just figured out that you can convert LaTeX “label” and “ref” pairs
into HTML “a name” and “a href=‘\#’”, which R Markdown can handle. I am
ludicrously pleased with myself. To that effect, you will occasionally
see question parts beginning with a \*; this means that other question
parts refer back to this one. (One of my favourite question strategies
is to ask how two different approaches lead to the same answer, or more
generally to demonstrate that there are different ways to see the same
thing.)

## How you can help

If you see anything, [file an
issue](https://github.com/nxskok/pasias/issues) on the Github page. I
will take pull requests and will acknowledge all the people who catch
things. Likely problems include:

  - some LaTeX construction that I didn’t catch (eg. block quotes)
  - disappeared footnotes (that will show up as an apparently missing
    sentence in the text)
  - references to “in class” or a lecture or a course by course number,
    which need to be eliminated (in favour of wording like “a previous
    course”)
  - references to other questions or question parts that are *wrong*
    (likely caused by *not* being “labels” or “refs” in the original
    LaTeX)
  - my contorted English that is difficult to understand.

## Background for these problems

As I read through looking for problems like these, I realize that there
ought to be a textbook that reflects my way of doing things. There isn’t
one (yet), though there are lecture notes. Reasonably recent versions of
these are at:

  - [the STAC32 website](http://ritsokiguess.site/STAC32/)
  - [the STAC33 website](http://ritsokiguess.site/STAC33/)
  - [the STAD29 website](http://ritsokiguess.site/STAD29/)

A little background:

STAC32 is an introduction to R (and also SAS) as applied to statistical
methods that have (mostly) been learned in previous courses, for example
a non-mathematical applied course like
[this](https://utsc.calendar.utoronto.ca/course/stab27h3). The idea is
that students have already seen a little of regression and analysis of
variance (and the things that precede them), and need only an
introduction of how to run them in R.

STAC33 covers similar ground to STAC32. It is intended for students with
a more mathematical background, and will include some extra material
beyond what is in STAC32 (eg., bootstrapping, Bayesian statistics with
Stan).

STAD29 is an overview of a number of advanced statistical methods. I
start from regression and proceed to some regression-like methods
(logistic regression, survival analysis, log-linear frequency table
analysis), then I go a little further with analysis of variance and
proceed with MANOVA and repeated measures. I finish with a look at
classical multivariate methods such as discriminant analysis, cluster
analysis, principal components and factor analysis. I cover a number of
methods in no great depth; my aim is to convey an understanding of what
these methods are for, how to run them and how to interpret the results.
Statistics majors and specialists cannot take this course for credit
(they have separate courses covering this material with the proper
mathematical background). D29 is intended for students in other
disciplines who find themselves wanting to learn more statistics; we
have an [Applied Statistics Minor
program](https://utsc.calendar.utoronto.ca/minor-program-applied-statistics-science)
for which C32 and D29 are two of the last courses.

## My checklist

  - bring in the D29 questions
  - working on A4 D29
  - look for multiple regression Qs in A6 or wherever
