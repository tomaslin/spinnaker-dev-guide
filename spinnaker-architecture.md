# Spinnaker Project Architecture

## Navigating the Spinnaker Github project

The Spinnaker github project \([https://github.com/spinnaker/](https://github.com/spinnaker/\)\) exposes several projects, they can be broken down as follows:

### Microservices

Deployed together, these services make up the Spinnaker stack.

[**Deck**](https://github.com/spinnaker/deck)**: **User interface for Spinnaker.

[**Gate**](https://github.com/spinnaker/gate)**: **API proxy for Spinnaker microservices.** **

[**Orca**](https://github.com/spinnaker/orca)**:** Orchestration engine for Spinnaker tasks.

[**Clouddriver**](https://github.com/spinnaker/clouddriver)**: **Cloud driver is the service responsible for talking to the underlying cloud service that Spinnaker deploys to.

[**Front50:**](https://github.com/spinnaker/front50)** **Front50 provides persistent data storage to the rest of Spinnaker. When integrated with S3 \(or an S3 compatible API\), Front50 also provides versioning support for pipelines, applications and strategies. **  **

[**Echo**](https://github.com/spinnaker/echo)**: **Echo is the Spinnaker service listener. It is responsible for enforcing pipeline triggering and pipeline notifications.

[**Igor**](https://github.com/spinnaker/igor)**:** Igor monitors new Jenkins and Docker Registry builds and triggers echo events.

[**Rosco**](https://github.com/spinnaker/rosco)**: **Rosco is used for baking - transforming artifacts into cloud images. Uses packer under the hood.

[**Fiat**](https://github.com/spinnaker/fiat)**: **Fiat is responsible for authentication of service calls.

### Tools

[**Spinnaker**](https://github.com/spinnaker/spinnaker)**: **The top level spinnaker project provides the following functionality:

* Issue Tracking - \( [https://github.com/spinnaker/spinnaker/issues](https://github.com/spinnaker/spinnaker/issues) \)
* Experimental Deployment Support - \( [https://github.com/spinnaker/spinnaker/tree/master/experimental](https://github.com/spinnaker/spinnaker/tree/master/experimental) \)
* Common Configuration - \( [https://github.com/spinnaker/spinnaker/tree/master/config](https://github.com/spinnaker/spinnaker/tree/master/config) \)
* Single Image deployment configuration - \( https://github.com/spinnaker/spinnaker \)

[**Halyard**](https://github.com/spinnaker/halyard)**:** Halyard is a command line tool that makes it easier to configure Spinnaker.

### Libraries

[**Spinnaker-dependencies**](https://github.com/spinnaker/spinnaker-dependencies)**: **This project is used to manage the versions of common libraries used by all the Spinnaker microservices.

[**Spinnaker-gradle-project**](https://github.com/spinnaker/spinnaker-gradle-project)**: **This library is used across all Spinnaker microservices to provide common gradle functionality and centralizes logic for deploying build artifacts.

[**Kork**](https://github.com/spinnaker/kork)**: **Kork provides Spring bindings for NetflixOSS projects.

