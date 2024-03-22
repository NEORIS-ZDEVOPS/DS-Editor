# NEORIS File Editor Extension for z/OS

**NEORIS File Editor Extension for z/OS. It's an extension for Visual Studio Code that provide fully support to EBCDIC encoding for Sequential Data Sets.**

Now supports VSAM! Check [our github page](https://github.com/NEORIS-ZDEVOPS/DS-Editor/tree/master/doc) for more details.

This extension has been designed to help developers to manipulate  z/OS environment files, and for those teams have adopted the open source software for z/OS development and DevOps under IBM z platform. Provides fully hexadecimal integration and EBCDIC support for sequential data sets, allowing to load a Copybook (Layout) from your application repository or even the same MVS system (Using Zore Explore). The files are unload to the local system to increase the performance and can be sincronized with the z/OS system once the changes has completed.

## Features

- Read, Edit and Write EBCDIC (datasets) files
- Hexadecimal conversion
- Apply Layouts using Copybooks
  - Alpha-Numeric Supprot
  - Display Support
  - Binary Support
  - Comp-3 Support
- Zowe Explorer Compatibility

## Requirements

- To use the z/OS connection capabilities, it is required to have configured a ZOWE profile. A ZOWE profile, in turn, requires the mainframe to have "zosmf" or "rse api".
- For VSAM files, NEORIS's VSAM API has to be installed in the mainframe.

## Known Issues

For a list of known issues and to raise your own, visit [our github page](https://github.com/NEORIS-ZDEVOPS/DS-Editor/issues).

## How to use

Check the documentation in [our github page](https://github.com/NEORIS-ZDEVOPS/DS-Editor/tree/master/doc)