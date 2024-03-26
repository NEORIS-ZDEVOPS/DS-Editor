# VsamApi documentation <a id="documentation">

## Table of contents<a id="table-of-contents"></a>
- [VsamApi documentation ](#vsamapi-documentation-)
	- [Table of contents](#table-of-contents)
	- [Introduction](#introduction)
	- [Prerequisites ](#prerequisites-)
	- [Operating mode](#operating-mode)
	- [Use cases](#use-cases)
		- [Open a file](#open-a-file)
		- [Create a record](#create-a-record)
		- [Delete a record](#delete-a-record)
		- [Update a record](#update-a-record)
		- [Undo/Redo an action](#undoredo-an-action)
	- [Notes](#notes)

## Introduction<a id="introduction"></a>
NEORIS' VSAM API allows granullar CRUD (Create, Read, Update, Delete) operations with [KSDS VSAM](https://www.ibm.com/docs/en/zos/2.4.0?topic=types-key-sequenced-data-sets) files from capable clients. File Editor Extension for z/OS is such capable client.

We have plans to expand the API's functionality.

## Prerequisites <a id="prerequisites"></a>
To utilize the VSAM functionality, it is essential to have the NEORIS' VSAM API and IBM's RSE API set-up in the mainframe.

To learn how to set-up NEOSRIS' VSAM API, get in touch with us [zdevops@neoris.com](mailto:zdevops@neoris.com?subject=About%20setting%20up%20VSAM%20API&body=Greetings%2C%0A%0AI'm%20interested%20in%20setting%20up%20NEORIS's%20VSAM%20API%20in%20a%20z%2FOS%20mainframe.%20Can%20I%20get%20information%20about%20the%20process%3F%0A%0ARegards.%0A).

## Operating mode<a id="operating-mode"></a>
Is important to know that for every operation on the VSAM file(read, add, update and delete), the extension will make a request to the VSAM API.

## Use cases<a id="use-cases"></a>
Note: All the operations are explained in table mode (we encourage using this mode for VSAM files).

### Open a file<a id="open-a-file"></a>

![gif featuring open vsam file in table mode](./assets/openZoweVsamDSFile.gif)

1. Search the vsam file in zowe explorer in the Data Sets-> rse section
2. In the results, right-click on any of the three files associated with the VSAM file, and select "Open with z/OS File Editor."

### Create a record

![gif featuring creating vsam record in table mode](./assets/addRecord.gif)

1. Click on the plus button where no record exists.
2. Fill in the fields (Based on the data type of each field, we control the data that is filled).
3. Click "Confirm" button to add the record.

### Delete a record
![gif featuring delete vsam record in table mode](./assets/deleteRecord.gif)

1.Click on the "x" button on the record that you want to delete

### Update a record

![gif featuring update vsam record in table mode](./assets/updateRecord.gif)

1. Click in the field of the record to update.
2. Change the content and click the confirm button.

### Undo/Redo an action 

![gif featuring undo/redo an action in table mode](./assets/undoRedo.gif)

1. With the delete action(is the same for every action), push "Ctrl + Z" to undo the action and push "Ctrl + Y" to redo.

Note: As mentioned in the [Operating mode](#operating-mode) section, for every undo/redo action, it will make a request to the VSAM API.

## Notes 

All the previous functionality explained in the [table mode](./table_mode.md) and [text mode](./text_mode.md) are the same with Neoris vsam api