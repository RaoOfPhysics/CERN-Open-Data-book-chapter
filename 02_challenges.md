# Challenges

- Themes:
    1. Volume of data
    2. Software environment and documentation
- Word count: **2,000**
- Authors: All

---

Since the LHC began delivering collisions in 2010 and as of writing this document (March 2016), the four detectors have recorded a total volume of [FIXME INSERT NUMBER HERE] of data. It is important to note that these data represent a tiny fraction (FIXME 0.000000000??%) of the total data *generated* by the LHC. Performing an analysis on this volume of data is far from trivial. First, the data from the collisions, which are in the form of electrical signals from individual channels within each detector, must be pieced together or reconstructed to form a coherent image of the collision itself. Then, analysis software must sift through trillions upon trillions of collisions to look for signatures associated with physics phenomena.

The LHC collaborations rely on the Worldwide LHC Computing Grid (or the Grid, for short) to perform these analysis tasks. The Grid is a network of interconnected computers distributed all over the globe, and datasets are broken into chunks to facilitate processing. While those outside the LHC collaborations don't typically have access to these resources, it is worth pointing out that the open data from the detectors is already "reconstructed" and "reprocessed" — that is, a lot of the gruntwork has already been done to prepare the datasets into a form useful for the final analyses themselves. Despite this, analysing the "analysable" data is no easy task. To make life easier, we have provided "derived" or simplified datasets along with the code used to prepare them, so that these smaller datasets can be used for analysis in a classroom or university environment without a large technological overhead.

The appropriate software environments necessary for the analyses are also provided, often in the form of virtual machines that have been tested on a variety of hardware and software configurations. Documentation will also guide the users through the basic actions needed to familiarise themselves with the tools provided.

Once the datasets, the software environments and the documentation have been
assembled, an important challenge was to present this information in an
easy-to-use and attractive way for the targeted non-specialist audience,
consisting of non-physics, citizen scientists, general public, or high-school
students learning about particle physics. A considerable effort was therefore
devoted to an attractive presentation of assembled data and the ease-of-use of
tools permitting to work with it.