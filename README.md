The central, fundamental, component of the OpenCDMS project is the OpenCDMS API.

> Specifically: the OpenCDMS API will be the specification of a universal API for interacting with conformant CDMSs.

We have:

* The abstract [CDMS Specifications](https://library.wmo.int/index.php?lvl=notice_display&id=16300) (2014)
* The OpenCDMS API Specifications (this repository)
* The Reference Implementation: our implementation of the OpenCDMS API specifications

The creation of the OpenCDMS API Specifications here is a broad top-down activity, possibly with the following components:
- Data API
- Process API

The prototyping of an initial Reference Implementation is currently being explored as a bottom-up collaborative activity in
[OpenCDMS Experimental](https://github.com/opencdms-dev):
- [Data API]()
- Process API
  - Hydrological modules (from MCH)
  - Climatological modules (from R-Instat)

Other CDMS developers could also conform to the OpenCDMS API specification and, in doing so,
they could be certified as being conformant. Being conformant to the OpenCDMS API specification
guarantees conformance to the CDMS specifications).
