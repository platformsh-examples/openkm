# OpenKM for Platform.sh

<p align="center">
<a href="https://console.platform.sh/projects/create-project/?template=https://raw.githubusercontent.com/platformsh-examples/openkm/master/.platform.template.yaml&utm_campaign=deploy_on_platform?utm_medium=button&utm_source=affiliate_links&utm_content=https://raw.githubusercontent.com/platformsh-examples/openkm/master/.platform.template.yaml" target="_blank" title="Deploy with Platform.sh"><img src="https://platform.sh/images/deploy/deploy-button-lg-blue.svg"></a>
</p>

This project provides a starter kit for OpenKM projects hosted on Platform.sh.


OpenKM is a Free/Libre document management system that provides a web interface for managing nonspecific files. OpenKM includes a content repository, Lucene indexing, and jBPM workflow. The OpenKM system was developed using open technology. 

## Features

* Java 8
* PostgreSQL
* Automatic TLS certificates

## Post-install

1. Set the plan to a Large one.
2. Go to login page: User `okmAdmin`  the password: `admin`
3. Change the password on:  `Tools` -> `Preferences` -> `User configuration`

## Customizations

The following files and additions make the Jenkins work.  If using this project as a reference for your own existing project, replicate the changes below to your project.

* [`.platform/routes.yaml`](.platform/routes.yaml): Platform.sh allows you to define the [routes](https://docs.platform.sh/configuration/routes.html).
* [`.platform/services.yaml`](.platform/services.yaml):  Platform.sh allows you to completely define and configure the topology and [services you want to use on your project](https://docs.platform.sh/configuration/services.html).
* [`.platform.app.yaml`](.platform.app.yaml): You control your application and the way it will be built and deployed on Platform.sh [via a single configuration file](https://docs.platform.sh/configuration/app-containers.html).

## References

* [OpenKM](https://www.openkm.com/)
* [Java at Platform.sh](https://docs.platform.sh/languages/java.html)
