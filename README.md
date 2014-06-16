google-gcloud
=============

*This* repository contains polymer elements for interacting
with [Google Cloud Platform](http://example.com/) services. 

### Naming Conventions
Google Cloud Platform (GCP) encompasses a wide variety of 
products and APIs so it's important to establish a clear and
consistent naming scheme for the components we created
for interacting with GCP.

We will following the naming scheme implemented by the 
[Google Cloud SDK](https://developers.google.com/cloud/sdk/), 
which has estbalished a well defined collection of commands 
and subcommands for requesting GCP services.

Our model is to map the service identification part of the
Cloud SDK's command syntax into a hyphen separated element
name, which gives us the following mappings:

| Cloud SDK Name | Polymer ELement Name |
|________________|______________________|


### Current Status of this Element Collection
