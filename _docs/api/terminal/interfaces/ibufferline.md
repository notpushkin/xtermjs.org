---
title: IBufferLine
category: API-interfaces
layout: docs
---


# Interface: IBufferLine

## Hierarchy

* **IBufferLine**

## Index

### Properties

* [isWrapped]({% link _docs/api/terminal/interfaces/ibufferline.md %}#iswrapped)
* [length]({% link _docs/api/terminal/interfaces/ibufferline.md %}#length)

### Methods

* [getCell]({% link _docs/api/terminal/interfaces/ibufferline.md %}#getcell)
* [translateToString]({% link _docs/api/terminal/interfaces/ibufferline.md %}#translatetostring)

## Properties

###  isWrapped

• **isWrapped**: *boolean*

*Defined in [xterm.d.ts:1349](https://github.com/xtermjs/xterm.js/blob/5.0.0/typings/xterm.d.ts#L1349)*

___

###  length

• **length**: *number*

*Defined in [xterm.d.ts:1357](https://github.com/xtermjs/xterm.js/blob/5.0.0/typings/xterm.d.ts#L1357)*

## Methods

###  getCell

▸ **getCell**(`x`: number, `cell?`: [IBufferCell]({% link _docs/api/terminal/interfaces/ibuffercell.md %})): *[IBufferCell]({% link _docs/api/terminal/interfaces/ibuffercell.md %}) | undefined*

*Defined in [xterm.d.ts:1371](https://github.com/xtermjs/xterm.js/blob/5.0.0/typings/xterm.d.ts#L1371)*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`x` | number | The character index to get. |
`cell?` | [IBufferCell]({% link _docs/api/terminal/interfaces/ibuffercell.md %}) | Optional cell object to load data into for performance reasons. This is mainly useful when every cell in the buffer is being looped over to avoid creating new objects for every cell.  |

**Returns:** *[IBufferCell]({% link _docs/api/terminal/interfaces/ibuffercell.md %}) | undefined*

___

###  translateToString

▸ **translateToString**(`trimRight?`: boolean, `startColumn?`: number, `endColumn?`: number): *string*

*Defined in [xterm.d.ts:1381](https://github.com/xtermjs/xterm.js/blob/5.0.0/typings/xterm.d.ts#L1381)*

**Parameters:**

Name | Type | Description |
------ | ------ | ------ |
`trimRight?` | boolean | Whether to trim any whitespace at the right of the line. |
`startColumn?` | number | The column to start from (inclusive). |
`endColumn?` | number | The column to end at (exclusive).  |

**Returns:** *string*
