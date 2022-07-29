---
layout: page
title: IntelIJ IDEA
---
This page contains information about developing the OpenDA Java source code using [IntelliJ IDEA](https://en.wikipedia.org/wiki/IntelliJ_IDEA).
A free community version can be downloaded from the [JetBrains website](https://www.jetbrains.com/idea/download/).
By opening the project file`openda.ipr` in the main folder `<path_to_openda_source>`, most of the settings for this project will be set correctly.

In order to use the Java Development Kit in IntelliJ, you can refer to it via `File -> Project Structure -> Platform Settings -> SDKs`.

To build the source code into usable binaries, [Ant](https://en.wikipedia.org/wiki/Apache_Ant) is used which is already present in recent versions of IntelliJ. The Ant sidebar can be opened by heading to `View -> Tool Windows -> Ant`.

By selecting the `<path_to_openda_source>/build.xml` in the Ant plugin, a list of build targets can be run. Common practice is to run the `build-x64` target in this list by selecting it and choosing `Run Target`. By running it, the OpenDA binaries will be generated in `bin`. These binaries can be used to run OpenDA by non-developer users outside of IntelliJ.

If one of the XML schema files (`.xsd`) has changed, then it is necessary to run the [Castor framework](https://en.wikipedia.org/wiki/Castor_(framework)) to convert XML files to Java source code. More information about these configuration files can be found in the [introduction to OpenDA](https://openda-association.github.io/wiki/introduction_openda). Castor is run by selecting the corresponding `build_castor.xml` target in the Ant plugin (see, for example, `core/build_castor.xml`), and then executing it by choosing `Run Target`.

