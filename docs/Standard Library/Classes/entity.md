# Entity

## addTag(tag: [String](string.md)) -> [Null](null.md) {data-toc-label='addTag'}

Adds the `tag` tag to the entity. Similar to `/tag add`

## canFreeze() -> [Boolean](boolean.md) {data-toc-label='canFreeze'}

Returns whether the entity can freeze.

## canUsePortals() -> [Boolean](boolean.md) {data-toc-label='canUsePortals'}

Returns whether the entity can use portals.

## dismount() -> [Null](null.md) {data-toc-label='dismount'}

Dismounts the entity from any vehicle it's riding.

## extinguish(play_sound: [Boolean](boolean.md)) -> [Null](null.md) {data-toc-label='extinguish'}

Extinguishes the entity. Plays sound if `play_sound` is true.

## getBlockPos() -> [BlockPos](blockpos.md) {data-toc-label='getBlockPos'}

Returns the block pos of the entity.

## getBlockX() -> [Integer](integer.md) {data-toc-label='getBlockX'}

Returns the x coordinate of the entity.

## getBlockY() -> [Integer](integer.md) {data-toc-label='getBlockY'}

Returns the y coordinate of the entity.

## getBlockZ() -> [Integer](integer.md) {data-toc-label='getBlockZ'}

Returns the z coordinate of the entity.

## getTags() -> [List\[String\]](list.md) {data-toc-label='getTags'}

Returns the tags on the entity. Similar to `/tag list`.

## getName() -> [String](string.md) {data-toc-label='getName'}

Returns the name of the entity.

## getPassengers() -> [List\[Entity\]](list.md) {data-toc-label='getPassengers'}

Returns the passengers riding the entity.

## getVehicle() -> [Entity](entity.md) {data-toc-label='getVehicle'}

Returns the vehicle the entity is riding.

## getX() -> [Float](float.md) {data-toc-label='getX'}

Returns the x coordinate of the entity.

## getY() -> [Float](float.md) {data-toc-label='getY'}

Returns the y coordinate of the entity.

## getZ() -> [Float](float.md) {data-toc-label='getZ'}

Returns the z coordinate of the entity.

## hasControllingPassenger() -> [Boolean](boolean.md) {data-toc-label='hasControllingPassenger'}

Returns whether the passenger riding the entity is controlling.

## hasNoGravity() -> [Boolean](boolean.md) {data-toc-label='hasNoGravity'}

Returns whether the entity has no gravity.

## hasPassenger(passenger: [Entity](entity.md)) -> [Boolean](boolean.md) {data-toc-label='hasPassenger'}

Returns whether `passenger` is riding the entity.

## hasPassengers() -> [Boolean](boolean.md) {data-toc-label='hasPassengers'}

Returns whether the entity has passengers.

## hasVehicle() -> [Boolean](boolean.md) {data-toc-label='hasVehicle'}

Returns whether the entity is riding an entity.

## isCrawling() -> [Boolean](boolean.md) {data-toc-label='isCrawling'}

Returns whether the entity is crawling.

## isDescending() -> [Boolean](boolean.md) {data-toc-label='isDescending'}

Returns whether the entity is descending.

## isFireImmune() -> [Boolean](boolean.md) {data-toc-label='isFireImmune'}

Returns whether the entity is fire immune.

## isFrozen() -> [Boolean](boolean.md) {data-toc-label='isFrozen'}

Returns whether the entity is frozen.

## isGlowing() -> [Boolean](boolean.md) {data-toc-label='isGlowing'}

Returns whether the entity is glowing.

## isInFluid() -> [Boolean](boolean.md) {data-toc-label='isInFluid'}

Returns whether the entity is in a fluid.

## isInLava() -> [Boolean](boolean.md) {data-toc-label='isInLava'}

Returns whether the entity is in lava.

## isInsideWall() -> [Boolean](boolean.md) {data-toc-label='isInsideWall'}

Returns whether the entity is in inside a wall.

## isInvisible() -> [Boolean](boolean.md) {data-toc-label='isInvisible'}

Returns whether the entity is invisible.

## isInvulnerable() -> [Boolean](boolean.md) {data-toc-label='isInvulnerable'}

Returns whether the entity is invulnerable.

## isOnFire() -> [Boolean](boolean.md) {data-toc-label='isOnFire'}

Returns whether the entity is on fire.

## isOnGround() -> [Boolean](boolean.md) {data-toc-label='isOnGround'}

Returns whether the entity is on ground.

## isOnRail() -> [Boolean](boolean.md) {data-toc-label='isOnRail'}

