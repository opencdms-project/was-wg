The central component of the OpenCDMS project is the OpenCDMS API.

> Specifically: the OpenCDMS API will be the specification of a universal API for interacting with conformant CDMSs.

We have:

* The abstract [CDMS Specifications](https://library.wmo.int/index.php?lvl=notice_display&id=16300) (2014)
* The OpenCDMS API Specifications (this repository)
* The Reference Implementation: our implementation of the OpenCDMS API specifications

The creation of the OpenCDMS API Specifications here is a broad top-down activity, possibly with the following components:
- Data API (extending [OCG API - Features](https://www.opengeospatial.org/standards/ogcapi-features))
- Process API (using [OGC API -Processes](https://github.com/opengeospatial/wps-rest-binding))
- Coverages API (possibly separate from Data API, see below)

It is anticipated that OpenCDMS will define an extention to the `OGC API - Features` standard, whilst using `OGC API - Processes` directly.

Gridded data (e.g. satellite imagery) maybe available through the OpenCDMS Data API, but will use/extend the `OGC API - Coverages` standard. The work of the OGC MetOcean WG (e.g. [
MetOcean Hack(https://www.opengeospatial.org/metoceanhack)) may also be relevant
although this may apply more to multi-level model data.

The prototyping of an initial Reference Implementation is currently being explored as a bottom-up collaborative activity in
[OpenCDMS Experimental](https://github.com/opencdms-dev):
- [Data API](https://github.com/opencdms-dev/data-api)
- Process API
  - Hydrological modules (from [MCH](www.wmo.int/pages/prog/hwrp/mch/))
  - Climatological modules (from [R-Instat](http://r-instat.org))

Other CDMS developers could also conform to the OpenCDMS API specification and, in doing so,
they could be certified as being conformant. Being conformant to the OpenCDMS API specification
guarantees conformance to the CDMS specifications).
