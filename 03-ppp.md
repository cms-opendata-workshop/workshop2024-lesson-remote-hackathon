---
title: "Introduction"
teaching: 5
exercises: 0
---

:::::::::::::::::::::::::::::::::::::: questions 

- What is C++?
- What is ROOT?
- What is the point of these exercises?

::::::::::::::::::::::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: objectives

- Learn a bit about C++ and how to compile C++ code.
- Learn how to use ROOT to write and read from files, using the C++ libraries.
- Learn how to use ROOT to investigate data and create simple histograms.
- Explore the ROOT python libraries.

::::::::::::::::::::::::::::::::::::::::::::::::

## Let's talk about ROOT!

From the [ROOT website](https://root.cern/):

::::::::::::::::::::::: testimonial
*ROOT is a framework for data processing, born at CERN, at the heart of the research on high-energy physics. Every day, thousands of physicists use ROOT applications to analyze their data or to perform simulations.*

In short, ROOT is an overarching toolkit that defines a file structure, methods to analyze particle physics
data, visualization tools, and is the backbone of many widely used statistical analysis tool kits,
such as RooFit and RooStats. You don't *need* to use ROOT for your own analysis, but you will have to have
some familiarity with it when you are first accessing the open data.
:::::::::::::::::::::::

OK, that sounds cool. So what's the deal with C++?

## ROOT and C++

In the mid-80's, [C++](https://en.wikipedia.org/wiki/C%2B%2B) extended the very popular [C programming language](https://en.wikipedia.org/wiki/C_(programming_language)),
primarily with the introduction of [object-oriented programming](https://en.wikipedia.org/wiki/Object-oriented_programming) (OOP).
This programming paradigm was adopted by many particle physics experiments in the 1990's and when ROOT was written,
it was written in C++. While there are now python hooks to call the ROOT functions, the underlying code is all in C++.

Because C++ is a compiled code, it is usually much faster than a scripted language like python, though that is
changing with modern python tools. Still, since much of the original analysis and access code was written in C++
and calling the C++ ROOT libraries, it's good to know some of the basics of ROOT, in a C++ context.

Most CMS analysts interface with ROOT using python scripts and you may find yourself using a similar workflow.
Later on in this lesson, we'll walk you through some very basic python scripts and point you toward more in-depth
tutorials, for those who want to go further.

::::::::::::::::::::::::::::: callout
## You still have choices!

Just to emphasize, you really only *need* to use ROOT and C++ at the early stages of analyzing CMS Open Data in the AOD (Run 1) or MiniAOD (Run 2) formats. These datasets require using CMS-provided tools that perform much better in C++ than python. However, downstream in your analysis or to analyze Run 2 NanoAOD files, you are welcome to use whatever tools and file formats you choose.
:::::::::::::::::::::::::::::

::::::::::::::::::::::::::::::::::::: keypoints 

- C++ has a reputation for being intimidating, but there are only a few things you need to learn to edit the open data code for your own uses.
- You can use the ROOT toolkit using both C++ and python.
- Some ROOT code is written in C++ to access the datafiles.
- People will often use simpler C++ scripts or python scripts to analyze reduced datasets.

::::::::::::::::::::::::::::::::::::::::::::::::
