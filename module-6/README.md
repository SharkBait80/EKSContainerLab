# Module 6 - Dockerize the Sample Application


**Time to complete:** 20 minutes

**Services used:**


### Overview

In this module, we will add Docker support to our app and containerize it. 

If you are new to Docker or using Docker with .NET, it is recommended to read [this first](https://docs.microsoft.com/en-us/dotnet/core/docker/intro-net-docker) to give you a quick overview of Docker basics. You can skip the Azure section. :-)

Firstly, install [Visual Studio Tools for Docker](https://docs.microsoft.com/en-us/dotnet/standard/containerized-lifecycle-architecture/design-develop-containerized-apps/visual-studio-tools-for-docker) which will allow you to access Docker tooling from within Visual Studio.

![Adding Docker support from Visual Studios](/images/module-6/AddDockerSupport-2.jpg)

Visual Studio should have created a Dockerfile for you. The next step is to run the application in a container, following [this guide](https://docs.microsoft.com/en-us/dotnet/core/docker/build-container#create-the-dockerfile).

Tips:

_The application expects an input file which isn't copied into the Docker image by default. How can you get this copied into the right location?_

_You might see errors like 'duplicate assembly information', which is caused by the presence of an AssemblyInfo.cs file in your project having updated from .NET to .NET Core. You should delete this to prevent them from being included in the build._

## Next

Please proceed to the next lesson.

**[Proceed to Module 7](/module-7)**


### [AWS Developer Center](https://developer.aws)
