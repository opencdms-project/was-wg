The central component of the OpenCDMS project is the OpenCDMS API.

> Specifically:
> - The OpenCDMS API specifications will define universal APIs for interacting with conformant CDMSs.
> - The OpenCDMS Reference Implementation will provide a complete implementation of the OpenCDMS API specifications.

The OpenCDMS API specifications, developed in this repository,
are one realisation of the WMO [CDMS Specifications](https://library.wmo.int/index.php?lvl=notice_display&id=16300) (2014).

The creation of the OpenCDMS API Specifications is a broad top-down activity, possibly comprising the following components:
- Data API (extending [OCG API - Features](https://www.opengeospatial.org/standards/ogcapi-features))
- Process API (using [OGC API - Processes](https://github.com/opengeospatial/wps-rest-binding))
- Coverages API (using/extending [OGC API - Coverages](https://github.com/opengeospatial/ogc_api_coverages))

It is anticipated that the OpenCDMS Data API will define an extention to the `OGC API - Features` standard.
In addition to supporting operations on features, the Data API will also provide controlled access to other resources.

`OGC API - Processes` is likely to be used directly.

Gridded data (e.g. satellite imagery) will use/extend the `OGC API - Coverages` standard. The work of the OGC MetOcean WG (e.g. [
MetOcean Hack](https://www.opengeospatial.org/metoceanhack)) will also be reviewed
(although this may apply more to multi-level model data).

The prototyping of an initial Reference Implementation is currently being explored as a bottom-up collaborative activity in
[OpenCDMS Experimental](https://github.com/opencdms-dev):
- [Data API](https://github.com/opencdms-dev/data-api)
- Process API
  - Hydrological modules (from [MCH](http://www.wmo.int/pages/prog/hwrp/mch/))
  - Climatological modules (from [R-Instat](http://r-instat.org))

Software other than the OpenCDMS Reference Implementation may also conform to the OpenCDMS API specification and, in doing so,
they could be certified as being conformant. Being conformant to the OpenCDMS API specification
guarantees conformance to the WMO CDMS specifications.
