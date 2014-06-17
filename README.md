google-gcloud
=============

This repository contains polymer elements for interacting
with [Google Cloud Platform](http://example.com/) services. 

### Naming Conventions
Google Cloud Platform (GCP) encompasses a wide variety of 
products and APIs so it's important to establish a clear and
consistent naming scheme for the associated components. 
We will following the naming scheme implemented by the 
[Google Cloud SDK](https://developers.google.com/cloud/sdk/), 
which has established a well defined naming scheme for a
collection of commands and subcommands for requesting GCP 
services.

Our approach is to map the service identification part of the
Cloud SDK's command syntax into a hyphen separated element
name, which gives us the following mappings:

| Cloud SDK Syntax   | Polymer Element Name |
| ------------------ | -------------------- |
| gcloud auth        | gcloud-auth          |
| gcloud config      | gcloud-config        |
| App Engine(*)      | gcloud-appengine     |
| BigQuery(*)        | gcloud-bigquery      |
| gcloud compute     | gcloud-compute       |
| Cloud Datastore(*) | gcloud-datastorage   |
| gcloud dns         | gcloud-dns           |
| Cloud Storage      | gcloud-storage       |
| gcloud sql         | gcloud-sql           |

(*) = command not yet implemented in Cloud SDK.

Within each product (e.g. gcloud-compute, gcloud-storage), 
there will be a potentially large number of sub-components
(e.g. gcloud-compute-instance, gcloud-compute-disk, 
gcloud-storage-bucket, gcloud-storage-object, etc.).
The taxonomy for each set of sub-components will necessarily
vary by product and is left to the design and implementation 
of each product's components. Wherever possible, designers 
of new components in this collection should take care to 
following the naming contention described here, i.e. to 
choose names that model those used by the Cloud SDK and 
to try to be consistent with other components in this 
collection.

### Current Status of this Element Collection

This component collection is still in a very early state
of development. Initially, it includes functionality for 
a small subset of the full suite of components anticipated, 
however, the goal is to expand this collection over time 
to provide a comprehensive set of declarative web components 
for interacting with the full set of Google Cloud Platform
products and services. 

Interested in contributing? We'd love to have your help!
Please fill out either the individual or corporate 
Contributor License Agreement (CLA):

* If you are an individual writing original source code and 
you're sure you own the intellectual property, then you'll 
need to sign an [https://developers.google.com/open-source/cla/individual](individual CLA).

* If you work for a company that wants to allow you to contribute your work, then you'll need to sign a [https://developers.google.com/open-source/cla/corporate](corporate CLA).

Follow either of the two links above to access the appropriate 
CLA and instructions for how to sign and return it. Once we 
receive it, we'll be able to accept your pull requests.
