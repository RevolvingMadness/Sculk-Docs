# Events

Events are listeners for things to happen in the world and call a function when they do.

## Place Block Event

Occurs when a living entity places a block.

This event is not cancellable.

```java
/*
`entity` is of type `LivingEntity`.
`block` is of type `Block`.
*/

events.onPlaceBlock(function(entity, block) {});
```

## Player Attack Entity Event

Occurs when a player attacks an entity.

This event is cancellable.

```java
/*
`player` is of type `PlayerEntity`.
`target` is of type `Entity`.
`weapon` is of type `ItemStack`.
*/

events.onPlayerAttackEntity(function(player, target, weapon) {});
```

## Player Break Block Event

Occurs when a player breaks a block.

This event is cancellable.

```java
/*
`player` is of type `PlayerEntity`.
`block_broken` is of type `Block`.
*/

events.onPlayerBreakBlock(function(player, pos, block_broken) {});
```

## Player Craft Item Event

Occurs when a player crafts an item.

This event is not cancellable.

```java
/*
`player` is of type `PlayerEntity`.
`item_crafted` is of type `ItemStack`.
*/

events.onPlayerCraftItem(function(player, item_crafted) {});
```

## Player Drop Item Event

Occurs when a player drops an item.

This event is not cancellable.

```java
/*
`player` is of type `PlayerEntity`.
`item_dropped` is of type `ItemStack`.
*/

events.onPlayerDropItem(function(player, item_dropped) {});
```

## Player Jump Event

Occurs when a player jumps.

This event is not cancellable.

```java
/*
`player` is of type `PlayerEntity`.
*/

events.onPlayerJump(function(player) {});
```

## Player Pickup Item Event

Occurs when a player picks up an item.

This event is cancellable.

```java
/*
`player` is of type `PlayerEntity`.
`item_picked_up` is of type `ItemStack`.
*/

events.onPlayerPickupItem(function(player, item_picked_up) {});
```

## Entity Sleep Event

Occurs when an entity sleeps.

This event is not cancellable.

```java
/*
`entity` is of type `LivingEntity`.
*/

events.onEntitySleep(function(entity) {});
```

## Player Use Item Event

Occurs when a player uses an item.

This event is cancellable.

```java
/*
`player` is of type `LivingEntity`.
`item_used` is of type `ItemStack
 */

events.onPlayerUseItem(function(player, item_used) {});
```

## Player Ring Bell Event

Occurs when a player rings a bell.

This event is cancellable.

```java
/*
`player` is of type `PlayerEntity`.
 */

events.onPlayerRingBell(function(player) {});
```

## Send Chat Message Event

Occurs when a player sends a message in chat.

This event is cancellable.

```java
/*
`player` is of type `ServerPlayerEntity`.
`message` is of type `String`.
 */

events.onPlayerSendChatMessage(function(player, message) {});
```

## Player Sneak Event

Occurs when a player is sneaking.

This event is not cancellable.

```java
/*
`player` is of type `ServerPlayerEntity`.
 */

events.onPlayerSneak(function(player) {});
```
