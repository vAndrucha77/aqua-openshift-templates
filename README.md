# aqua-openshift-templates
Collection of Openshift Templates to deploy Aqua CSP.


## Policy Links
[CSP with Persistent Volume](https://github.com/BryanKMorrow/aqua-openshift-templates/tree/master/csp-with-pv)

## Cluster Prerequistes

## Deployments

## Services

## Routes

## Role Bindings

## Parameters

* name: **DB_PASSWORD**
* required: true
* description: This is the Postgres database password that will be used by the CSP components that communicate with the database. (Created as a string data Opaque secret)
* name: **AQUA_REGISTRY**
* required: true
* description: This is the path to the registry where the CSP images are stored (Example: registry.domain.com or registry.domain.com/aqua) 
* name: **AQUA_TAG**
* required: true
* description: Aqua CSP image tags (Example: 4.2 or 4.2.19918)
* name: **SERVICE_ACCOUNT**
* required: true
* description: The service account is needed if you are using it to pull the CSP images from the Aqua private registry  
* name: **ROUTER**
* required: false
* description: The fully qualified domain name or ip address of the OpenShift node that hosts the OpenShift router.
* name: **DOCKERLESS**
* required: true
* description: Dockerless Scanning (1 is enabled,  0 is disabled) 
* name: **GRPC**
* required: true
* description: Gateway communication uses GRPC (1 is enabled, 0 is disabled)