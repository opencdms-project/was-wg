# OpenCDMS API

The central component of the OpenCDMS project is the OpenCDMS API. Specifically:
- The OpenCDMS API specifications will define universal APIs for interacting with conformant CDMSs.
- The OpenCDMS Reference Implementation will provide a complete implementation of the OpenCDMS API specifications.

The overall approach and documentation relating to the OpenCDMS API *specifications* will be discussed in this `api` repository. Please use the <kbd>Watch</kbd> button above to receive email updates.

Software other than the OpenCDMS Reference Implementation may also conform to the OpenCDMS API specification and, in doing so,
they could be certified as being conformant. Being conformant to the OpenCDMS API specification
guarantees conformance to the WMO CDMS specifications.

---

The prototyping of an initial Reference Implementation is currently being explored in the following repositories:
- [Data API](https://github.com/opencdms/data-api/) - It is anticipated that the OpenCDMS Data API may define an extention to the [OGC API - Features](https://www.opengeospatial.org/standards/ogcapi-features) standard. In addition to supporting operations on features, the Data API will also provide controlled access to other resources.
- [Process API](https://github.com/opencdms/process-api/) (potentially utilising [OGC API - Processes](https://github.com/opengeospatial/wps-rest-binding)). Process will include:
  - Hydrological modules (from [MCH](http://www.wmo.int/pages/prog/hwrp/mch/))
  - Climatological modules (from [R-Instat](http://r-instat.org) and [Climatol](https://CRAN.R-project.org/package=climatol))
- Coverages API (using/extending [OGC API - Coverages](https://github.com/opengeospatial/ogc_api_coverages)). Gridded data (e.g. satellite imagery) may use/extend the `OGC API - Coverages` standard. The work of the OGC MetOcean WG (e.g. [
MetOcean Hack](https://www.opengeospatial.org/metoceanhack)) will also be reviewed, although this may apply more to multi-level model data.

The *reference implementation* (RI) of the OpenCDMS API specifications will be one realisation of the WMO [CDMS Specifications](https://library.wmo.int/index.php?lvl=notice_display&id=16300) (2014).
