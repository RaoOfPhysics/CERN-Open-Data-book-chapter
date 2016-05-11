#Solution

- Themes:
    1. Logistical (Authors: @TimSmithCH): Collaborative approach, Invenio 
    2. Technical –– schema, formats etc. (Authors: @suenjedt, @pherterich): MARC standards, customzied fields for new data types, soon JSON
    3. Documentation (Authors: @katilp, @RaoOfPhysics)
- Word count: **3,000**

Logistical:

A collaborative approach was taken to deliver the CERN Open Data Portal and the big first open data release for CMS at the same time. Members of the CMS collaboration, CERN IT and CERN Scientific Information service developed the platform, its visualization tools, the data and software (access) for the release, as well as user guidance and documentation. From the very beginning, it proved to be important to have subject specialists, information specialists and information technology experts together on board to tackle the delivery of big complex datasets. As part of this collaboration, CMS has also contributed the vizualization of data on the portal which enables users on the portal to easily select and vizualize the data in the detector from various angles. Regular meetings and feedback cycles ensured that the work on the portal and its content was on track and meeting the requirements of the potential users community and use cases. 


Technical:

The platform is based on the digital library framework Invenio [link] which is also developed at CERN. It has been used for numerous digital libraries and repositories around the world and is particularly known for its scalability for large scale libraries, e.g. the INSPIREHEP or CERN Document Server. 
Using this digital library platform technology provides users with sophisticated search technology while preservation standards are ensured and preservation practices facilitated. Invenio workflows adhere to OAIS. This should help improving the access to resources that have only been available behind closed doors so far. 
[!FIX ME: this needs some more tech details]


Documentation:

The information architecture of the portal reflects the most prominent known use cases so far (see chapter 4). Special emphasis has been given on contextual information that are needed to understand and reuse data and software. 
On the CERN Open Data Portal each data set has its own record. Related records are aggregated in dedicated collections, e.g. for primary or derived data. This can be considered a standard digital libraries practice, simply adopted to research data. Within each record, metadata is provided. Metadata is standardised according MARC [link]. Inspired by the practices developed by the partner information platforms in HEP (e.g. INSPIRE and CDS), standard metadata fields were populated. However, various additional metadata fields needed to be created to make sure information about data are standardized and comprehensive across - as this was the first time such data would be shared in public. The information provided was "tested" to be comprehensive enough for future reuse of the provided data. Special emphasis was given to complete mandatory fields needed for DOI minting for datasets (e.g. authors, publication year, title, publisher). It is planned to move to JSON Schemas with the next major software upgrade to the forthcoming Invenio 3 framework. This will allow more flexibility and interoperability with other platforms. 
The data and metadata on the Open Data Portal are provided under a Creative Commons Public Domain Dedication (CC0). This liberal choice should be enable any kind of reuse and exploitation of the material. Naturally, also the software releases through the portal are published under Open Source licences. All these are documented in the individual records, alongside notes about validation procedures or limitations of the content displayed. 

An example data record for primary data is shown below (Fig x for basic metadata and y for more specific information). 


