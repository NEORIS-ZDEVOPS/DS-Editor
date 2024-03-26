# Text mode documentation
## Table of contents
- [Text mode documentation](#text-mode-documentation)
	- [Table of contents](#table-of-contents)
	- [Introduction](#introduction)
	- [Use cases](#use-cases)
		- [Open a file](#open-a-file)
		- [Change Row Size](#change-row-size)
		- [Change Rows per page](#change-rows-per-page)
		- [Navigate to Another Page](#navigate-to-another-page)
		- [Make a selection with mouse](#make-a-selection-with-mouse)
		- [Make a selection with keyboard](#make-a-selection-with-keyboard)
			- [Simple selection](#simple-selection)
			- [Word selection](#word-selection)
			- [Multiple selection](#multiple-selection)
			- [Row selection](#row-selection)
			- [All selection](#all-selection)
		- [Peek at the underlying hexadecimal](#peek-at-the-underlying-hexadecimal)
		- [Undo](#undo)
		- [Redo](#redo)
		- [Copy text](#copy-text)
		- [Paste text](#paste-text)
		- [Edit segment](#edit-segment)
		- [Clone row](#clone-row)
		- [Append empty row](#append-empty-row)
		- [Insert empty row](#insert-empty-row)
		- [Delete this row](#delete-this-row)
		- [Search](#search)
			- [Advanced search](#advanced-search)

## Introduction
 The text mode provides fully hexadecimal integration and EBCDIC support for sequential data sets.

## Use cases

### Open a file

![gif featuring opening the editor](./assets/openEditor.gif)

1. Open the dataset file
   1. Select "Open Anyway"
   2. Choose "z/OS File Editor"

### Change Row Size

![gif featuring change row size in text editor](./assets/ChangeRows.gif)

1. Click "Open Settings" under Others
2. Manually adjust the "Row size" , or use the side buttons.
3. Press Enter to apply changes.

### Change Rows per page

![gif featuring change rows per page in text editor](./assets/ChangeRowsPerPage.gif)

1. Click "Open Settings" under Others
2. Manually adjust the "Rows per page" , or use the side buttons.
3. Press Enter to apply changes.
### Navigate to Another Page

![gif featuring navigation page in text editor](./assets/ChangePage.gif)

Prerequisite: If the selected number of rows per page is smaller than the number of rows, pagination will be activated, showing page 1 of total numer of pages.

1. Click on the right-arrow icon to move to the next page.
2. Click on the left-arrow icon to move to the previous page.
3. Click on the arrow with the 'enter' symbol and input a number within the page range to go directly to that page.

### Make a selection with mouse

![gif featuring selection with mouse in text editor](./assets/SelectionMouse.gif)

1. Press and hold on the text to expand the selection.

### Make a selection with keyboard

Prerequisite: Place the mouse cursor over the text to give it focus.

#### Simple selection

![gif featuring selection simple with keyboard in text editor](./assets/SelectionKeySimple.gif)

1. Press any arrow key on the text to create a basic selection, and move the selection in the direction of the arrow key.
#### Word selection

![gif featuring selection word with keyboard in text editor](./assets/CtrlSelectionUpdate.gif)

Note: Only combinations of numbers and letters are considered words.

1. Press left or right key plus ctrl key to move over the words.

#### Multiple selection

![gif featuring selection multiple with keyboard in text editor](./assets/ShiftSelectionUpdate.gif)

1. Press arrow keys plus shift key to make a multiple selection that grows when the combination is held down

#### Row selection

![gif featuring selection row with keyboard in text editor](./assets/SelectLine.gif)

1. Right-click on any row, and the entire row will be selected.

#### All selection

![gif featuring selection all with keyboard in text editor](./assets/AllSelectionUpdate.gif)

Prerequisite: Focus on the text

1. Press ctrl + a, and the entire text will be selected, spanning all pages

### Peek at the underlying hexadecimal

![gif featuring peek  at the underlying hexadecimal  in text editor](./assets/PeekEyeDs.gif)

Prerequisite: Having a dataset file opened, no copybook loaded.

1. Click the eye icon at the left of the lines.
2. Press the space bar on the row where a selection is active; the corresponding row will be highlighted with an eye icon

### Undo

![gif featuring undo  in text editor](./assets/UndoUpdate.gif)

1. Press ctrl+z to undo the last action

### Redo

![gif featuring redo  in text editor](./assets/RedoUpdate.gif)

1. Press ctrl+y to redo the last action

### Copy text

![gif featuring copy  in text editor](./assets/CopyUpdate.gif)

Prerequisite: Having a selection made

1. Made a selection and press ctrl+c or right button and select the option copy text

### Paste text

![gif featuring paste  in text editor](./assets/PasteUpdate.gif)

Prerequisite: Ensure there is content on the clipboard

1. Press ctrl+v or right button to paste the content from the clipboard where the selection is located

### Edit segment

![gif featuring edit  in text editor](./assets/EditUpdate.gif)

Prerequisite:Having a selection made

1. Over the selection press the right button and press the edit segment option.
2. In the contextual menu, in the "Text" field delete the original selection and introduce the new one.
3. Pressing the Enter key will apply the changes, then press the "Confirm" button

### Clone row

![gif featuring clone row in text editor](./assets/CloneRow.gif)

1. Hover over any selection or simply right-click on any row, and then choose the "Clone this row" option.
2. Under the applied row, the clone will be added.

### Append empty row

![gif featuring append empty row in text editor](./assets/AppendEmptyRow.gif)

1. Right-click on any row, select "Append empty row," and an empty row will be added below the selected row

### Insert empty row

![gif featuring insert empty row in text editor](./assets/InsertEmptyRow.gif)

1. Right-click on any row, select "Insert empty row", and a empty row will be added above the selected row

### Delete this row

![gif featuring delete row in text editor](./assets/DeleteRow.gif)

1. Right-click on any row, select "Delete this row", and the selected row will be removed

### Search

![gif featuring search in text editor](./assets/SearchDataLines.gif)

1. Click on the search header input
2. Enter the string and click the search button(magnifying glass)
3. Navigate forward through the matches by clicking on the table and pressing the Tab key.
4. Navigate back through the matches by clicking on the table and pressing the Shift key.
5. Cancel the search mode by clicking the X button on the search header menu.

Notes: 
- If the search results contain multiple tables, to navigate between them you need to give focus by clicking on the one you want to move to.
- If the search results span multiple pages, we can still navigate through the resulting pages using the pagination menu buttons.
- If the search does not return any result, a warning message will be launched:"There are no matches".

#### Advanced search
The advanced search allows finding hexadecimal patterns with the addition of text.

![gif featuring advanced search in text editor](./assets/AdvancedTextSearch.gif)

1. Click on the advanced search button to enable advanced search ![advance button](./assets/AdvanceSearchButton.png)
2. An advance search icon will appear into the input box when the advanced search is enabled ![advance button](./assets/AdvanceSearchIcon.png)
3. Click the advanced search button or cancel search button to disable the advanced search.
3. Click on the search header input
4. Enter a valid pattern for advanced search (Search for valid patterns in the pattern section).
5. The rest of functionality is the same as normal search.

- Notes:
	- If the search string is normal text, it will work as normal search.
	- If the search does not return any result, a warning message will be launched:"There are no matches".

- Valid patterns:
	- To search in hexadecimal mode, use \x follow by the hexadecimal number(\xd9)
	- Every hexadecimal number must be preceded by the \x format.
	- Characters can be used with hexadecimal numbers too
	- Normal numbers can be used with hexadecimal numbers too
	- Valid examples:
		- \x96
		![advance search text mode 1](./assets/AdvanceTextSearch1.png)

		- \xc2a\xa3
		![advance search text mode 2](./assets/AdvanceTextSearch2.png)

		- M\x81n
		![advance search text mode 3](./assets/AdvanceTextSearch3.png)


		- \xe35
		![advance search text mode 4](./assets/AdvanceTextSearch4.png)


