# CoMSES Net Science Gateway CSSI 2023 PI meeting, Houston TX
Supporting materials and Jupyter notebooks for the 2023 NSF CSSI PI meeting

## From Metrics to Machine Learning

Like many other groups in academia, research software engineering (and industry), CoMSES.Net has struggled to [find full-time research software engineers](https://doi.org/10.5281/zenodo.8329337) to help us develop supporting cyberinfrastructure for our research community that studies the complex dynamics of social and ecological systems through computational models and simulation.

In early 2023 after another failed full-time RSE search we decided to invest in building a student developer pipeline, partially inspired by programs like the University of Utah's [Student University Development Opportunity program (sudo.utah.edu)](https://sudo.utah.edu). Overall this has been an excellent and positive experience for our student developers and our research group. Hiring and training undergraduate students advances our University's mission of experiential learning and discovery for our student developers and improves the reach of our social and professional networks. It also helps our project stay honest by exercising core software project components including documentation, tests, build engineering, and more broadly how amenable our project is to a new developers' contributions and our software stack’s agility and capacity for evolution and change in response to emerging community needs.

1. Developer onboarding documentation - how easy is it for our students to download, install and create a development environment for our science gateway with an edit-build-test cycle that actively supports experimentation and rapid prototyping?
2. Mentorship and training - how do we help our students learn how to contribute to a real-world project with practical concerns of security, usability, maintainability, codebase consistency and style, etc., while maintaining clean code contribution workflows on Git and GitHub? How do we help them establish baseline competencies in the technologies, languages, and software frameworks we use?

Four undergraduate students joined us in January 2023 and helped us develop a [metrics page](https://comses.net/about/metrics). Along the way we revisited issues of data quality that all Science Gateways face, as developing useful usage metrics depends on _clean data_. Every public science gateway that supports user entered metadata will have metadata curation issues which can benefit from data science and machine learning support. In our case, this means record linkage and deduplication of user-entered metadata (e.g., tags and their [resultant folksonomies](https://www.sciencedirect.com/topics/computer-science/folksonomies)), as well as detection and warning systems for spam content and malicious actors.

## cookiecutter Open Science Grid NetLogo template

https://github.com/comses-education/cookiecutter-netlogo-osg
