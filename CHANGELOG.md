# Change Log

All notable changes to the File Editor extension for z/OS will be documented in this file.

## [2.2.1] 2024-11-11
- Extended support for zowe 3.0

## [2.2.0] 2024-10-30
- Added text decodification selection functionality
- Improved UI when editing rows in server stream mode
- Fixed more bugs with copybooks with OCCURS and REDEFINES
- Expanded capabilities with API VSAM API
- Changed how the application interacts with zowe explorer profiles
- Fixed some issues with VSAM state control
- Fixed bug when fetching datasets with multiple ZOWE profiles configured in ZOWE explorer

## [2.1.0] 2024-04-12
- Added partial support for COMP-1, COMP-2, NATIONAL, and type aliases
- Removed extra tables when redefines are present.
- Fixed multiple bugs regarding copybooks with OCCURS
- Fixed collapse menu not opening in place bug
- Fixed multiple search bugs and updated documentation

## [2.0.1] 2024-03-26
- Changed texts
- Fixed bug when parsing copybook with REDEFINE inside OCCURS
- Fixed bug when parsing copybook with a REDEFINE group

## [2.0.0] 2024-03-22
- Added VSAM support! Check the documentation for more information.
- Added search
- Added capabilities to hide and show columns
- Changed icon

## [1.4.1] 2023-08-04

- Fixed being unable to write into symbol and usymbol columns (yellow ones)
- Fixed negative numbers being turned positive on edition
- Changed how profiles are stored

## [1.4.0] 2023-07-26

- Added support for RSE API
- Added support for editing data in text view
- Added commands to manage zowe profiles
- Added configuration for managing zowe profiles

## [1.3.1]

- Updated readme with gifs
- Added repository to raise questions and issues

## [1.3.0]

- Added status icon
- Now you can upload and download to a mainframe directly from the editor
- Added goto page functionality

## [1.2.1]

- Now row size for variable type datasets will be calculated as (registered lrecl)-4
- A notification will inform when a dataset has started it's download.

## [1.2.0]

- Added context menu with more capabilities of row manipulation (reset values, copy row, paste row...)

## [1.1.0]

- Now addding and removing rows is possible

## [1.0.2]

- Readme changes and better documentation

## [1.0.0] [1.0.1]

- Published extension