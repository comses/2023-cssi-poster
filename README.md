# CoMSES Net CSSI 2023 PI meeting, Houston TX
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/comses/2023-cssi-poster/HEAD)

Supporting materials and Jupyter notebooks for the 2023 NSF CSSI PI meeting

## From Metrics to Machine Learning

Like many other groups in academia, research software engineering (and industry), CoMSES.Net has struggled to [find full-time research software engineers](https://doi.org/10.5281/zenodo.8329337) to help us develop supporting cyberinfrastructure for our research community that studies the complex dynamics of social and ecological systems through computational models and simulation.

<details>
<summary>More info</summary>


In late 2022 after another failed full-time RSE search we decided to invest in building a student developer pipeline, partially inspired by programs like the University of Utah's [Student University Development Opportunity program (sudo.utah.edu)](https://sudo.utah.edu). Overall this has been an excellent and positive experience for our student developers and our research group. Hiring and training undergraduate students advances our University's mission of experiential learning and discovery for our student developers and improves the reach of our social and professional networks. It also helps our project stay honest by exercising core software project components including documentation, tests, build engineering, and more broadly how amenable our project is to new developers' contributions and our software stack’s capacity for evolution and change in response to emerging community needs.

### Developer onboarding documentation 

How easy is it for our students to download, install and create a development environment for our science gateway with an edit-build-test cycle that actively supports experimentation and rapid prototyping?

### Mentorship and training 

How do we help our students learn how to contribute to a real-world project with practical concerns of security, usability, maintainability, codebase consistency and style, etc., while maintaining clean code contribution workflows on Git and GitHub? How do we help them establish baseline competencies in the technologies, languages, and software frameworks we use?
</details>

Four undergraduate students joined us in January 2023 and helped us develop a [metrics page](https://comses.net/about/metrics). Along the way we revisited issues of data quality that all Science Gateways face, as developing useful usage metrics depends on _clean data_. Every public science gateway that supports user entered metadata will have metadata curation issues which can benefit from data science and machine learning support. In our case, this means implementing data curation workflows that help human curators perform [entity resolution](https://doi.org/10.1145/2487575.2506179), record linkage and deduplication of user-entered metadata (e.g., tags and their [resultant folksonomies](https://www.sciencedirect.com/topics/computer-science/folksonomies)), and detection and early warning systems to identify spam content and malicious actors.

Our intrepid students 🥳 have put together interactive Jupyter notebooks that describe the technologies and processes we used to build these ML-assisted data curation workflows:

- [Tag Deduplication](dedupe.ipynb) by [Noel Ngu](https://github.com/hwelsters)
- [Spam Detection](spam_detection.ipynb) by [Aiko Muraishi](https://github.com/BlllueSea) and [Charles Sheelam](https://github.com/CharlesSheelam)

## High Throughput Computing and the Open Science Grid


> The [Open Science Grid (OSG)](https://osg-htc.org/about/introduction/) is a consortium dedicated to the advancement of open science via the practice of distributed High Throughput Computing, and the advancement of its state of the art.

In general terms, the OSG provides access to a distributed set of compute resources for researchers to run "embarrassingly parallel" computational workloads. For the [CoMSES.Net](https://comses.net) community this is an ideal fit for the kinds of [model analysis](https://www.jasss.org/18/4/4.html) that need to be run on simulation models which often include detailed sensitivity analysis and uncertainty quantification.

<details>
  <summary>More info on the OSG</summary>

  
  > The OSG Consortium builds and operates a set of pools of shared computing and data capacity for distributed high-throughput computing (dHTC). Each pool is organized and operated to serve a particular research community (e.g. a campus, multi-institutional collaboration, etc.), using technologies and services provided by the core OSG Team. One of these pools, known as the Open Science Pool is operated for all of US-associated open science. The Consortium, thus, represents the totality of all researchers, resources, individuals and institutions that benefit from or contribute to any of the OSG Fabric of Services.
> 
> The OSG Council governs the consortium ensuring that the OSG benefits the scientific mission of its stakeholders: the research communities, organizations that provide resources and services for them, including funding resources.

> The Executive Team manages the core OSG Team, with team members from various institutions organized into Areas that provide core OSG technologies and services required to operate pools in support of research communities. As of January 2022, the OSG Team is funded primarily via the PATh (NSF #2030508), IRIS-HEP (NSF #1836650) projects, and in kind contributions from multiple entities, including DOE national laboratories.

</details>

## Cookiecutter templates, educational materials, and scaffolding for FAIR+OSG computational models

Co-PIs Sean Bergin and Allen Lee attended the recent [OSG User School 2023](https://osg-htc.org/user-school-2023/) and are developing educational materials tailored to our research community as well as computational and build scaffolding to help researchers adopt FAIR practices for research software as well as tools like the OSG. This includes [cookiecutter](https://github.com/topics/cookiecutter-template) templates to help spin up new projects or update existing project's boilerplate with [cruft](https://cruft.github.io/cruft/), and the development of GitHub apps and actions that can suggest codebase augmentations for FAIR compliance, containerization, OSG integration, etc. via GitHub pull requests.

A cookiecutter template for the [NetLogo simulation modeling platform](https://ccl.northwestern.edu/netlogo/) is currently being piloted at https://github.com/comses-education/cookiecutter-netlogo-osg to make running NetLogo headless BehaviorSpace sensitivity analyses easier on the OSG. Future cookiecutter templates are planned for other popular modeling platforms and languages like [Julia](https://juliadynamics.github.io/Agents.jl/stable/) and [Python](https://github.com/projectmesa/mesa).
