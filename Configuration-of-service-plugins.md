Service plugins are configured in the main `mqttwarn.ini` file. Each service has a mandatory _section_ named `[config:_service_]`, where _service_ is the name of the service. This section _may_ have some settings which are required for a particular service. One mandatory option is called `targets`. This defines individual "service points" for a particular service, e.g. different paths for the `file` service, distinct database tables for `mysql`, etc.

We term the array for each target an "address list" for the particular service. These may be path names (in the case of the `file` service), topic names (for outgoing `mqtt` publishes), hostname/port number combinations for `xbmc`, etc.

* [file](https://github.com/jpmens/mqttwarn/wiki/file)
* [gss](https://github.com/jpmens/mqttwarn/wiki/gss)