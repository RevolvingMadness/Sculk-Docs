# ItemStack

Represents a stack of items.

## item: [Item](item.md) {data-toc-label='item'}

The item in the stack.

## init(item: [Item](item.md), count: [Integer](integer.md)) -> [ItemStack](itemstack.md) {data-toc-label='init'}

Initializes ItemStack.

## decrement(amount: [Integer](integer.md)) -> [Null](null.md) {data-toc-label='decrement'}

Decrements the amount of items in the stack by `amount`.

## getCount() -> [Integer](integer.md) {data-toc-label='getCount'}

Returns the amount of items in the stack.

## getDamage() -> [Integer](integer.md) {data-toc-label='getDamage'}

Returns how the damage (lost durability) of the item stack.

Does **NOT** return how much damage the item does!

## getHolder() -> [Entity](entity.md) {data-toc-label='getHolder'}

Returns the entity who is holding the item.

## getItem() -> [Item](item.md) {data-toc-label='getItem'}

Returns the item in the stack.

## getMaxCount() -> [Integer](integer.md) {data-toc-label='getMaxCount'}

Returns the max amount of items that can be in 1 stack.

## getMaxDamage() -> [Integer](integer.md) {data-toc-label='getMaxDamage'}

Returns the durability of the item.

## getName() -> [String](string.md) {data-toc-label='getName'}

Returns the name of the item.

## getRepairCost() -> [Integer](integer.md) {data-toc-label='getRepairCost'}

Returns the repair cost of the item.

## hasEnchantments() -> [Boolean](boolean.md) {data-toc-label='hasEnchantments'}

Returns whether the item has enchantments.

## increment(amount: [Integer](integer.md)) -> [Null](null.md) {data-toc-label='increment'}

Increments the amount of items in the stack by `amount`.

## isDamageable() -> [Boolean](boolean.md) {data-toc-label='isDamageable'}

Returns whether the item is damageable.

## isDamaged() -> [Boolean](boolean.md) {data-toc-label='isDamaged'}

Returns whether the item is damaged.

## isEnchantable() -> [Boolean](boolean.md) {data-toc-label='isEnchantable'}

Returns whether the item is enchantable.

## isFood() -> [Boolean](boolean.md) {data-toc-label='isFood'}

Returns whether the item is food.

## isInFrame() -> [Boolean](boolean.md) {data-toc-label='isInFrame'}

Returns whether the item is in a frame.

## isStackable() -> [Boolean](boolean.md) {data-toc-label='isStackable'}

Returns whether the item is stackable.

## setCount(amount: [Integer](integer.md)) -> [Null](null.md) {data-toc-label='setCount'}

Sets the amount of items in the stack to `amount`.

## setDamage(damage: [Integer](integer.md)) -> [Null](null.md) {data-toc-label='setDamage'}

Sets the damage (lost durability) of the item.

## setRepairCost(repair_cost: [Integer](integer.md)) -> [Null](null.md) {data-toc-label='setRepairCost'}

Sets the repair cost of the item.
