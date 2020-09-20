# OpenKM for Platform.sh

<p align="center">
<a href="https://console.platform.sh/projects/create-project?template=https://raw.githubusercontent.com/platformsh/template-builder/master/templates/jenkins/.platform.template.yaml&utm_content=jenkins&utm_source=github&utm_medium=button&utm_campaign=deploy_on_platform">
    <img src="https://platform.sh/images/deploy/lg-blue.svg" alt="Deploy on Platform.sh" width="180px" />
</a>
</p>

This project provides a starter kit for OpenKM projects hosted on Platform.sh.


OpenKM is a Free/Libre document management system that provides a web interface for managing nonspecific files. OpenKM includes a content repository, Lucene indexing, and jBPM workflow. The OpenKM system was developed using open technology. 

## Features

* Java 8
* PostgreSQL
* Automatic TLS certificates
* Jenkins downloaded on the fly during build

## Post-install

1. After creating a Jenkins project, the post-installation setup wizard begins.
2. When you first access a new Jenkins instance, you are asked to unlock it using an automatically-generated password.
3. Browse to the Jenkins service link and wait until the Unlock Jenkins page appears.
4. From the Jenkins console log output, copy the automatically-generated alphanumeric password
5. (Execute: `platform ssh cat /app/.jenkins/secrets/initialAdminPassword` and copy the output)[https://docs.platform.sh/development/access-site.html#accessing-the-application-with-ssh]
6. On the Unlock Jenkins page, paste this password into the Administrator password field and click Continue.

## Customizations

The following files and additions make the Jenkins work.  If using this project as a reference for your own existing project, replicate the changes below to your project.

* [`.platform/routes.yaml`](.platform/routes.yaml): Platform.sh allows you to define the [routes](https://docs.platform.sh/configuration/routes.html).
* [`.platform/services.yaml`](.platform/services.yaml):  Platform.sh allows you to completely define and configure the topology and [services you want to use on your project](https://docs.platform.sh/configuration/services.html).
* [`.platform.app.yaml`](.platform.app.yaml): You control your application and the way it will be built and deployed on Platform.sh [via a single configuration file](https://docs.platform.sh/configuration/app-containers.html).

## References

* [OpenKM](https://www.openkm.com/)
* [Java at Platform.sh](https://docs.platform.sh/languages/java.html)
