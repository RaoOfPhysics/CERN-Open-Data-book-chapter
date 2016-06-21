# Solution

- Word count: **3,000**

## Logistics and Infrastructure

A collaborative approach was taken to deliver both the CERN Open Data Portal and the big first open-data release from CMS at the same time. Members of the CMS Collaboration, CERN IT and CERN Scientific Information Service developed the platform, its visualisation tools, the data and software for the release, as well as user guidance and documentation. From the very beginning, it proved to be important to have subject specialists, information specialists and IT experts together on board to tackle the delivery of big complex datasets. As part of this collaboration, CMS has also contributed the visualisation of data on the portal which enables users on the portal to easily select and visualise the data in the detector from various angles. Regular meetings and feedback cycles ensured that the work on the portal and its content was on track and meeting the requirements of the potential users community and use cases.

The CERN Open Data platform is based on the [Invenio digital library framework](http://inveniosoftware.org/)
that was originally developed at CERN and that is now co-developed by an
international collaboration.

Invenio provides an ecosystem of standalone independent packages that permit the
construction of a custom digital repository solution oriented towards various
use cases, such as an integrated library system, a digital document repository,
a multimedia archive, or a data repository. Invenio has been used for numerous
digital library and document repository instances in the world and is
particularly known for its scalability for large scale libraries, such as [CERN
Document Server](http://cds.cern.ch/) or [INSPIRE](http://inspirehep.net/).

In the context of the CERN Open Data Portal, the Invenio framework has been
extended with several general-public oriented features to make the digital
library instance look attractive to high-school students and other targeted
audience (see section 4).

Figure: home page of CODP (see below).

The Invenio digital repository platform manages datasets, software and other
archived assets by means of persistent identifiers to help later referencability
and citability. The platform draws inspiration from the Open Archival
Information System (OAIS) recommended practices to ensure long-term preservation
of captured assets.

The datasets themselves are stored in CERN's [EOS disk storage system](https://eos.web.cern.ch/). EOS is a
disk-based service providing low-latency storage infrastructure for physics
users. The EOS system manages over 120 PB of disk storage at the moment of writing this publication.
The data access is provided by the [XRootD protocol](http://xrootd.org/) and is very well
suited in situations with many concurrent users, significant fraction of random
data access, and large file open rate. The XRootD protocol allows ad-hoc
streaming of necessary portions of data during an analysis, saving general
public from having to prealably download the complete dataset before an analysis
can start.

The captured software environments necessary to reproduce an analysis use the
[CernVM virtual machine technology](http://cernvm.cern.ch/). The CernVM Virtual Software Appliance
represents a complete, portable and easy-to-configure user environment for
developing and running LHC data analysis locally and on institutional and
commercial clouds (OpenStack, Amazon EC2, Google Compute Engine). It removes the
need for the installation of the experiment software.

## Technical

The information architecture of the portal reflects the most prominent known use cases so far (see section 4). Special emphasis has been given on contextual information that are needed to understand and reuse data and software.
On the CERN Open Data Portal each data set has its own record. Related records are aggregated in dedicated collections, e.g. for primary or derived data. This can be considered a standard digital libraries practice, simply adopted to research data. Within each record, metadata is provided. Metadata is standardised according MARC [link]. Inspired by the practices developed by the partner information platforms in HEP (e.g. INSPIRE and CDS), standard metadata fields were populated. However, various additional metadata fields needed to be created to make sure information about data are standardised and comprehensive across (see Table 1). The information provided was "tested" to be comprehensive enough for future reuse of the provided data. Special emphasis was given to complete mandatory fields needed for DOI minting for datasets (e.g. authors, publication year, title, publisher). It is planned to move to JSON Schemas with the next major software upgrade to the forthcoming Invenio 3 framework. This will allow more flexibility and interoperability with other platforms. Work is ongoing in regards to Linked Open Data and defining ontologies for such data in the HEP community.  
The data and metadata on the Open Data Portal are provided under a Creative Commons Public Domain Dedication (CC0). This liberal choice should be enable any kind of reuse and exploitation of the material. Naturally, also the software releases through the portal are published under Open Source licences. They are displayed on the individual data records on the platform.

Two example data records for primary data is shown below: Fig x for basic metadata, alongside the Datacite Metadata schema and Fig y for more specific information such as validation procedures or limitations of the content displayed).

## Documentation
