# Example pipeline for helloworld node application 
Bluemix Containers have gone live!  Before you start with this example you need to setup a namespace.  The namespace is set for each organization and will be used for your image repositories names in your organizations private Container Registry.  To setup a namespace, simply login to [Bluemix](https://bluemix.net), and click ![Start Containers](start-containers.jpg).  
If you have not setup a namespace you will be asked to.  Even if you were a beta participant you will need to create a new namespace.  

Now press this button, to get your own copy of the sample running in Bluemix !

[![Deploy To Bluemix](https://bluemix.net/deploy/button.png)](https://bluemix.net/deploy?repository=https://github.com/Puquios/hello-containers.git)

## Overview 
IBM DevOps Services has a Continuous Delivery Pipeline for deploying Cloud Foundry applications, containers, and micro-services to IBM Bluemix. You can use a textual representation of a pipeline defined by a pipeline.yml file, which makes it easy to share and copy interesting pipelines. The Deploy to Bluemix button provides a simple way to clone a project that includes the source files and the Delivery Pipeline configuration. 

## The application 
Helloworld node application

## The pipeline 
As simple as it gets
- Build 
    + Leverages the container build service to take the Dockerfile in the root of the project, builds a docker image that is versioned by tagging based on the build number, and pushes the image to your orgnanization's registry on IBM Bluemix. 
- Deploy 
    + • Using the container image from the Build stage, a container group is deployed with a single container to start with, and then a route is generated for the Deploy stage that will be reused across deployments.

## References 
- [Blog on continuous delivery for containers](https://developer.ibm.com/bluemix/docs/set-up-continuous-delivery-ibm-containers/)
- [IBM DevOps Services](http://hub.jazz.net)
- [IBM Bluemix](http://bluemix.net)
