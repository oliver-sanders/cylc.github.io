---
layout: frontpage
title: a workflow engine
---

**Cylc (*"silk"*) is a workflow engine for cycling systems** - it orchestrates
distributed **suites** of interdependent **cycling tasks** that may continue to
run indefinitely.

There are several reasons why tasks might need to be cycled:

 * To run successive cycles of an environmental forecasting system (where in
   real time operation new forecasts are initiated at regular intervals; but in
   catch-up or historical mode dependencies may allow concurrent cycles).

 * To split long model runs into a sequence of smaller runs, with associated
   processing tasks for each chunk.

 * To run successive steps in some multi-task iterative process, such as for
   optimizing model parameters.

 * To process a series of datasets (potentially concurrently, to the extent
   possible) as they are generated or received.

Cylc was originally developed for operational environmental forecasting at
[NIWA](http://www.niwa.co.nz) by [Dr Hilary
Oliver](mailto:hilary.oliver@niwa.co.nz). It is now an Open
Source collaboration involving NIWA, [Met Office](http://www.metoffice.gov.uk),
and
[others](https://github.com/cylc/cylc/blob/master/CONTRIBUTING.md#code-contributors).
It is [available under the GPL v3 license](./license.html).

{% include feature.html content="Suites are defined in a human-readable config
file format - so you can use software development power tools for suite
development." %}

{% include feature.html content="Configure scheduling with an efficient graph
description notation, and task runtime properties in an efficient inheritance
hierarchy (to factor out all commonality)." %}

{% include feature.html content="Cylc dynamically generates new workflow
without being constrained by a global cycle loop. Cycles interleave
naturally, suites flow around failed or delayed tasks, and they adapt to
insertion and removal of tasks." %}

{% include feature.html content="Cylc has low admin overhead and a small
security footprint, because - as a distributed system - there is no central
server process to manage workflows for all users." %}

{% include feature.html content="Plus <a href='features.html'>many other
features</a> to support both clock-triggered real time and free-flow
metascheduling in research and operational environments." %}

Please [let us know](mailto:hilary.oliver@niwa.co.nz) if your organization
should be included in the **[list of Cylc users](./users.html)**.


### Presentations

Format HTML5 with embedded .webm videos (plays natively in Firefox or Chrome).
Hit the "Home" and "End" keys to skip to the beginning and end of the
presentation, and the 'o' key for a multi-slide summary. This is the
[dzslides](https://github.com/paulrouget/dzslides) framework by Paul Roget.

* [Cylc Keynote](cylc-keynote-lisbon-Sept2016/index.html) - from
  the IS-ENES2 Workshop on Workflow in Earth Systems Modeling, Lisbon,
  September 2016

* [Cylc High Level Introduction](BoM-Feb-2017/index.html) - Bureau of
  Meteorology, Melbourne, February 2017


### Publications, Citations, and References

Please cite Cylc in your publications if you used it to automate your
workflows.

* [![DOI](https://zenodo.org/badge/1836229.svg)](https://zenodo.org/badge/latestdoi/1836229) - Citable DOI for Cylc source code

* [![DOI](http://joss.theoj.org/papers/10.21105/joss.00737/status.svg)](https://doi.org/10.21105/joss.00737) - A short paper in the Journal of Open Source Software.
Cite as:
> _Oliver et al., (2018). Cylc: A Workflow Engine for Cycling Systems. Journal of
Open Source Software, 3(27), 737, [https://doi.org/10.21105/joss.00737](https://doi.org/10.21105/joss.00737)_
