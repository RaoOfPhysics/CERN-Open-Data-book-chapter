# Motivation

- Word count: **1,000**

CERN, the European Laboratory for Particle Physics, is the world's premier research facility for accelerator-based high-energy physics, located outside of Geneva on both sides of the Franco-Swiss border. The laboratory's flagship accelerator is the Large Hadron Collider (LHC), which, at 27 km in circumference, is the biggest and most powerful particle accelerator ever built. It accelerates protons in clockwise and anti-clockwise directions to nearly the speed of light before colliding them at four points around its ring. Four giant detectors, operated by international collaborations of scientists and engineers, record information from these collisions, generating an enormous volume of data for analysis: each collision event produces data of the order of megabytes (MB), and, with the LHC delivering millions of collision events each second, the CERN Data Centre has collected tens of petabytes since the accelerator began operations in 2010.

Not only are these datasets interesting for students and data scientists, they also form a significant part of the scientific legacy of the LHC.

In order to ensure that these data continue to remain available to researchers in the future, the four LHC collaborations have put in place [policies for data preservation and access](http://opendata.cern.ch/collection/Data-Policies). These lay out basic statements on preservation and data publishing, regarding matters such as embargo periods, openness, licensing and reuse. The specifications distinguish four different data levels (see [DPHEP, 2009](https://arxiv.org/abs/0912.0255)) that define the resulting recommendations:

> 1. Level 1 data comprises data that is directly related to publications which provide documentation for the published results
> 2. Level 2 data includes simplified data formats for analysis in outreach and training exercises
> 3. Level 3 data comprises reconstructed data and simulations as well as the analysis level software to allow a full scientific analysis
> 4. Level 4 covers basic raw level data (if not yet covered as level 3 data) and their associated software and allows access to the full potential of the experimental data

The Open Data being discussed here refer to Levels 2 and 3.

CERN is itself a strong proponent of openness in research, having worked with publishers and other laboratories to ensure that all particle-physics results from the LHC collaborations are published as open-access papers (see [SCOAP3](https://scoap3.org/) and the [Open Access Policy for CERN Physics Publications](https://cds.cern.ch/record/1955574)). More recently this paradigm has been [expanded to cover Open Science more comprehensively](http://home.cern/cern-people/opinion/2014/11/road-open-science). CERN has helped build tools and digital libraries to foster Open Science practices beyond the particle-physics community, with the widely used Invenio digital library software forming the basis for projects such as ZENODO, has helped thousands of scientists archive their work on CERN's servers with persistent identifiers. In order to facilitate storage for and access to open data from the LHC collaborations, the laboratory launched the CERN Open Data Portal in November 2014.

All four LHC experiments provide data in a format suitable for a classroom environment. In additional to these "educational" datasets, the CMS Collaboration, in accordance with its data preservation and access policies, has also released large volumes of high-quality data for research purposes along with the tools necessary for accessing and analysing them. This chapter describes the motivation behind the launch of the CERN Open Data Portal as well as the background to and experience with the release of the open data from the LHC. In the spirit of openness, development work for the portal is conducted publicly on the code-sharing platform, [GitHub](https://github.com/cernopendata/opendata.cern.ch).

Please note that while CMS released a second batch of data in April 2016 [LINK], this chapter focuses on the first release from November 2014.
