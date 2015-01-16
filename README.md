## OpenShift Apache Tika Server Cartridge

A cartridge for OpenShift that provides access to the Apache Tika JAXRS Server. This was prepared for a talk at JBUG Scotland, April 2014.

### Installation

To install this cartridge use the cartridge reflector when creating an application

	rhc create-app myapp http://cartreflect-claytondev.rhcloud.com/reflect?github=LogicalSpark/openshift-tika-cartridge

It has been developed to support scaling with a scaleable application, so if you would like use it in this way you can use the -s flag

	rhc create-app myapp http://cartreflect-claytondev.rhcloud.com/reflect?github=LogicalSpark/openshift-tika-cartridge -s

### Tika Version

This cartridge supports Apache Tika Version 1.7, released on 15th of January 2015.

### Tika Server Usage

If you would like to try out the Apache Tika JAXRS server you can find a deployed instance using this cartridge at:
	
	http://tikaserver-logicalspark.rhcloud.com/

To extract the contents of a file, you can use the following:

	curl -T <file> http://tikaserver-logicalspark.rhcloud.com/tika

To extract the metadata of a file, you can use the following:

	curl -T <file> http://tikaserver-logicalspark.rhcloud.com/meta

You can read more about the TIKA JAXRS server and it's commands [here](http://wiki.apache.org/tika/TikaJAXRS).

### Support

This cartridge is provided provided "as is", with absolutely no warranty expressed or implied. Any use is at your own risk.
