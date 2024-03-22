# File Editor Extension for z/OS<a id="ds-editor-extension-for-zos"></a>

## Table of contents<a id="table-of-contents"></a>
- [File Editor Extension for z/OS](#file-editor-extension-for-zos)
	- [Table of contents](#table-of-contents)
	- [Introduction](#introduction)
	- [Use cases](#use-cases)
		- [Open an editor](#open-an-editor)
		- [Change from text to table mode](#change-from-text-to-table-mode)
		- [Change from table to text mode](#change-from-table-to-text-mode)
		- [Use editor with vsam files](#use-editor-with-vsam-files)
	- [Links](#links)


## Introduction<a id="introduction"></a>

**File Editor Extension for z/OS. It's an extension for Visual Studio Code that provides full support to EBCDIC encoding.**

This extension has been designed to help developers manipulate z/OS environment files for those teams that have adopted the open source software for z/OS development and DevOps under IBM Z platform. The extension provides hexadecimal peek and EBCDIC text support. In addition, it allows loading Copybooks (Layouts) from local or MVS hosted files with the help of [Zowe Explorer](vscode:extension/zowe.vscode-extension-for-zowe).

Sequential datasets are downloaded to the local file system if accessed through [Zowe Explorer](vscode:extension/zowe.vscode-extension-for-zowe). These files can be synchronized manually.

VSAM files require installing NEORIS' VSAM API in your mainframe. This API allows a granullar and precise control with improved performance.

## Use cases<a id="use-cases"></a>

### Open an editor<a id="open-an-editor"></a>

![gif featuring opening the editor](./assets/openEditor.gif)

Prerequisite: Having the dataset file at hand.

1. Open the dataset file
   1. Select "Open Anyway"
   2. Choose NEORIS File Editor

### Change from text to table mode<a id="change-from-text-to-table-mode"></a>

![gif featuring change to table from text mode](./assets/LoadTableWays.gif)

Prerequisite: Having a dataset file opened and a copybook or json at hand.

1. Click "Manage" under definition
2. Click "Load Copybook" or "Load from json"
3. Select the copybook layout or json file

### Change from table to text mode<a id="change-from-table-to-text-mode"></a>

![gif featuring change to text from table mode](./assets/LoadTextWays.gif)

Prerequisite: Having a  a copybook or json file opened and a  at hand.

1. Click "Manage" under definition
2. Click "Unload"

### Use editor with vsam files<a id="use-editor-with-vsam-files"></a>
![gif featuring read vsam file in table mode](./assets/openZoweVsamDSFile.gif)

Support with VSAM
Prerequisite: Having Neoris-vsamapi and IBM rseapi installed in mainframe and zowe explorer extension in vscode.

## Links<a id="links"></a>

You can find more specific information in the following documents.

- [Text Mode functionality](./text_mode.md)
- [Table Mode functionality](./table_mode.md)
- [Zowe Explorer functionality](./zowe_explorer.md)
- [VsamApi functionality](./vsamapi.md)
