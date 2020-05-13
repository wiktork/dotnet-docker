## Important: Client Firewall Rules Update to Microsoft Container Registry (MCR)

To provide a consistent FQDNs, the data endpoint will be changing from *.cdn.mscr.io to *.data.mcr.microsoft.com

For more info, see [MCR Client Firewall Rules](https://aka.ms/mcr/firewallrules).
---------------------------------------------------------------------------------

The images from the dotnet/nightly repositories include last-known-good (LKG) builds for the next release of [.NET](https://github.com/dotnet/core).

See [dotnet/dotnet-docker](https://hub.docker.com/r/microsoft/dotnet/) for images with official releases of [.NET](https://github.com/dotnet/core).

As part of the transition to .NET 5.0, Docker repos for .NET 5.0 and higher do not include `core` in the name as was done with older versions. As an example, ASP.NET Core 5.0 can be found at `mcr.microsoft.com/dotnet/nightly/aspnet:5.0` while 3.1 is still at `mcr.microsoft.com/dotnet/core-nightly/aspnet:3.1`. See the [related issue](https://github.com/dotnet/dotnet-docker/issues/1765) for more details.

# Featured Tags

* `5.0` (Preview)
  * `docker pull mcr.microsoft.com/dotnet/nightly/aspnet:5.0`

# About This Image

This image contains the ASP.NET Core and .NET Core runtimes and libraries and is optimized for running ASP.NET Core apps in production.

Watch [dotnet/announcements](https://github.com/dotnet/announcements/labels/Docker) for Docker-related .NET announcements.

# How to Use the Image

The [.NET Docker samples](https://github.com/dotnet/dotnet-docker/blob/master/samples/README.md) show various ways to use .NET Core and Docker together. See [Building Docker Images for .NET Applications](https://docs.microsoft.com/dotnet/core/docker/building-net-docker-images) to learn more.

## Container sample: Run a web application

You can quickly run a container with a pre-built [.NET Docker image](https://hub.docker.com/_/microsoft-dotnet-core-samples/), based on the [ASP.NET Core sample](https://github.com/dotnet/dotnet-docker/blob/master/samples/aspnetapp/README.md).

Type the following command to run a sample web application:

```console
docker run -it --rm -p 8000:80 --name aspnetcore_sample mcr.microsoft.com/dotnet/core/samples:aspnetapp
```

After the application starts, navigate to `http://localhost:8000` in your web browser.

See [Hosting ASP.NET Core Images with Docker over HTTPS](https://github.com/dotnet/dotnet-docker/blob/master/samples/host-aspnetcore-https.md) to use HTTPS with this image.

# Related Repos

.NET Core 2.1/3.1:

* [dotnet/core](https://hub.docker.com/_/microsoft-dotnet-core/): .NET Core
* [dotnet/core/samples](https://hub.docker.com/_/microsoft-dotnet-core-samples/): .NET Core Samples

.NET 5.0+:

* [dotnet](https://hub.docker.com/_/microsoft-dotnet/): .NET
* [dotnet/nightly](https://hub.docker.com/_/microsoft-dotnet-nightly/): .NET (Preview)
* [dotnet/nightly/sdk](https://hub.docker.com/_/microsoft-dotnet-nightly-sdk/): .NET SDK (Preview)
* [dotnet/nightly/runtime](https://hub.docker.com/_/microsoft-dotnet-nightly-runtime/): .NET Runtime (Preview)
* [dotnet/nightly/runtime-deps](https://hub.docker.com/_/microsoft-dotnet-nightly-runtime-deps/): .NET Runtime Dependencies (Preview)

.NET Framework:

* [dotnet/framework](https://hub.docker.com/_/microsoft-dotnet-framework/): .NET Framework, ASP.NET and WCF
* [dotnet/framework/samples](https://hub.docker.com/_/microsoft-dotnet-framework-samples/): .NET Framework, ASP.NET and WCF Samples

# Full Tag Listing

## Linux amd64 Tags
##### .NET 5.0 Preview Tags
Tags | Dockerfile | OS Version
-----------| -------------| -------------
5.0.0-preview.3-buster-slim, 5.0-buster-slim, 5.0.0-preview.3, 5.0 | [Dockerfile](https://github.com/dotnet/dotnet-docker/blob/master/5.0/aspnet/buster-slim/amd64/Dockerfile) | Debian 10
5.0.0-preview.3-alpine3.11, 5.0-alpine3.11, 5.0.0-preview.3-alpine, 5.0-alpine | [Dockerfile](https://github.com/dotnet/dotnet-docker/blob/master/5.0/aspnet/alpine3.11/amd64/Dockerfile) | Alpine 3.11
5.0.0-preview.3-focal, 5.0-focal | [Dockerfile](https://github.com/dotnet/dotnet-docker/blob/master/5.0/aspnet/focal/amd64/Dockerfile) | Ubuntu 20.04

## Linux arm64 Tags
##### .NET 5.0 Preview Tags
Tags | Dockerfile | OS Version
-----------| -------------| -------------
5.0.0-preview.3-buster-slim-arm64v8, 5.0-buster-slim-arm64v8, 5.0.0-preview.3, 5.0 | [Dockerfile](https://github.com/dotnet/dotnet-docker/blob/master/5.0/aspnet/buster-slim/arm64v8/Dockerfile) | Debian 10
5.0.0-preview.3-alpine3.11-arm64v8, 5.0-alpine3.11-arm64v8, 5.0.0-preview.3-alpine-arm64v8, 5.0-alpine-arm64v8 | [Dockerfile](https://github.com/dotnet/dotnet-docker/blob/master/5.0/aspnet/alpine3.11/arm64v8/Dockerfile) | Alpine 3.11
5.0.0-preview.3-focal-arm64v8, 5.0-focal-arm64v8 | [Dockerfile](https://github.com/dotnet/dotnet-docker/blob/master/5.0/aspnet/focal/arm64v8/Dockerfile) | Ubuntu 20.04

## Linux arm32 Tags
##### .NET 5.0 Preview Tags
Tags | Dockerfile | OS Version
-----------| -------------| -------------
5.0.0-preview.3-buster-slim-arm32v7, 5.0-buster-slim-arm32v7, 5.0.0-preview.3, 5.0 | [Dockerfile](https://github.com/dotnet/dotnet-docker/blob/master/5.0/aspnet/buster-slim/arm32v7/Dockerfile) | Debian 10

## Windows Server, version 1909 amd64 Tags
##### .NET 5.0 Preview Tags
Tag | Dockerfile
---------| ---------------
5.0.0-preview.3-nanoserver-1909, 5.0-nanoserver-1909, 5.0.0-preview.3, 5.0 | [Dockerfile](https://github.com/dotnet/dotnet-docker/blob/master/5.0/aspnet/nanoserver-1909/amd64/Dockerfile)

## Windows Server, version 1903 amd64 Tags
##### .NET 5.0 Preview Tags
Tag | Dockerfile
---------| ---------------
5.0.0-preview.3-nanoserver-1903, 5.0-nanoserver-1903, 5.0.0-preview.3, 5.0 | [Dockerfile](https://github.com/dotnet/dotnet-docker/blob/master/5.0/aspnet/nanoserver-1903/amd64/Dockerfile)

## Windows Server 2019 amd64 Tags
##### .NET 5.0 Preview Tags
Tag | Dockerfile
---------| ---------------
5.0.0-preview.3-nanoserver-1809, 5.0-nanoserver-1809, 5.0.0-preview.3, 5.0 | [Dockerfile](https://github.com/dotnet/dotnet-docker/blob/master/5.0/aspnet/nanoserver-1809/amd64/Dockerfile)

You can retrieve a list of all available tags for dotnet/aspnet at https://mcr.microsoft.com/v2/dotnet/aspnet/tags/list.

# Support

See [Microsoft Support for .NET](https://github.com/dotnet/core/blob/master/microsoft-support.md) for the support lifecycle.

# Image Update Policy

* We update the supported .NET images within 12 hours of any updates to their base images (e.g. debian:buster-slim, windows/nanoserver:1909, buildpack-deps:bionic-scm, etc.).
* We publish .NET images as part of releasing new versions of .NET including major/minor and servicing.

# Feedback

* [File a .NET Docker issue](https://github.com/dotnet/dotnet-docker/issues)
* [File a .NET issue](https://github.com/dotnet/core/issues)
* [File an ASP.NET Core issue](https://github.com/aspnet/home/issues)
* [File an issue for other .NET components](https://github.com/dotnet/core/blob/master/Documentation/core-repos.md)
* [File a Visual Studio Docker Tools issue](https://github.com/microsoft/dockertools/issues)
* [File a Microsoft Container Registry (MCR) issue](https://github.com/microsoft/containerregistry/issues)
* [Ask on Stack Overflow](https://stackoverflow.com/questions/tagged/.net-core)
* [Contact Microsoft Support](https://support.microsoft.com/contactus/)

# License

* [.NET license](https://github.com/dotnet/dotnet-docker/blob/master/LICENSE)
* [Discover licensing for Linux image contents](https://github.com/dotnet/dotnet-docker/blob/master/documentation/image-artifact-details.md)
* [Windows Nano Server license](https://hub.docker.com/_/microsoft-windows-nanoserver/) (only applies to Windows containers)
* [Pricing and licensing for Windows Server 2019](https://www.microsoft.com/cloud-platform/windows-server-pricing)