![GitHub forks](https://img.shields.io/github/forks/demaconsulting/VSWhereTool?style=plastic)
![GitHub Repo stars](https://img.shields.io/github/stars/demaconsulting/VSWhereTool?style=plastic)
![GitHub contributors](https://img.shields.io/github/contributors/demaconsulting/VSWhereTool?style=plastic)
![GitHub](https://img.shields.io/github/license/demaconsulting/VSWhereTool?style=plastic)

# About

VSWhereTool is a repackaging of the [vswhere](https://github.com/microsoft/vswhere) utility as a [Dotnet tool](https://learn.microsoft.com/en-us/dotnet/core/tools/global-tools).

VSWhere is already available in numerous formats for [installation](https://github.com/microsoft/vswhere/wiki/Installing).
Packaging it as a Dotnet tool allows for multiple versions to be installed and cached on a system
simultaneously, and users can control which version is used through a
[Dotnet tool manifest file](https://learn.microsoft.com/en-us/dotnet/core/tools/global-tools#install-a-local-tool).


# Installation & Usage

The following will add VSWhereTool to a Dotnet tool manifest file:

```
dotnet new tool-manifest # if you are setting up this repo
dotnet tool install --local DemaConsulting.VSWhereTool
```

The tool can then be executed by:

```
dotnet vswhere <arguments>
```
