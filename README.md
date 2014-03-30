## OpenShift Apache Tika Cartridge

A cartridge for OpenShift that provides access to the Apache Tika JAXRS Server. This was prepared for a talk at JBUG Scotland, April 2014.

### Installation

To install this cartridge use the cartridge reflector when creating an application

	rhc create-app myapp http://cartreflect-claytondev.rhcloud.com/reflect?github=Categorize/openshift-tika-cartridge

### Tika Version

The current release (1.5) does not currently has two issues stopping it being useful in an OpenShift environment; its use of binding to the public interface and its lack of an endpoint on the root of the servers URL.

To address these two issues the author has created a custom build of Apache Tika, whilst they are addressed within the trunk code base. Once incorporated the cartridge will use a source code build of the latest trunk.

### Support

This cartridge is provided provided "as is", with absolutely no warranty expressed or implied. Any use is at your own risk.
