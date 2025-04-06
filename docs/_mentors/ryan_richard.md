---
title: "Ryan M. Richard"
layout: page
image:
  path: /mentors/images/fragment_based_methods.png
  thumbnail: /images/mentors/ryan_richard.png
  caption: "Fragment Based Method Research"
author: Ryan Richard
---

# About Me

Dr. Ryan Richard is a scientist at Ames National Laboratory and an adjunct
assistant professor of chemistry at Iowa State University. Ryan is the chief
architect and lead developer of
[NWChemEx](https://github.com/NWChemEx/NWChemEx). He is also the PI of several
other software packages including
[GhostFragment](https://github.com/rmrresearch/GhostFragment) and
[CMinx](https://github.com/CMakePP/CMinx). Ryan's research interests include
research software engineering, high-performance quantum chemistry, and method
development. He also dabbles in DevOps.

# Why I Like My Research

I first encountered ab initio chemistry after taking undergraduate organic
chemistry. Having just finished memorizing 100+ reactions, I learned that there
exists physics equations that could have "solved the reactions for me", i.e.,
I "just" had to plug the molecules in and solve the equations. Moreover, there
already existed software package which could solve the equations, so it was
even easier! As I know now, while this sentiment isn't conceptually wrong, it
does gloss over the fact that modern computational chemistry software is not yet
at this point where this approach works for arbitrary chemical reactions.

While computational chemistry isn't the "silver bullet" I thought it would be, I
still favor the use of software over memorizing reactions and now strive to
make existing software even more applicable. It turns out this is a very
challenging problem that keeps me thoroughly engrossed. Given the multi-
disciplinary nature, I learn new things every day. Slowly but surely I am
watching the applicability of ab initio chemistry increase and truly believe
that some day it will be routinely applicable to most of chemistry. In the
meantime, computational chemistry offers one of the more straightforward means
of gaining mechanistic insight into chemical reactions and programs like
NWChemEx are widely used for this purpose.

# Success in My Group

My research is highly inter-disciplinary and involves contributions from
chemistry, physics, mathematics, computer science, and software engineering.
These topics are unavoidable. Students do not need to be experts in these
topics, but they will need to learn some aspects as they are encountered. At the
same time, given the complexity of the equations, the only feasible manner of
obtaining solutions is by using software specifically written to solve these
equations. Thus software development is also unavoidable. While you do not need
to be a Google-level programmer, you must be willing to learn some programming
skills as well as the accompanying best practices.

Ideal skills:

- A strong math background including pre-calculus, if not calculus.
- Well organized (we deal with a lot of data and it is essential to keep it
  all straight).
- Ability to think critically about problems (debugging software is an
  exercise in logic).
- Basic computer skills. 95% of software engineering is knowing how to search
  Stack Overflow.

Wiling to learn (if you don't know them already):

- Linear algebra concepts. Linear algebra is the math of quantum chemistry and
  computer science. Terms will creep in.
- GitHub, Slack, VSCode, and Jupyter. These are among the most popular
  technologies of modern software development and data science. They will make
  your life much easier...
- Some C++. While users interact with NWChemEx through Python, the reality is
  the Python calls C++ libraries to do the heavy lifting. Inevitably, some of
  C++'s idiosyncrasies will slip through...
- Software engineering. Writing code that gets the right answer is only half
  the battle. The other half is ensuring that code is reasonably robust, user-
  friendly (including by other software), and well documented. Good code is not
  an accident, it is designed.

# Example Research Projects

Some of the research projects REU students can work on with me include:

## Fragment-Based Methods

Electronic structure calculations are computationally expensive. One way to
reduce the cost, and make the computations more suitable for supercomputing, is
to break large systems into many smaller systems called "fragments." Fragment-
based methods are variations on traditional electronic structure methods that
rely on fragmenting the target system. Potential research avenues include:

- Coding up new fragment-based methods. There's an obscenely large number of
  ways to fragment your average chemical system. Maybe we can come up with a
  better one?
- Benchmarking. Having fragment-based methods available isn't enough. We need to
  know when they work and when they fail. While analysis of the equations and
  algorithms offers some insight, brute-force running the method on many systems
  helps catch edge cases we may have missed.

These research projects are joint research efforts with (TODO: list other REU
mentors here).

## High-Throughput Electronic Structure

Training AI/ML models require a lot of data. Electronic structure theory is an
ideal candidate for generating this data because it solves the actual underlying
physics equations and can be run on many chemical systems without the need for
costly experiments. Roughly speaking most AI/ML models need at least a thousand
data points. This is more data than you want to manipulate by hand we must
develop automated solutions.

- Design and development of workflows and associated tools. While tools for
  executing workflows exist, they are generic and additional scripts are
  necessary to use them.
- Campaigns. With access to high-throughput electronic structure theory we need
  to assemble databases of results. It is also important that we characterize
  this data to make sure it is representative of the problem space.

These research projects are joint research efforts with (TODO: list other REU
mentors here).

## Software Development

Computational chemistry is a complicated endeavor. Computational chemistry
software must manage this complexity. NWChemEx is fairly unique among
computational chemistry software in that it was designed from the ground up to
be high-performance, flexible, modular, and highly-customizable. This leads to
a number of unique opportunities:

- Automated tooling. NWChemEx modules have some level of reflection (the
  ability for a software component to inspect itself at runtime). This in turn
  allows for the creation of tools for automated tasks which must be manually
  written in other software. Examples include documentation, testing, and
  saving/loading state.
- DevOps. Software maintenance is an ongoing battle. While modular software is
  a boon for the community, it can be a maintenance headache for the maintainer
  on account of needing to manage not just one monolithic package, but many
  separate components. Research in this area focuses on automating DevOps
  across the many components.

These research projects are joint research efforts with (TODO: list other REU
mentors here).
