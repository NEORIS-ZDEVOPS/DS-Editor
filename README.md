# File Editor Extension for z/OS

**File Editor Extension for z/OS. It's an extension for Visual Studio Code that provides full support to EBCDIC encoding.**

Now supports VSAM! Check [our github page](https://github.com/NEORIS-ZDEVOPS/DS-Editor/tree/master/doc/vsamapi.md) for more details.

This extension has been designed to help developers manipulate z/OS environment files for those teams that have adopted the open source software for z/OS development and DevOps under IBM Z platform. The extension provides hexadecimal peek and EBCDIC text support. In addition, it allows loading Copybooks (Layouts) from local or MVS hosted files with the help of [Zowe Explorer](vscode:extension/zowe.vscode-extension-for-zowe).

Sequential datasets are downloaded to the local file system if accessed through [Zowe Explorer](vscode:extension/zowe.vscode-extension-for-zowe). These files can be synchronized manually.

VSAM files require installing NEORIS' VSAM API in your mainframe. This API allows a granullar and precise control with improved performance.

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