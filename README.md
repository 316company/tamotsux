# ⛔️ DEPRECATED

Please use [@sheetbase/tamotsux-server](https://github.com/sheetbase/tamotsux-server).

# TamotsuX

This is a modification version of original **Tomatsu** library, **supports multiple Spreadsheets**.

Tamotsu original repo: [https://github.com/itmammoth/Tamotsu](https://github.com/itmammoth/Tamotsu)

## Install

Library ID: ``19cYeZpDb9KiMV_fY5wNQjcPiwDMLDoxslulErvWctLI44AY0SExCWu5l``

Select latest version, set Indentifier to ``TamotsuX``.

## Usage

Pass a parammeter of **spreadsheet** (the Spreadsheet Object) when define table.

If **spreadsheet** param not defined, the Spreadsheet in ``Tamotsu.initialize([Spreadsheet])`` will be used.

```js
var mySpreadsheet = SpreadsheetApp.openById('1Jh316...');
var myOtherSpreadsheet = SpreadsheetApp.openById('1Pl413...');

Tamotsu.initialize(mySpreadsheet); // init and set 'mySpreadsheet' the default spreadsheet
var Agent = Tamotsu.Table.define({ sheetName: 'Agents', spreadsheet: mySpreadsheet });
var Flower = Tamotsu.Table.define({ sheetName: 'Flowers', spreadsheet: myOtherSpreadsheet });

var agent = Agent.first();
var flower = Flower.first();
    
```
