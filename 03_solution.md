# Solution

A collaborative approach was taken to deliver both the CERN Open Data Portal and the first big open-data release -- from CMS -- at the same time. Members of CERN IT, CERN Scientific Information Service and the CMS Collaboration developed the platform, catalogued the data and analysis tools for the release, and prepared the appropriate user guidance and documentation. From the very beginning, it proved to be important to have subject specialists, information specialists and IT experts on board together to tackle the delivery of the big, complex datasets. Regular working meetings, sprints and feedback cycles ensured that the work on the portal and its content was on track and meeting the requirements of the potential users and use cases.

## Developing the platform

The CERN Open Data platform is based on the [Invenio digital library framework](http://inveniosoftware.org/), which was originally developed at CERN and is now co-developed by an international collaboration.

Invenio provides an ecosystem of standalone independent packages that can be used to build custom digital repositories. Use cases for Invenio include integrated library systems, digital document repositories, multimedia archives and data repositories. The software framework has been used for numerous such instances in the world and is particularly known for its scalability for large libraries, such as [CERN Document Server](http://cds.cern.ch/) or [INSPIRE](http://inspirehep.net/).

Invenio is mainly used in academic environments. In order to make the CERN Open Data Portal attractive to the general public, including high-school students and other targeted audiences, the framework has been extended with several features such as documentation pages and glossaries. Image XXX shows the home page of the CERN Open Data Portal.

A crucial aspect of providing open data is to ensure the long-term preservation of the datasets, as well as the accompanying software tools, so that they can be referenced and cited by means of persistent identifiers. This is also managed by Invenio, drawing inspiration from recommended practices of the Open Archival Information System (OAIS).

The datasets available on the CERN Open Data Portal are themselves stored in CERN's [EOS disk storage system](https://eos.web.cern.ch/). EOS is a disk-based service that provides low-latency storage infrastructure for physics use cases. EOS manages over 120 petabytes (PB) of disk storage at the time of writing this chapter. Access to the open data is provided by the [XRootD protocol](http://xrootd.org/) and is well suited to situations with many concurrent users, a significant fraction of random data access, and a large rate of file opening. The XRootD protocol allows ad-hoc streaming of necessary portions of data during an analysis, saving potential users of the large datasets from having to preemptively download the complete datasets before starting an analysis.

## Cataloging data and analysis tools

The CERN Open Data Portal has been developed to serve two main use cases: education and research (see more under Section 4). This is reflected in the information architecture of the Portal itself. It should be noted that special emphasis has been given to providing contextual information that is needed to understand and reuse data and accompanying software.

On the Portal each dataset has its own record. Related records are aggregated in dedicated collections, such as those for "Primary datasets" or "Derived datasets". This aggregation, considered as standard practice in digital libraries, has been adopted to research data. Further, metadata -- standardised according to [MARC](https://en.wikipedia.org/wiki/MARC_standards) -- are provided within each record. Adopting the practices developed by partner information platforms in high-energy physics (e.g. INSPIRE and CDS), standard metadata fields were populated. However, various additional metadata fields needed to be created to make sure information about data are standardised and comprehensive across all the datasets available via the Portal (see Table XXX).

The information provided was vetted to be comprehensive enough for future reuse of the data. Certain fields, such as the names of the authors, the publication year, title of the dataset, name of the publisher, were made mandatory for the sake of minting Digital Object Identifiers (DOIs).

The metadata are currently stored as XML files, although it is planned to move to JSON schemas with the next release of Invenio (version 3). JSON schemas will provide more flexibility and interoperability with other platforms.

The data and metadata on the Open Data Portal are provided under a Creative Commons Public Domain Dedication (CC0). This liberal choice should be enable any kind of reuse and exploitation of these datasets. Similarly, the software releases available via the portal are also published under Open Source licences. Licences are displayed on the individual records on the Portal.

Two example records for primary data are shown below: Image XXX for basic metadata, alongside the Datacite Metadata schema and Image XXX for more specific information such as validation procedures or limitations of the content displayed.

## Preparing user guidance and documentation

As mentioned earlier, performing a physics analyses with the open data from the LHC is far from trivial. To lower the barrier of entry and make the datasets meaningful for students, citizen scientists and members of the wider particle-physics community, clear and thorough documentation has been provided, either on the Portal itself or via external resources stored on CERN webpages.

Performing an analysis on the datasets requires the use of a special software framework, known as [ROOT](https://root.cern.ch/about-root), which was developed at CERN. In addition to ROOT, detector-specific software packages are needed to analyse data from the different LHC collaborations. To streamline access to these tools, the software environments necessary to perform a physics analysis on the LHC datasets are captured using the [CernVM technology](http://cernvm.cern.ch/). The CernVM Virtual Software Appliance provides a complete, portable and easy-to-configure user environment for developing and running LHC data analysis locally or on institutional and commercial clouds (such as OpenStack, Amazon EC2, Google Compute Engine). Use of CernVM removes the need for separately installing the various software packages and libraries. Documentation on the Portal also guides the users through the basic actions needed to familiarise themselves with the tools provided.

Once the datasets, the software environments and the documentation have been
assembled, an important challenge was to present this information in an
easy-to-use way. A considerable effort was therefore devoted to an attractive presentation of assembled data and tools needed to work with them.

Further, precise instructions were provided for getting started with an analysis using the CMS data, by documenting the installation and testing of the applicable virtual machines and the initialisation of the CMS analysis environment. Prior to the release of the data, these steps were extensively tested on a variety of hardware and software configurations. A validation report, based on this testing, was also produced and made available on the Portal.

Yet another barrier -- one that might not seem obvious to those used to working with particle-physics datasets -- is one of vocabulary. This isn't limited just to the terminologies within particle physics -- several terms are used in CMS-specific contexts, referring to the analysis software or to the information recorded in the datasets themselves. A Portal-wide glossary was therefore created; terms included in the glossary are highlighted on all pages on the Portal, and hovering on the term displays the definition. This helps provide contextual information within the documentation.