Returns whether the entity is on a rail.

## isSilent() -> [Boolean](boolean.md) {data-toc-label='isSilent'}

Returns whether the entity is silent.

## isSneaking() -> [Boolean](boolean.md) {data-toc-label='isSneaking'}

Returns whether the entity is sneaking.

## isSprinting() -> [Boolean](boolean.md) {data-toc-label='isSprinting'}

Returns whether the entity is sprinting.

## isSwimming() -> [Boolean](boolean.md) {data-toc-label='isSwimming'}

Returns whether the entity is swimming.

## isTouchingWater() -> [Boolean](boolean.md) {data-toc-label='isTouchingWater'}

Returns whether the entity is touching water.

## isTouchingWaterOrRain() -> [Boolean](boolean.md) {data-toc-label='isTouchingWaterOrRain'}

Returns whether the entity is touching water or rain.

## isWet() -> [Boolean](boolean.md) {data-toc-label='isWet'}

Returns whether the entity is touching water, being rained on, or is inside a bubble column.

## kill() -> [Null](null.md) {data-toc-label='kill'}

Kills the entity.

## raycast(distance: [Float](float.md), target: [Block](block.md), check_fluids: [Boolean](boolean.md)) -> [BlockHitResult](blockhitresult.md) {data-toc-label='raycast'}

Raycasts `distance` until it hits `target` and if `check_fluids` is true and it encounters a fluid it will stop.

## removePassengers() -> [Null](null.md) {data-toc-label='removePassengers'}

Dismounts all passengers riding the entity.

## removeTag(tag: [String](string.md)) -> [Null](null.md) {data-toc-label='removeTag'}

Removes the `commandTag` from the entity. Similar to `/tag remove`

## resetPortalCooldown() -> [Null](null.md) {data-toc-label='resetPortalCooldown'}

Resets the entity's portal cooldown.

## sendMessage(contents: [String](string.md)) -> [Null](null.md) {data-toc-label='sendMessage'}

Sends a message with contents `contents` to the entity.

## setInvisible(invisible: [Boolean](boolean.md)) -> [Null](null.md) {data-toc-label='setInvisible'}

Sets the entity to be invisible according to `invisible`.

## setInvulnerable(invulnerable: [Boolean](boolean.md)) -> [Null](null.md) {data-toc-label='setInvulnerable'}

Sets the entity to be invulnerable according to `invulnerable`.

## setNoGravity(noGravity: [Boolean](boolean.md)) -> [Null](null.md) {data-toc-label='setNoGravity'}

Sets the entity to have no gravity according to `noGravity`.

## setOnFire(onFire: [Boolean](boolean.md)) -> [Null](null.md) {data-toc-label='setOnFire'}

Sets the entity to be on fire according to `onFire`.

## setOnGround(onGround: [Boolean](boolean.md)) -> [Null](null.md) {data-toc-label='setOnGround'}

Sets the entity to be on the ground according to `onGround`.

## setPortalCooldown(portalCooldown: [Integer](integer.md)) -> [Null](null.md) {data-toc-label='setPortalCooldown'}

Sets the entity's portal cooldown to `portalCooldown`.

## setPos(x: [Float](float.md), y: [Float](float.md), z: [Float](float.md)) -> [Null](null.md) {data-toc-label='setPos'}

Changes the entity's position according to `x`, `y`, and `z`.

## setSilent(silent: [Boolean](boolean.md)) -> [Null](null.md) {data-toc-label='setSilent'}

Sets the entity to be silent according to `silent`.

## setSneaking(sneaking: [Boolean](boolean.md)) -> [Null](null.md) {data-toc-label='setSneaking'}

Sets the entity to be sneaking according to `sneaking`.

## setSprinting(sprinting: [Boolean](boolean.md)) -> [Null](null.md) {data-toc-label='setSprinting'}

Sets the entity to be sprinting according to `sprinting`.

## setSwimming(swimming: [Boolean](boolean.md)) -> [Null](null.md) {data-toc-label='setSwimming'}

Sets the entity to be swimming according to `swimming`.

## shouldDismountUnderwater() -> [Boolean](boolean.md) {data-toc-label='shouldDismountUnderwater'}

Returns whether the entity should dismount underwater.

## stopRiding() -> [Boolean](boolean.md) {data-toc-label='stopRiding'}

Makes the entity stop riding its vehicle.

## teleport(x: [Float](float.md), y: [Float](float.md), z: [Float](float.md)) -> [Null](null.md) {data-toc-label='setPos'}

Teleports the entity to `x`, `y`, and `z`.
