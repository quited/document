# How-to: setting up development environment of UWE and its sub projects

### Overview

The environment  is consist of  several parts:

+ VCS Tool
+ IDE
+ Toolchains
+ Project Generating Tool
+ Documenting Tool
+ Flashing Tool

We assume that you use **Windows10** as the develop platform, and if you use Linux or MacOS , the installation process should be almost the same using package manager, and you may need to fix some dependences problems of the tools.



### VCS Tool

UWE and its sub projects use **Git** as the VCS tool and are currently being hosted on **GitHub** .

To apply operations on these projects, **Git for Windows** must be installed, then you can use **Git Bash** or **Git GUI** to manage projects.



### IDE

Aiming at doing everything at the same place, we suggest to use **JetBrains CLion** as an IDE (currently at version 2019.1.4).

The **CLion** version must be higher than 2019. 1 EAP，to support build-in embedded development plug-ins.



### Toolchains

Here we need two kinds of toolchains:  **MinGW** for CLion and **gnu-non-eabi** for cross compilation support.

When finished installing CLion and Toolchains, you may need to check if they have been automatically detected  by CLion, if not, you have to set path to them manually.



### Project Generating Tool

To create embedded projects automatically, we use **STM32CubeMX** to Generate projects that can be loaded into CLion.



### Documenting Tool

We use Typora to create Markdown files, temporarily.



### UML Tool

For compatibility with VCS systems, we use PlantUML to generate visual UML map from plain text.

To edit these **.plantuml** files, we use **VSCode** with these following two plug-ins:

+ **PlantUML v2.11.2**
+ **Yog PlantUML Highlight v0.0.5**

And **Graphviz** is needed in the visual map generation, **v2.38** had been tested.



### Flashing Tool

To work with CLion, we use **OpenOCD** as flashing and debugging tool.
