## Cataloguing data and analysis tools

The CERN Open Data Portal has been developed to serve two main use cases: education and research (see more under Section 4). This is reflected in the information architecture of the Portal itself. It should be noted that special emphasis has been given to providing contextual information that is needed to understand and reuse the data and accompanying software.

On the Portal each dataset has its own record. Related records are aggregated in dedicated collections, such as those for "Primary datasets" or "Derived datasets". This aggregation, which is standard practice in digital libraries, has been adopted to research data. Further, metadata -- standardised according to MARC\footnote{\url{https://en.wikipedia.org/wiki/MARC_standards}} -- are provided within each record. Adopting the practices developed by partner information platforms in high-energy physics (e.g. INSPIRE and CDS), standard metadata fields were populated. However, various additional metadata fields needed to be created to make sure information about data are standardised and comprehensive across all the datasets available via the Portal.

The information provided was vetted to be comprehensive enough for future reuse of the data. Certain fields, such as the names of the authors, the publication year, title of the dataset, name of the publisher, were made mandatory for the sake of minting DOIs.

The metadata are currently stored as XML files, although it is planned to move to JSON schemas with the next release of Invenio (version 3). JSON schemas will provide more flexibility and interoperability with other platforms.

The data and metadata on the Portal are provided under a Creative Commons Public Domain Dedication (CC0). This liberal choice should enable any kind of reuse and exploitation of these datasets. Similarly, the software releases available via the portal are also published under Open Source licences. The respective licences are displayed on the individual records on the Portal.

Two example records for primary data are shown below: Image XXX for basic metadata, alongside the Datacite Metadata schema and Image XXX for more specific information such as validation procedures or limitations of the content displayed.
