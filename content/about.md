---
title: "About"
date: 2018-01-23T18:42:58+13:00
---

# Law as Code

As part of the [Better Rules Hackathon](https://legalhackers.nz/betterruleshack/), we wanted to help make legislation easier to use, track, and improve.

## The Goal

We wanted to build a proof-of-concept, to show that it is both **feasible** and **beneficial** to make legislation easier to work with.

## The Approach

We wanted to use simple, familiar tools, to make the most of our limited time over the weekend. We chose to push our output to GitHub, a popular platform for sharing and working with code, to avoid any need to manage our own web hosting.

We chose to turn the XML law into AsciiDoc text files. AsciiDoc is a format that works well for both people and computers.

{{< youtube VhprEZVXreg >}}

## The Source

We started with raw XML files from the official legislation website.

![Legislation.govt.nz offers enactments in XML format](/img/legislation-web.png "The official website for NZ legislation offers law as XML files")

# The Outcome

We created automated tools to:

1. Read legislation from the official XML source
2. Transform the XML into readable .adoc files
3. Upload the .adoc files to GitHub for sharing and re-use

## What can our tools do?

Our proof-of-concept worked with legislation from 1993, but is already capable of working on **all** legislation provided through the official XML source. That includes law going all the way back to the Statute of Marlborough from 1267.

![](img/statute-of-marlborough.png)

## Proof-of-Concept: The Privacy Act 1993

We demonstrated our tools working with the Privacy Act 1993. This is a topical bit of law, with a Privacy Bill to update it before Parliament. Below you can see how the automated comparison in GitHub helps to see the specifics of a law change.

GitHub also makes it easy to [link to a specific change](https://github.com/jamestingedwards/legis-hack/commit/c34b6fc40521174591afca9fd7ffdbf1d4a5e6df?diff=split) - try it out!

![](img/priv-act-diff.png "The automatic comparison makes it clear what has changed with this amendment")

## Progress on process

As we honed our tools, the process got substantially faster. It took us:

- Just under 30 hours to process our first enactment
- 15 minutes to do the second (and solve a bug)
- 15 minutes to do the remaining 47 Acts from 1993

The remaining bottleneck is download speed. With all the enactments on one machine, we could do this much quicker from here.
