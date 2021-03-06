WADO-URI Specification
^^^^^^^^^^^^^^^^^^^^^^

.. _wado-uri-retrieve-imaging-document-set:

WADO-URI Retrieve Imaging Document Set
""""""""""""""""""""""""""""""""""""""

.. csv-table:: WADO-URI Retrieve Imaging Documents Specification
   :header: "Parameter", "Restrictions"
   :file: retrieve-imaging-docs-specs.csv

If the URI Retrieve specifies no transfer syntax that is supported by the archive, the SOP Instance will be returned using the Implicit VR Little Endian Transfer Syntax.

.. _wado-uri-retrieve-rendered-imaging-document-set:

WADO-URI Retrieve Rendered Imaging Document Set
"""""""""""""""""""""""""""""""""""""""""""""""

.. csv-table:: WADO-URI Retrieve Rendered Imaging Documents Specification
   :header: "Parameter", "Restrictions"
   :file: retrieve-rendered-imaging-docs-specs.csv

.. _wado-uri-retrieve-imaging-document-set-metadata:

WADO-URI Retrieve Imaging Document Set Metadata
"""""""""""""""""""""""""""""""""""""""""""""""

Not Supported

.. _wado-uri-connection-policies:

WADO-URI Connection Policies
""""""""""""""""""""""""""""

.. _wado-uri-general:

General
'''''''
All URI connections are limited to HTTP GET requests. The DCM4CHEE-WADO-SERVICE ignores all unknown HTTP header parameters.

.. _wado-uri-number-of-connections:

Number Of Connections
'''''''''''''''''''''
DCM4CHEE-WADO-SERVICE limits the number of simultaneous HTTP connections.

.. csv-table:: Number of HTTP Requests Supported
   :file: common/qido-rs-stow-rs-wado-uri-wado-rs-number-of-connections.csv

.. _wado-uri-asynchronous-nature:

Asynchronous Nature
'''''''''''''''''''
DCM4CHEE-WADO-SERVICE supports HTTP pipelined requests and responses.