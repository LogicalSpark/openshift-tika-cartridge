## OpenShift Apache Tika Server Cartridge

A cartridge for OpenShift that provides access to the Apache Tika JAXRS Server. This was prepared for a talk at JBUG Scotland, April 2014.

### Installation

To install this cartridge use the cartridge reflector when creating an application

	rhc create-app myapp http://cartreflect-claytondev.rhcloud.com/reflect?github=Categorize/openshift-tika-cartridge

It has been developed to support scaling with a scaleable application, so if you would like use it in this way you can use the -s flag

	rhc create-app myapp http://cartreflect-claytondev.rhcloud.com/reflect?github=Categorize/openshift-tika-cartridge -s

### Tika Version

The current release (1.5) does not currently has two issues stopping it being useful in an OpenShift environment; its use of binding to the public interface and its lack of an endpoint on the root of the servers URL.

To address these two issues the author (an Apache Tika commiter) has created a custom binary build of Apache Tika based on the trunk on the 28th of March 2014 for use whilst the issues are addressed within the trunk code base. Once incorporated the cartridge will use a source code build of the latest trunk.

### Tika Server Usage

You can read about the TIKA JAXRS server [here](http://wiki.apache.org/tika/TikaJAXRS).

### Support

This cartridge is provided provided "as is", with absolutely no warranty expressed or implied. Any use is at your own risk.
