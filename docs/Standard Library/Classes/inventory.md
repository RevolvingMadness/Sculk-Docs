# Inventory

Represents an entity's inventory.

## contains(item: [Item](item.md)) -> [Boolean](boolean.md) {data-toc-label='contains'}

Returns whether the item is in the inventory.

## count(item: [Item](item.md)) -> [Integer](integer.md) {data-toc-label='count'}

Returns how many of `item` is in the inventory.

## getStack(slot: [Integer](integer.md)) -> [ItemStack](itemstack.md) {data-toc-label='getStack'}

Returns the stack in the slot `slot`.

## isEmpty() -> [Boolean](boolean.md) {data-toc-label='isEmpty'}

Returns whether the inventory is empty.

## removeStack(stack: [ItemStack](itemstack.md)) -> [Null](null.md) {data-toc-label='removeStack'}

Removes `stack` from the inventory.

## setStack(slot: [Integer](integer.md), stack: [ItemStack](itemstack.md)) -> [Null](null.md) {data-toc-label='setStack'}

Sets the stack at slot `slot` to the stack `stack`.
