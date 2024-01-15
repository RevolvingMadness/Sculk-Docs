# Sculk's Standard Library

## BlockPos

Represents the position of a block in a three-dimensional volume.
Each coordinate is integer-valued.

| Argument Name | Type                | Description                   |
|---------------|---------------------|-------------------------------|
| `x`           | [Integer](#integer) | The x coordinate of the block |
| `y`           | [Integer](#integer) | The y coordinate of the block |
| `z`           | [Integer](#integer) | The z coordinate of the block |

## Blocks

A class that contains every modded and unmodded block.

### get(blockID: [Resource](#resource)) {data-toc-label='get'}

Gets the block from the given ID.

Arguments:

| Argument Name | Type                  | Description  |
|---------------|-----------------------|--------------|
| `blockID`     | [Resource](#resource) | The block ID |

## Block

Represents a block.

### asItem(): [Item](#Item) {data-toc-label='asItem'}

Returns the block in item form.

### getBlastResistance(): [Float](#float) {data-toc-label='getBlastResistance'}

Returns the blast resistance of the block.

### getName(): [String](#string) {data-toc-label='getName'}

Returns the name of the block.

### getSlipperiness(): [Float](#float) {data-toc-label='getSlipperiness'}

Returns the slipperiness of the block.

## Boolean

Represents a true or false value.

## CommandResult

Represents the result of running a command. (Returned from [MinecraftServer.runCommand()](#minecraftserver))

[](COME_BACK_TO_THIS)

### result: [Integer](#integer) | [Null](#null) {data-toc-label='result'}

The result of the command. If the command did not succeed the value will default to [Null](#null).

### succeeded: [Boolean](#boolean) {data-toc-label='succeeded'}

Whether the command succeeded.

### errorMessage: [String](#string) | [Null](#null) {data-toc-label='errorMessage'}

Whether the command succeeded. If the command succeeded the value will default to [Null](#null).

## Dictionary

Represents a dictionary.

## Entity

### addCommandTag(commandTag: [String](#string)): [Null](#null) {data-toc-label='addCommandTag'}

Adds a tag to the entity. Similar to `/tag add`

| Argument Name | Type              | Description                  |
|---------------|-------------------|------------------------------|
| `commandTag`  | [String](#string) | The tag to add to the entity |

### canFreeze(): [Boolean](#boolean) {data-toc-label='canFreeze'}

Returns whether the entity can freeze.

### canUsePortals(): [Boolean](#boolean) {data-toc-label='canUsePortals'}

Returns whether the entity can use portals.

### dismountVehicle(): [Null](#null) {data-toc-label='dismountVehicle'}

Dismounts the entity from any vehicle it's riding.

### extinguish(): [Null](#null) {data-toc-label='extinguish'}

Extinguishes the entity with no sound.

### extinguishWithSound(): [Null](#null) {data-toc-label='extinguishWithSound'}

Extinguishes the entity with sound.

### getBlockPos(): [BlockPos](#blockpos) {data-toc-label='getBlockPos'}

Returns the block pos of the entity.

### getBlockX(): [Integer](#integer) {data-toc-label='getBlockX'}

Returns the x coordinate of the entity.

### getBlockY(): [Integer](#integer) {data-toc-label='getBlockY'}

Returns the y coordinate of the entity.

### getBlockZ(): [Integer](#integer) {data-toc-label='getBlockZ'}

Returns the z coordinate of the entity.

### getCommandTags(): [List\[String\]](#list) {data-toc-label='getCommandTags'}

Returns the tags on the entity. Similar to `/tag list`.

### getName(): [String](#string) {data-toc-label='getName'}

Returns the name of the entity.

### getPassengers(): [List\[Entity\]](#list) {data-toc-label='getPassengers'}

Returns the passengers riding the entity.

### getVehicle(): [Entity](#entity) {data-toc-label='getVehicle'}

Returns the vehicle the entity is riding.

### getX(): [Float](#float) {data-toc-label='getX'}

Returns the x coordinate of the entity.

### getY(): [Float](#float) {data-toc-label='getY'}

Returns the y coordinate of the entity.

### getZ(): [Float](#float) {data-toc-label='getZ'}

Returns the z coordinate of the entity.

### hasControllingPassenger(): [Boolean](#boolean) {data-toc-label='hasControllingPassenger'}

Returns whether the passenger riding the entity is controlling.

### hasNoGravity(): [Boolean](#boolean) {data-toc-label='hasNoGravity'}

Returns whether the entity has no gravity.

### hasPassenger(passenger: [Entity](#entity)): [Boolean](#boolean) {data-toc-label='hasPassenger'}

Returns whether `passenger` is riding the entity.

| Argument Name | Type              | Description            |
|---------------|-------------------|------------------------|
| `passenger`   | [Entity](#entity) | The passenger to check |

### hasPassengers(): [Boolean](#boolean) {data-toc-label='hasPassengers'}

Returns whether the entity has passengers.

### hasVehicle(): [Boolean](#boolean) {data-toc-label='hasVehicle'}

Returns whether the entity is riding an entity.

### isCrawling(): [Boolean](#boolean) {data-toc-label='isCrawling'}

Returns whether the entity is crawling.

### isDescending(): [Boolean](#boolean) {data-toc-label='isDescending'}

Returns whether the entity is descending.

### isFireImmune(): [Boolean](#boolean) {data-toc-label='isFireImmune'}

Returns whether the entity is fire immune.

### isFrozen(): [Boolean](#boolean) {data-toc-label='isFrozen'}

Returns whether the entity is frozen.

### isGlowing(): [Boolean](#boolean) {data-toc-label='isGlowing'}

Returns whether the entity is glowing.

### isInFluid(): [Boolean](#boolean) {data-toc-label='isInFluid'}

Returns whether the entity is in a fluid.

### isInLava(): [Boolean](#boolean) {data-toc-label='isInLava'}

Returns whether the entity is in lava.

### isInsideWall(): [Boolean](#boolean) {data-toc-label='isInsideWall'}

Returns whether the entity is in inside a wall.

### isInvisible(): [Boolean](#boolean) {data-toc-label='isInvisible'}

Returns whether the entity is invisible.

### isInvulnerable(): [Boolean](#boolean) {data-toc-label='isInvulnerable'}

Returns whether the entity is invulnerable.

### isOnFire(): [Boolean](#boolean) {data-toc-label='isOnFire'}

Returns whether the entity is on fire.

### isOnGround(): [Boolean](#boolean) {data-toc-label='isOnGround'}

Returns whether the entity is on ground.

### isOnRail(): [Boolean](#boolean) {data-toc-label='isOnRail'}

Returns whether the entity is on a rail.

### isSilent(): [Boolean](#boolean) {data-toc-label='isSilent'}

Returns whether the entity is silent.

### isSneaking(): [Boolean](#boolean) {data-toc-label='isSneaking'}

Returns whether the entity is sneaking.

### isSprinting(): [Boolean](#boolean) {data-toc-label='isSprinting'}

Returns whether the entity is sprinting.

### isSwimming(): [Boolean](#boolean) {data-toc-label='isSwimming'}

Returns whether the entity is swimming.

### isTouchingWater(): [Boolean](#boolean) {data-toc-label='isTouchingWater'}

Returns whether the entity is touching water.

### isTouchingWaterOrRain(): [Boolean](#boolean) {data-toc-label='isTouchingWaterOrRain'}

Returns whether the entity is touching water or rain.

### isWet(): [Boolean](#boolean) {data-toc-label='isWet'}

Returns whether this entity is touching water, being rained on, or is inside a bubble column.

### kill(): [Null](#null) {data-toc-label='kill'}

Kills the entity.

### removeAllPassengers(): [Null](#null) {data-toc-label='removeAllPassengers'}

Dismounts all passengers riding the entity.

### removeCommandTag(commandTag: [String](#string)): [Null](#null) {data-toc-label='removeCommandTag'}

Removes `commandTag` from the entity. Similar to `/tag remove`

| Argument Name | Type              | Description       |
|---------------|-------------------|-------------------|
| `commandTag`  | [String](#string) | The tag to remove |

### resetPortalCooldown(): [Null](#null) {data-toc-label='resetPortalCooldown'}

Resets the entity's portal cooldown.

### sendMessage(message: [String](#string)): [Null](#null) {data-toc-label='sendMessage'}

Sends `message` to the entity.

| Argument Name | Type              | Description                        |
|---------------|-------------------|------------------------------------|
| `message`     | [String](#string) | The message to send to the entity. |

### setInvisible(invisible: [Boolean](#boolean)): [Null](#null) {data-toc-label='setInvisible'}

Changes the entity to be invisible according to `invisible`.

| Argument Name | Type                | Description         |
|---------------|---------------------|---------------------|
| `invisible`   | [Boolean](#boolean) | The invisible flag. |

### setInvulnerable(invulnerable: [Boolean](#boolean)): [Null](#null) {data-toc-label='setInvulnerable'}

Changes the entity to be invulnerable according to `invulnerable`.

| Argument Name  | Type                | Description            |
|----------------|---------------------|------------------------|
| `invulnerable` | [Boolean](#boolean) | The invulnerable flag. |

### setNoGravity(noGravity: [Boolean](#boolean)): [Null](#null) {data-toc-label='setNoGravity'}

Changes the entity to have no gravity according to `noGravity`.

| Argument Name | Type                | Description          |
|---------------|---------------------|----------------------|
| `noGravity`   | [Boolean](#boolean) | The no gravity flag. |

### setOnFire(onFire: [Boolean](#boolean)): [Null](#null) {data-toc-label='setOnFire'}

Changes the entity to be on fire according to `onFire`.

| Argument Name | Type                | Description       |
|---------------|---------------------|-------------------|
| `onFire`      | [Boolean](#boolean) | The on fire flag. |

### setOnGround(onGround: [Boolean](#boolean)): [Null](#null) {data-toc-label='setOnGround'}

Changes the entity to be on the ground according to `onGround`.

| Argument Name | Type                | Description         |
|---------------|---------------------|---------------------|
| `onGround`    | [Boolean](#boolean) | The on ground flag. |

### setPortalCooldown(portalCooldown: [Integer](#integer)): [Null](#null) {data-toc-label='setPortalCooldown'}

Changes the entity's portal cooldown to `portalCooldown`.

| Argument Name    | Type                | Description                       |
|------------------|---------------------|-----------------------------------|
| `portalCooldown` | [Integer](#integer) | The entity's new portal cooldown. |

### setPos(x: [Float](#float), y: [Float](#float), z: [Float](#float)): [Null](#null) {data-toc-label='setPos'}

Changes the entity's position according to `x`, `y`, and `z`.

| Argument Name | Type            | Description                    |
|---------------|-----------------|--------------------------------|
| `x`           | [Float](#float) | The entity's new x coordinate. |
| `y`           | [Float](#float) | The entity's new y coordinate. |
| `z`           | [Float](#float) | The entity's new z coordinate. |

### setSilent(silent: [Boolean](#boolean)): [Null](#null) {data-toc-label='setSilent'}

Sets the entity to be silent according to `silent`.

| Argument Name | Type                | Description      |
|---------------|---------------------|------------------|
| `silent`      | [Boolean](#boolean) | The silent flag. |

### setSneaking(sneaking: [Boolean](#boolean)): [Null](#null) {data-toc-label='setSneaking'}

Sets the entity to be sneaking according to `sneaking`.

| Argument Name | Type                | Description        |
|---------------|---------------------|--------------------|
| `sneaking`    | [Boolean](#boolean) | The sneaking flag. |

### setSprinting(sprinting: [Boolean](#boolean)): [Null](#null) {data-toc-label='setSprinting'}

Sets the entity to be sprinting according to `sprinting`.

| Argument Name | Type                | Description         |
|---------------|---------------------|---------------------|
| `sprinting`   | [Boolean](#boolean) | The sprinting flag. |

### setSwimming(swimming: [Boolean](#boolean)): [Null](#null) {data-toc-label='setSwimming'}

Sets the entity to be swimming according to `swimming`.

| Argument Name | Type                | Description        |
|---------------|---------------------|--------------------|
| `swimming`    | [Boolean](#boolean) | The swimming flag. |

### shouldDismountUnderwater(): [Boolean](#boolean) {data-toc-label='shouldDismountUnderwater'}

Returns whether the entity should dismount underwater.

### stopRiding(): [Boolean](#boolean) {data-toc-label='stopRiding'}

Makes the entity stop riding its vehicle.

### teleport(x: [Float](#float), y: [Float](#float), z: [Float](#float)): [Null](#null) {data-toc-label='setPos'}

Teleports the entity to `x`, `y`, and `z`.

| Argument Name | Type            | Description                      |
|---------------|-----------------|----------------------------------|
| `x`           | [Float](#float) | The x coordinate to teleport to. |
| `y`           | [Float](#float) | The y coordinate to teleport to. |
| `z`           | [Float](#float) | The z coordinate to teleport to. |

## Enum


## Events


## Float


## Function


## GameModesEnum


## GameRules


## Integer


## ItemStack


## Items


## Item


## List


## LivingEntity


## Method


## MinecraftServer


## Null


## Object


## PlayerEntity


## PlayerManager


## Resource


## ServerPlayerEntity


## String


## Type


## UserDefinedEnum


## UserDefined


## Vec3d


## World

