## Developing the platform

The CERN Open Data platform is based on the Invenio digital library framework\footnote{\url{http://inveniosoftware.org/}}, which was originally developed at CERN and is now co-developed by an international collaboration.

Invenio provides an ecosystem of standalone independent packages that can be used to build custom digital repositories. Use cases for Invenio include integrated library systems, digital document repositories, multimedia archives and data repositories. The software framework has been used for numerous such instances around the world and is particularly known for its scalability for large libraries, such as CERN Document Server (CDS)\footnote{\url{https://cds.cern.ch/}} or INSPIRE\footnote{\url{https://inspirehep.net/}}.

Invenio is mainly used in academic environments. In order to make the CERN Open Data Portal attractive to the general public, including high-school students and other targeted audiences, several features such as documentation pages and glossaries have been included on the Portal. Image XXX shows the home page of the CERN Open Data Portal.

A crucial aspect of providing open data is to ensure the long-term preservation of the datasets, as well as the accompanying software tools. Invenio enables the persistence and longevity of the Portal's assets, drawing inspiration from recommended practices of the Open Archival Information System (OAIS)\footnote{\url{https://en.wikipedia.org/wiki/Open_Archival_Information_System}}. As part of this, persistent identifiers -- in this case Digital Object Identifiers (DOIs) -- ensure that the datasets and software tools can be referenced and cited well into the foreseeable future.

The datasets available on the CERN Open Data Portal are themselves stored in CERN's EOS\footnote{\url{https://eos.web.cern.ch/}} disk storage system. EOS is a disk-based service that provides low-latency storage infrastructure for physics use cases. EOS manages over 120 petabytes (PB) of disk storage at the time of writing this chapter. Access to the open data is provided by the XRootD\footnote{\url{http://xrootd.org/}} protocol and is well suited to situations with many concurrent users, a significant fraction of random data access, and a large rate of file opening. The XRootD protocol allows ad-hoc streaming of necessary portions of data during an analysis, saving potential users of the large datasets from having to preemptively download the complete datasets before starting an analysis.

In the spirit of openness, development work for the Portal is conducted publicly on the code-sharing platform, GitHub\footnote{\url{https://github.com/cernopendata/opendata.cern.ch}}.