---
title: Welcome to HandyControl
---

HandyControl is a WPF control library that rewrites almost all native styles and includes more than 70 custom controls (increasingly).

# Requirements

![dotnet-require](https://img.shields.io/badge/.net-%3E%3D4.0-blue.svg) ![os-require](https://img.shields.io/badge/OS-%3E%3Dwin7-brightgreen) ![IDE-require](https://img.shields.io/badge/IDE-vs2019-blue.svg) ![csharp-require](https://img.shields.io/badge/C%23-8.0-blue.svg)

# Download

## Nuget

Nuget is a compiled release : [HandyControl-Nuget](https://www.nuget.org/packages/HandyControl/)

{% note info %}
There is a custom version : [HandyControls-Nuget](https://www.nuget.org/packages/HandyControls/)
{% endnote %}

{% note warning %}
Nuget are generally released at least once a month, so there is a high probability that this document will differ from this document. Any discrepancies are subject to this document.
{% endnote %}

## Github

The latest source code on Github is: [HandyControl-Github](https://github.com/HandyOrg/HandyControl)

{% note info %}
There is a custom version : [HandyControls-Github](https://github.com/ghost1372/HandyControls)
{% endnote %}

{% note warning %}
Github is generally updated every day and is relatively unsuitable for production.
{% endnote %}

{% note warning %}
The update speed of the document must not keep up with the latest Github source code. There are places where the entry and exit are based on the Demo example on Github.
{% endnote %}

# Project Structure Introduction

## the whole frame

After cloning the source code from Github, go to the src folder. The folder structure is as follows:
![Project_Structure](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/Project_Structure.png)

There are 4 solutions sln files here.

`Net_GE45` means that the .Net version is greater than or equal to 4.5.

The `Shared` folder is used to store the code of the shared project.

The five folders in the figure each contain two subfolders, for example, two shared subfolders in Shared:
![Sub_Folder_Structure](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/Sub_Folder_Structure.png)

They store the source code of the control and the sample source of the control.

## Source structure

We use HandyControl.sln as an example to illustrate, use VS2019 to open the solution:
![Net_GE45_Structure](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/Net_GE45_Structure.png)

If you want to start the example and see the effect of the control, please use HandyControlDemo_[specified item type] as the startup item.

As shown in the figure, HandyControlDemo_Net_GE45 has been used as the startup item.

Most of the public source code is in the Shared folder, and some of the code that needs to be customized for a particular project type is proposed to be placed in its own folder.

The HandyControl source code (mainly in HandyControl_Shared) mainly contains 7 folders, and their descriptions are as follows:

| Name | Use |
|-|-|
| Controls | Background interaction logic with all controls |
| Data | Basic data definitions required by the control library |
| Expression | Extracted from Microsoft.Expression.Drawing |
| Interactivity | Extracted from Microsoft.Expression.Interactions & System.Windows.Interactivity and made some modifications |
| Properties | Contains control library properties and language packs |
| Themes | Contains all xaml definitions for the control library |
| Tools | Mainly contains the help methods and extension methods required by the control library |

{% note info %}
Each control in Controls can generally find the corresponding xaml definition in Themes.
{% endnote %}

# Compile source code

{% note warning %}
Please confirm that your development environment meets the requirements before compiling.
{% endnote %}

Open HandyControl.sln and select the specified environment to compile in the Solution Configuration drop-down box:
![Build_Config](https://raw.githubusercontent.com/HandyOrg/HandyOrgResource/master/HandyControl/Doc/Build_Config.png)

## Compile source code with Powershell

go to Build folder and open Powershell here, then execute this command

{% code %}
.\build.ps1
{% endcode %}