# Events

Events are listeners for things to happen in the world and call a function when they do.

## Place Block Event

Occurs when a living entity places a block.

This event is not cancellable.

```java
Events.onPlaceBlock(function(entity: LivingEntity, block: Block) -> Null {
    
});
```

## Attack Entity Event

Occurs when a player attacks an entity.

This event is cancellable.

```java
Events.onAttackEntity(function(player: PlayerEntity, target: Entity, weapon: ItemStack) -> Boolean {
    return true;
});
```

## Break Block Event

Occurs when a player breaks a block.

This event is cancellable.

```java
Events.onBreakBlock(function(player: PlayerEntity, pos: BlockPos, block_broken: Block) -> Boolean {
    return true;
});
```

## Craft Item Event

Occurs when a player crafts an item.

This event is not cancellable.

```java
Events.onCraftItem(function(player: PlayerEntity, item_crafted: ItemStack) -> Null {
    
});
```

## Drop Item Event

Occurs when a player drops an item.

This event is not cancellable.

```java
Events.onDropItem(function(player: PlayerEntity, item_dropped: ItemStack) -> Null {
    
});
```

## Jump Event

Occurs when a player jumps.

This event is not cancellable.

```java
Events.onJump(function(player: PlayerEntity) -> Null {
    
});
```

## Pickup Item Event

Occurs when a player picks up an item.

This event is cancellable.

```java
Events.onPickupItem(function(player: PlayerEntity, item_picked_up: ItemStack) -> Boolean {
    return true;
});
```

## Entity Sleep Event

Occurs when an entity sleeps.

This event is not cancellable.

```java
Events.onEntitySleep(function(entity: LivingEntity) -> Null {
    
});
```

## Right Click Item Event

Occurs when a player uses an item.

This event is cancellable.

```java
Events.onRightClickItem(function(player: PlayerEntity, item_used: ItemStack) -> Boolean {
    return true;
});
```

## Ring Bell Event

Occurs when a player rings a bell.

This event is cancellable.

```java
Events.onRingBell(function(player: PlayerEntity) -> Boolean {
    return true;
});
```

## Send Chat Message Event

Occurs when a player sends a message in chat.

This event is cancellable.

```java
Events.onSendChatMessage(function(player: ServerPlayerEntity, message: String) -> Boolean {
    return true;
});
```

## While Sneaking Event

Occurs when a player is sneaking.

This event is not cancellable.

```java
Events.whileSneaking(function(player: ServerPlayerEntity) -> Null {
    
});
```
