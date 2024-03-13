# Trusted Application Pipeline Software Template

This application, **conservative-lizard-java-springboot**, was created from a Trusted Application Pipeline Software Template.

The software templates create a new source and gitops deployment repositories with a sample source application. 

## Repositories

The source code for your application can be found in [https://github.com/rhtap-hub/conservative-lizard-java-springboot ](https://github.com/rhtap-hub/conservative-lizard-java-springboot ).
 
The gitops repository, which contains the kubernetes manifests for the application can be found in 
[https://github.com/rhtap-hub/conservative-lizard-java-springboot-gitops ](https://github.com/rhtap-hub/conservative-lizard-java-springboot-gitops ) 

## Application namespaces 

The default application will be found in the following namespaces. Applications can be deployed into unique namespaces or multiple software templates can also bet generated into the same group namespaces.  

|  Namespace   |  Description   |  
| -------- | -------- |   
| **rhtap-demo-development** | The default application during development. Every build will be deployed to this namespace for testing. | 
| **rhtap-demo-stage** | The staging namespace for this application. Promotion from development to stage is manual via an update to the [gitops repository](https://github.com/rhtap-hub/conservative-lizard-java-springboot-gitops ) in the components/conservative-lizard-java-springboot/overlays/prod directory |  
| **rhtap-demo-prod** | The production namespace for this application. Promotion from stage to production is manual via an update to the [gitops repository](https://github.com/rhtap-hub/conservative-lizard-java-springboot-gitops ) in the components/conservative-lizard-java-springboot/overlays/prod directory | 