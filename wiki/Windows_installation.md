---
layout: page
title: OpenDA installation on a Windows platform
---

With the following instructions, the OpenDA software can be installed on a Windows machine: 

* Ensure that a 64-bit Java version 1.8 or higher is installed on your computer. You can check which version is installed through the `java -version` command in a terminal or command window. The latest open-source version of Java is included in [Amazon Corretto](https://aws.amazon.com/corretto).
* Download the [OpenDA binaries](https://github.com/OpenDA-Association/OpenDA/releases).
* Extract the OpenDA distribution file to the desired location on your computer. Note: OpenDA does not work when it is installed on a location with a space in the path (like "`My Documents`").
* Open the OpenDA GUI: 
    * Open a command prompt by pressing the Windows button and typing `cmd` in the search box;
    * Head to the folder `<path_to_openda_release>/bin`;
    * Run `oda_run_gui.bat`
* Try to run an example. You can find examples in the `<path_to_openda_release>/examples` directory. An example that can easily be executed is found in `model_example_blackbox/blackbox_example_calibration/Dud.oda`. After opening this file in the GUI, you can run the simulation. For the examples `model_dflowfm_blackbox` and `model_delft3d` in this folder, it is necessary to connect to existing models. 
