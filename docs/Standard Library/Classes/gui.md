# GUI

[//]: # (See [Adding a Custom GUI]&#40;gui.md&#41; for more details.)

## getInventory() -> [Inventory](inventory.md) {data-toc-label='getInventory'}

Returns the inventory of the GUI.

## setInventory(inventory: [Inventory](inventory.md)) -> [Null](null.md) {data-toc-label='setInventory'}

Sets the contents of the GUI to be `inventory`.

## getTitle() -> [String](string.md) {data-toc-label='getTitle'}

Returns the title of the GUI.

## onSlotClick(slot: [Integer](integer.md), button: [Integer](integer.md), gui: [GUI](gui.md), player: [PlayerEntity](playerentity.md)) -> [Boolean](boolean.md) {data-toc-label='onSlotClick'}

This method is called when a user clicks a slot. This method is meant to be overridden.

## onClose(player: [PlayerEntity](playerentity.md), gui: [GUI](gui.md)) -> [Null](null.md) {data-toc-label='onClose'}

This method is called when the user closes the GUI. This method is meant to be overridden.
