# Sculk's Standard Library

## BlockPos

Represents the position of a block in a three-dimensional volume.
Each coordinate is integer based.

| Field Name | Type                | Description                   |
|------------|---------------------|-------------------------------|
| `x`        | [Integer](#integer) | The x coordinate of the block |
| `y`        | [Integer](#integer) | The y coordinate of the block |
| `z`        | [Integer](#integer) | The z coordinate of the block |

## Blocks

A class that contains every modded and unmodded block.

### get(blockID: [Resource](#resource)): [Block](#block) {data-toc-label='get'}

Gets the block from the given ID.

## Block

Represents a block.

### asItem(): [Item](#item) {data-toc-label='asItem'}

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

Represents the result of running a command. (Returned from [MinecraftServer.runCommand()](#runcommandcommand-string-commandresult))

### result: [Integer](#integer) | [Null](#null) {data-toc-label='result'}

The result of the command. If the command did not succeed the value will default to [Null](#null).

### succeeded: [Boolean](#boolean) {data-toc-label='succeeded'}

Whether the command succeeded.

### errorMessage: [String](#string) | [Null](#null) {data-toc-label='errorMessage'}

Whether the command succeeded. If the command succeeded the value will default to [Null](#null).

## Dictionary

Represents a dictionary.

## Difficulties

This enum stores all difficulties.

Constants:

- EASY
- NORMAL
- HARD
- PEACEFUL

## Entity

### addCommandTag(commandTag: [String](#string)): [Null](#null) {data-toc-label='addCommandTag'}

Adds the `commandTag` tag to the entity. Similar to `/tag add`

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

Removes the `commandTag` from the entity. Similar to `/tag remove`

### resetPortalCooldown(): [Null](#null) {data-toc-label='resetPortalCooldown'}

Resets the entity's portal cooldown.

### sendMessage(contents: [String](#string)): [Null](#null) {data-toc-label='sendMessage'}

Sends a message with contents `contents` to the entity.

### setInvisible(invisible: [Boolean](#boolean)): [Null](#null) {data-toc-label='setInvisible'}

Sets the entity to be invisible according to `invisible`.

### setInvulnerable(invulnerable: [Boolean](#boolean)): [Null](#null) {data-toc-label='setInvulnerable'}

Sets the entity to be invulnerable according to `invulnerable`.

### setNoGravity(noGravity: [Boolean](#boolean)): [Null](#null) {data-toc-label='setNoGravity'}

Sets the entity to have no gravity according to `noGravity`.

### setOnFire(onFire: [Boolean](#boolean)): [Null](#null) {data-toc-label='setOnFire'}

Sets the entity to be on fire according to `onFire`.

### setOnGround(onGround: [Boolean](#boolean)): [Null](#null) {data-toc-label='setOnGround'}

Sets the entity to be on the ground according to `onGround`.

### setPortalCooldown(portalCooldown: [Integer](#integer)): [Null](#null) {data-toc-label='setPortalCooldown'}

Sets the entity's portal cooldown to `portalCooldown`.

### setPos(x: [Float](#float), y: [Float](#float), z: [Float](#float)): [Null](#null) {data-toc-label='setPos'}

Changes the entity's position according to `x`, `y`, and `z`.

### setSilent(silent: [Boolean](#boolean)): [Null](#null) {data-toc-label='setSilent'}

Sets the entity to be silent according to `silent`.

### setSneaking(sneaking: [Boolean](#boolean)): [Null](#null) {data-toc-label='setSneaking'}

Sets the entity to be sneaking according to `sneaking`.

### setSprinting(sprinting: [Boolean](#boolean)): [Null](#null) {data-toc-label='setSprinting'}

Sets the entity to be sprinting according to `sprinting`.

### setSwimming(swimming: [Boolean](#boolean)): [Null](#null) {data-toc-label='setSwimming'}

Sets the entity to be swimming according to `swimming`.

### shouldDismountUnderwater(): [Boolean](#boolean) {data-toc-label='shouldDismountUnderwater'}

Returns whether the entity should dismount underwater.

### stopRiding(): [Boolean](#boolean) {data-toc-label='stopRiding'}

Makes the entity stop riding its vehicle.

### teleport(x: [Float](#float), y: [Float](#float), z: [Float](#float)): [Null](#null) {data-toc-label='setPos'}

Teleports the entity to `x`, `y`, and `z`.

## Enum

All enums extend this class.

## Events

Please see [Events](events.md) for information.

## Float

Represents a floating point number.

## Function

Represents a function.

## GameModes

This enum stores all game modes.

Constants:

- SURVIVAL
- CREATIVE
- ADVENTURE
- SPECTATOR

## GameRules

### getDoFireTick(): [Boolean](#boolean) {data-toc-label='getDoFireTick'}

Returns the value of the doFireTick gamerule.

### getDoMobGriefing(): [Boolean](#boolean) {data-toc-label='getDoMobGriefing'}

Returns the value of the doMobGriefing gamerule.

### getKeepInventory(): [Boolean](#boolean) {data-toc-label='getKeepInventory'}

Returns the value of the keepInventory gamerule.

### getDoMobSpawning(): [Boolean](#boolean) {data-toc-label='getDoMobSpawning'}

Returns the value of the doMobSpawning gamerule.

### getDoMobLoot(): [Boolean](#boolean) {data-toc-label='getDoMobLoot'}

Returns the value of the doMobLoot gamerule.

### getDoTileDrops(): [Boolean](#boolean) {data-toc-label='getDoTileDrops'}

Returns the value of the doTileDrops gamerule.

### getDoEntityDrops(): [Boolean](#boolean) {data-toc-label='getDoEntityDrops'}

Returns the value of the doEntityDrops gamerule.

### getCommandBlockOutput(): [Boolean](#boolean) {data-toc-label='getCommandBlockOutput'}

Returns the value of the commandBlockOutput gamerule.

### getNaturalRegeneration(): [Boolean](#boolean) {data-toc-label='getNaturalRegeneration'}

Returns the value of the naturalRegeneration gamerule.

### getDoDaylightCycle(): [Boolean](#boolean) {data-toc-label='getDoDaylightCycle'}

Returns the value of the doDaylightCycle gamerule.

### getLogAdminCommands(): [Boolean](#boolean) {data-toc-label='getLogAdminCommands'}

Returns the value of the logAdminCommands gamerule.

### getShowDeathMessages(): [Boolean](#boolean) {data-toc-label='getShowDeathMessages'}

Returns the value of the showDeathMessages gamerule.

### getRandomTickSpeed(): [Integer](#integer) {data-toc-label='getRandomTickSpeed'}

Returns the value of the randomTickSpeed gamerule.

### getSendCommandFeedback(): [Boolean](#boolean) {data-toc-label='getSendCommandFeedback'}

Returns the value of the sendCommandFeedback gamerule.

### getReducedDebugInfo(): [Boolean](#boolean) {data-toc-label='getReducedDebugInfo'}

Returns the value of the reducedDebugInfo gamerule.

### getSpectatorsGenerateChunks(): [Boolean](#boolean) {data-toc-label='getSpectatorsGenerateChunks'}

Returns the value of the spectatorsGenerateChunks gamerule.

### getSpawnRadius(): [Integer](#integer) {data-toc-label='getSpawnRadius'}

Returns the value of the spawnRadius gamerule.

### getDisableElytraMovementCheck(): [Boolean](#boolean) {data-toc-label='getDisableElytraMovementCheck'}

Returns the value of the disableElytraMovementCheck gamerule.

### getMaxEntityCramming(): [Integer](#integer) {data-toc-label='getMaxEntityCramming'}

Returns the value of the maxEntityCramming gamerule.

### getDoWeatherCycle(): [Boolean](#boolean) {data-toc-label='getDoWeatherCycle'}

Returns the value of the doWeatherCycle gamerule.

### getDoLimitedCrafting(): [Boolean](#boolean) {data-toc-label='getDoLimitedCrafting'}

Returns the value of the doLimitedCrafting gamerule.

### getMaxCommandChainLength(): [Integer](#integer) {data-toc-label='getMaxCommandChainLength'}

Returns the value of the maxCommandChainLength gamerule.

### getCommandModificationBlockLimit(): [Integer](#integer) {data-toc-label='getCommandModificationBlockLimit'}

Returns the value of the commandModificationBlockLimit gamerule.

### getAnnounceAdvancements(): [Boolean](#boolean) {data-toc-label='getAnnounceAdvancements'}

Returns the value of the announceAdvancements gamerule.

### getDisableRaids(): [Boolean](#boolean) {data-toc-label='getDisableRaids'}

Returns the value of the disableRaids gamerule.

### getDoInsomnia(): [Boolean](#boolean) {data-toc-label='getDoInsomnia'}

Returns the value of the doInsomnia gamerule.

### getDoImmediateRespawn(): [Boolean](#boolean) {data-toc-label='getDoImmediateRespawn'}

Returns the value of the doImmediateRespawn gamerule.

### getDrowningDamage(): [Boolean](#boolean) {data-toc-label='getDrowningDamage'}

Returns the value of the drowningDamage gamerule.

### getFallDamage(): [Boolean](#boolean) {data-toc-label='getFallDamage'}

Returns the value of the fallDamage gamerule.

### getFireDamage(): [Boolean](#boolean) {data-toc-label='getFireDamage'}

Returns the value of the fireDamage gamerule.

### getFreezeDamage(): [Boolean](#boolean) {data-toc-label='getFreezeDamage'}

Returns the value of the freezeDamage gamerule.

### getDoPatrolSpawning(): [Boolean](#boolean) {data-toc-label='getDoPatrolSpawning'}

Returns the value of the doPatrolSpawning gamerule.

### getDoTraderSpawning(): [Boolean](#boolean) {data-toc-label='getDoTraderSpawning'}

Returns the value of the doTraderSpawning gamerule.

### getDoWardenSpawning(): [Boolean](#boolean) {data-toc-label='getDoWardenSpawning'}

Returns the value of the doWardenSpawning gamerule.

### getForgiveDeadPlayers(): [Boolean](#boolean) {data-toc-label='getForgiveDeadPlayers'}

Returns the value of the forgiveDeadPlayers gamerule.

### getUniversalAnger(): [Boolean](#boolean) {data-toc-label='getUniversalAnger'}

Returns the value of the universalAnger gamerule.

### getPlayersSleepingPercentage(): [Boolean](#boolean) {data-toc-label='getPlayersSleepingPercentage'}

Returns the value of the playersSleepingPercentage gamerule.

### getBlockExplosionDropDecay(): [Boolean](#boolean) {data-toc-label='getBlockExplosionDropDecay'}

Returns the value of the blockExplosionDropDecay gamerule.

### getMobExplosionDropDecay(): [Boolean](#boolean) {data-toc-label='getMobExplosionDropDecay'}

Returns the value of the mobExplosionDropDecay gamerule.

### getTntExplosionDropDecay(): [Boolean](#boolean) {data-toc-label='getTntExplosionDropDecay'}

Returns the value of the tntExplosionDropDecay gamerule.

### getSnowAccumulationHeight(): [Boolean](#boolean) {data-toc-label='getSnowAccumulationHeight'}

Returns the value of the snowAccumulationHeight gamerule.

### getWaterSourceConversion(): [Boolean](#boolean) {data-toc-label='getWaterSourceConversion'}

Returns the value of the waterSourceConversion gamerule.

### getLavaSourceConversion(): [Boolean](#boolean) {data-toc-label='getLavaSourceConversion'}

Returns the value of the lavaSourceConversion gamerule.

### getGlobalSoundEvents(): [Boolean](#boolean) {data-toc-label='getGlobalSoundEvents'}

Returns the value of the globalSoundEvents gamerule.

### getDoVinesSpread(): [Boolean](#boolean) {data-toc-label='getDoVinesSpread'}

Returns the value of the doVinesSpread gamerule.

### getEnderPearlsVanishOnDeath(): [Boolean](#boolean) {data-toc-label='getEnderPearlsVanishOnDeath'}

Returns the value of the enderPearlsVanishOnDeath gamerule.

### getMaxArgumentCount(): [Integer](#integer) {data-toc-label='getMaxArgumentCount'}

A custom gamerule created by sculk. See [Added Gamerules](added_gamerules.md) for more information.

Returns the value of the maxArgumentCount gamerule.

### getMaxLoops(): [Integer](#integer) {data-toc-label='getMaxLoops'}

A custom gamerule created by sculk. See [Added Gamerules](added_gamerules.md) for more information.

Returns the value of the maxLoops gamerule.

### setDoFireTick(doFireTick: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDoFireTick'}

Sets the value of the doFireTick gamerule.

### setDoMobGriefing(doMobGriefing: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDoMobGriefing'}

Sets the value of the doMobGriefing gamerule.

### setKeepInventory(keepInventory: [Boolean](#boolean)): [Null](#null) {data-toc-label='setKeepInventory'}

Sets the value of the keepInventory gamerule.

### setDoMobSpawning(doMobSpawning: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDoMobSpawning'}

Sets the value of the doMobSpawning gamerule.

### setDoMobLoot(doMobLoot: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDoMobLoot'}

Sets the value of the doMobLoot gamerule.

### setDoTileDrops(doTileDrops: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDoTileDrops'}

Sets the value of the doTileDrops gamerule.

### setDoEntityDrops(doEntityDrops: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDoEntityDrops'}

Sets the value of the doEntityDrops gamerule.

### setCommandBlockOutput(commandBlockOutput: [Boolean](#boolean)): [Null](#null) {data-toc-label='setCommandBlockOutput'}

Sets the value of the commandBlockOutput gamerule.

### setNaturalRegeneration(naturalRegeneration: [Boolean](#boolean)): [Null](#null) {data-toc-label='setNaturalRegeneration'}

Sets the value of the naturalRegeneration gamerule.

### setDoDaylightCycle(doDaylightCycle: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDoDaylightCycle'}

Sets the value of the doDaylightCycle gamerule.

### setLogAdminCommands(logAdminCommands: [Boolean](#boolean)): [Null](#null) {data-toc-label='setLogAdminCommands'}

Sets the value of the logAdminCommands gamerule.

### setShowDeathMessages(showDeathMessages: [Boolean](#boolean)): [Null](#null) {data-toc-label='setShowDeathMessages'}

Sets the value of the showDeathMessages gamerule.

### setRandomTickSpeed(randomTickSpeed: [Integer](#integer)): [Null](#null) {data-toc-label='setRandomTickSpeed'}

Sets the value of the randomTickSpeed gamerule.

### setSendCommandFeedback(sendCommandFeedback: [Boolean](#boolean)): [Null](#null) {data-toc-label='setSendCommandFeedback'}

Sets the value of the sendCommandFeedback gamerule.

### setReducedDebugInfo(reducedDebugInfo: [Boolean](#boolean)): [Null](#null) {data-toc-label='setReducedDebugInfo'}

Sets the value of the reducedDebugInfo gamerule.

### setSpectatorsGenerateChunks(spectatorsGenerateChunks: [Boolean](#boolean)): [Null](#null) {data-toc-label='setSpectatorsGenerateChunks'}

Sets the value of the spectatorsGenerateChunks gamerule.

### setSpawnRadius(spawnRadius: [Integer](#integer)): [Null](#null) {data-toc-label='setSpawnRadius'}

Sets the value of the spawnRadius gamerule.

### setDisableElytraMovementCheck(disableElytraMovementCheck: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDisableElytraMovementCheck'}

Sets the value of the disableElytraMovementCheck gamerule.

### setMaxEntityCramming(maxEntityCramming: [Integer](#integer)): [Null](#null) {data-toc-label='setMaxEntityCramming'}

Sets the value of the maxEntityCramming gamerule.

### setDoWeatherCycle(doWeatherCycle: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDoWeatherCycle'}

Sets the value of the doWeatherCycle gamerule.

### setDoLimitedCrafting(doLimitedCrafting: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDoLimitedCrafting'}

Sets the value of the doLimitedCrafting gamerule.

### setMaxCommandChainLength(maxCommandChainLength: [Integer](#integer)): [Null](#null) {data-toc-label='setMaxCommandChainLength'}

Sets the value of the maxCommandChainLength gamerule.

### setCommandModificationBlockLimit(commandModificationBlockLimit: [Integer](#integer)): [Null](#null) {data-toc-label='setCommandModificationBlockLimit'}

Sets the value of the commandModificationBlockLimit gamerule.

### setAnnounceAdvancements(announceAdvancements: [Boolean](#boolean)): [Null](#null) {data-toc-label='setAnnounceAdvancements'}

Sets the value of the announceAdvancements gamerule.

### setDisableRaids(disableRaids: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDisableRaids'}

Sets the value of the disableRaids gamerule.

### setDoInsomnia(doInsomnia: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDoInsomnia'}

Sets the value of the doInsomnia gamerule.

### setDoImmediateRespawn(doImmediateRespawn: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDoImmediateRespawn'}

Sets the value of the doImmediateRespawn gamerule.

### setDrowningDamage(drowningDamage: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDrowningDamage'}

Sets the value of the drowningDamage gamerule.

### setFallDamage(fallDamage: [Boolean](#boolean)): [Null](#null) {data-toc-label='setFallDamage'}

Sets the value of the fallDamage gamerule.

### setFireDamage(fireDamage: [Boolean](#boolean)): [Null](#null) {data-toc-label='setFireDamage'}

Sets the value of the fireDamage gamerule.

### setFreezeDamage(freezeDamage: [Boolean](#boolean)): [Null](#null) {data-toc-label='setFreezeDamage'}

Sets the value of the freezeDamage gamerule.

### setDoPatrolSpawning(doPatrolSpawning: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDoPatrolSpawning'}

Sets the value of the doPatrolSpawning gamerule.

### setDoTraderSpawning(doTraderSpawning: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDoTraderSpawning'}

Sets the value of the doTraderSpawning gamerule.

### setDoWardenSpawning(doWardenSpawning: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDoWardenSpawning'}

Sets the value of the doWardenSpawning gamerule.

### setForgiveDeadPlayers(forgiveDeadPlayers: [Boolean](#boolean)): [Null](#null) {data-toc-label='setForgiveDeadPlayers'}

Sets the value of the forgiveDeadPlayers gamerule.

### setUniversalAnger(universalAnger: [Boolean](#boolean)): [Null](#null) {data-toc-label='setUniversalAnger'}

Sets the value of the universalAnger gamerule.

### setPlayersSleepingPercentage(playersSleepingPercentage: [Boolean](#boolean)): [Null](#null) {data-toc-label='setPlayersSleepingPercentage'}

Sets the value of the playersSleepingPercentage gamerule.

### setBlockExplosionDropDecay(blockExplosionDropDecay: [Boolean](#boolean)): [Null](#null) {data-toc-label='setBlockExplosionDropDecay'}

Sets the value of the blockExplosionDropDecay gamerule.

### setMobExplosionDropDecay(mobExplosionDropDecay: [Boolean](#boolean)): [Null](#null) {data-toc-label='setMobExplosionDropDecay'}

Sets the value of the mobExplosionDropDecay gamerule.

### setTntExplosionDropDecay(tntExplosionDropDecay: [Boolean](#boolean)): [Null](#null) {data-toc-label='setTntExplosionDropDecay'}

Sets the value of the tntExplosionDropDecay gamerule.

### setSnowAccumulationHeight(snowAccumulationHeight: [Boolean](#boolean)): [Null](#null) {data-toc-label='setSnowAccumulationHeight'}

Sets the value of the snowAccumulationHeight gamerule.

### setWaterSourceConversion(waterSourceConversion: [Boolean](#boolean)): [Null](#null) {data-toc-label='setWaterSourceConversion'}

Sets the value of the waterSourceConversion gamerule.

### setLavaSourceConversion(lavaSourceConversion: [Boolean](#boolean)): [Null](#null) {data-toc-label='setLavaSourceConversion'}

Sets the value of the lavaSourceConversion gamerule.

### setGlobalSoundEvents(globalSoundEvents: [Boolean](#boolean)): [Null](#null) {data-toc-label='setGlobalSoundEvents'}

Sets the value of the globalSoundEvents gamerule.

### setDoVinesSpread(doVinesSpread: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDoVinesSpread'}

Sets the value of the doVinesSpread gamerule.

### setEnderPearlsVanishOnDeath(enderPearlsVanishOnDeath: [Boolean](#boolean)): [Null](#null) {data-toc-label='setEnderPearlsVanishOnDeath'}

Sets the value of the enderPearlsVanishOnDeath gamerule.

### setMaxArgumentCount(maxArgumentCount: [Integer](#integer)): [Null](#null) {data-toc-label='setMaxArgumentCount'}

A custom gamerule created by sculk. See [Added Gamerules](added_gamerules.md) for more information.

Sets the value of the maxArgumentCount gamerule.

### setMaxLoops(maxLoops: [Integer](#integer)): [Null](#null) {data-toc-label='setMaxLoops'}

A custom gamerule created by sculk. See [Added Gamerules](added_gamerules.md) for more information.

Sets the value of the maxLoops gamerule.

## Integer

Represents an integer value.


## ItemStack

Represents a stack of items.

### decrement(amount: [Integer](#integer)): [Null](#null) {data-toc-label='decrement'}

Decrements the amount of items in the stack by `amount`.

### getCount(): [Integer](#integer) {data-toc-label='getCount'}

Returns the amount of items in the stack.

### getDamage(): [Integer](#integer) {data-toc-label='getDamage'}

Returns how the damage (lost durability) of the item stack.

Does **NOT** return how much damage the item does!

### getHolder(): [Entity](#entity) {data-toc-label='getHolder'}

Returns the entity who is holding the item.

### getItem(): [Item](#item) {data-toc-label='getItem'}

Returns the item in the stack.

### getMaxCount(): [Integer](#integer) {data-toc-label='getMaxCount'}

Returns the max amount of items that can be in 1 stack.

### getMaxDamage(): [Integer](#integer) {data-toc-label='getMaxDamage'}

Returns the durability of the item.

### getName(): [String](#string) {data-toc-label='getName'}

Returns the name of the item.

### getRepairCost(): [Integer](#integer) {data-toc-label='getRepairCost'}

Returns the repair cost of the item.

### hasEnchantments(): [Boolean](#boolean) {data-toc-label='hasEnchantments'}

Returns whether the item has enchantments.

### increment(amount: [Integer](#integer)): [Null](#null) {data-toc-label='increment'}

Increments the amount of items in the stack by `amount`.

### isDamageable(): [Boolean](#boolean) {data-toc-label='isDamageable'}

Returns whether the item is damageable.

### isDamaged(): [Boolean](#boolean) {data-toc-label='isDamaged'}

Returns whether the item is damaged.

### isEnchantable(): [Boolean](#boolean) {data-toc-label='isEnchantable'}

Returns whether the item is enchantable.

### isFood(): [Boolean](#boolean) {data-toc-label='isFood'}

Returns whether the item is food.

### isInFrame(): [Boolean](#boolean) {data-toc-label='isInFrame'}

Returns whether the item is in a frame.

### isStackable(): [Boolean](#boolean) {data-toc-label='isStackable'}

Returns whether the item is stackable.

### setCount(amount: [Integer](#integer)): [Null](#null) {data-toc-label='setCount'}

Sets the amount of items in the stack to `amount`.

### setDamage(damage: [Integer](#integer)): [Null](#null) {data-toc-label='setDamage'}

Sets the damage (lost durability) of the item.

### setRepairCost(repair_cost: [Integer](#integer)): [Null](#null) {data-toc-label='setRepairCost'}

Sets the repair cost of the item.


## Items

A class that contains every modded and unmodded item.

### get(itemID: [Resource](#resource)): [Item](#item) {data-toc-label='get'}

Gets the item from the given ID.

## Item

Represents an item.

### getMaxCount(): [Integer](#integer) {data-toc-label='getMaxCount'}

Returns the max amount of items that can be in a stack.

### getMaxDamage(): [Integer](#integer) {data-toc-label='getMaxDamage'}

Returns the durability of the item.

### getName(): [String](#string) {data-toc-label='getName'}

Returns the name of the item.

### isDamageable(): [Boolean](#boolean) {data-toc-label='isDamageable'}

Returns whether the item is damageable.

### isFireproof(): [Boolean](#boolean) {data-toc-label='isFireproof'}

Returns whether the item is fireproof.

### isFood(): [Boolean](#boolean) {data-toc-label='isFood'}

Returns whether the item is food.


## List

Represents a list of items.

## LivingEntity

Represents a living entity.

### tiltScreen(x: [Float](#float), z: [Float](#float)): [Null](#null) {data-toc-label='tiltScreen'}

Tilts the screen of the entity.

### wakeUp(): [Null](#null) {data-toc-label='wakeUp'}

Wakes the entity up.

## Method

Represents a method on a class.

## MinecraftServer

Represents the Minecraft Server.

### runCommand(command: [String](#string)): [CommandResult](#commandresult) {data-toc-label='runCommand'}

Runs the command `command`.

### setPVPEnabled(pvp_enabled: [Boolean](#boolean)): [Null](#null) {data-toc-label='setPVPEnabled'}

Sets pvp to be enabled according to `pvp_enabled`.

### setDifficultyLocked(difficulty_locked: [Boolean](#boolean)): [Null](#null) {data-toc-label='setDifficultyLocked'}

Sets the difficulty to be locked according to `difficulty_locked`.


### isPVPEnabled(): [Boolean](#boolean) {data-toc-label='isPVPEnabled'}

Returns whether pvp is enabled.

### isNetherEnabled(): [Boolean](#boolean) {data-toc-label='isNetherEnabled'}

Returns whether the nether is enabled.

### isFlightEnabled(): [Boolean](#boolean) {data-toc-label='isFlightEnabled'}

Returns whether flight is enabled.

### getServerPort(): [Integer](#integer) {data-toc-label='getServerPort'}

Returns the port of the server.

### getServerIP(): [String](#string) {data-toc-label='getServerIP'}

Returns the IP of the server.

### isHardcore(): [Boolean](#boolean) {data-toc-label='isHardcore'}

Returns whether the server is hardcore.

### areCommandBlocksEnabled(): [Boolean](#boolean) {data-toc-label='areCommandBlocksEnabled'}

Returns whether command blocks are enabled.

### setDifficulty(difficulty: [Difficulty](#difficulties)): [Null](#null) {data-toc-label='setDifficulty'}

Sets the difficulty to `difficuly`.

### isModInstalled(modID: [Resource](#resource)): [Boolean](#boolean) {data-toc-label='isModInstalled'}

Returns whether `modID` is installed.

## Null

Represents `null`.

## Object

The base class of every class.

## PlayerEntity

Represents the player.

### addExperiencePoints(experience_points: [Integer](#integer)): [Null](#null) {data-toc-label='addExperiencePoints'}

Adds `experience_points` amount of XP points to the player.

### addExperienceLevels(experience_levels: [Integer](#integer)): [Null](#null) {data-toc-label='addExperienceLevels'}

Adds `experience_levels` amount of XP levels to the player.

### isCreative(): [Boolean](#boolean) {data-toc-label='isCreative'}

Returns whether the player is in creative mode.

### isSpectator(): [Boolean](#boolean) {data-toc-label='isSpectator'}

Returns whether the player is in spectator mode.

### getName(): [String](#string) {data-toc-label='getName'}

Returns the name of the player.

### getUUID(): [String](#string) {data-toc-label='getUUID'}

Returns the UUID of the player.

## PlayerManager

### areCheatsEnabled(): [Boolean](#boolean) {data-toc-label='areCheatsEnabled'}

Returns whether cheats are enabled.

### getCurrentPlayerCount(): [Integer](#integer) {data-toc-label='getCurrentPlayerCount'}

Returns the current amount of players.

### getMaxPlayerCount(): [Integer](#integer) {data-toc-label='getMaxPlayerCount'}

Returns the max player count.

### getSimulationDistance(): [Integer](#integer) {data-toc-label='getSimulationDistance'}

Returns the simulation distance.

### getViewDistance(): [Integer](#integer) {data-toc-label='getViewDistance'}

Returns the view distance.

### isWhitelistEnabled(): [Boolean](#boolean) {data-toc-label='isWhitelistEnabled'}

Returns whether whitelist is enabled.

### setCheatsEnabled(cheats_enabled: [Boolean](#boolean)): [Null](#null) {data-toc-label='setCheatsEnabled'}

Sets cheats to be enabled according to `cheats_enabled`.

### setSimulationDistance(simulation_distance: [Boolean](#boolean)): [Null](#null) {data-toc-label='setSimulationDistance'}

Sets the simulation distance according to `simulation_distance`.

### setViewDistance(view_distance: [Boolean](#boolean)): [Null](#null) {data-toc-label='setViewDistance'}

Sets the view distance according to `view_distance`.

### setWhitelistEnabled(whitelist_enabled: [Boolean](#boolean)): [Null](#null) {data-toc-label='setWhitelistEnabled'}

Sets whitelist to be enabled according to `whitelist_enabled`.

### getPlayer(name: [String](#string)): [Null](#null) {data-toc-label='getPlayer'}

Returns the player with the name `name`.


## Resource

Represents an identifier. It looks like `namespace:path`.

## ServerPlayerEntity

Represents a player on the server level. Extends from [PlayerEntity](#playerentity)

### changeGameMode(game_mode: [GameMode](#gamemodes)): [Null](#null) {data-toc-label='changeGameMode'}

Changes the players game mode based on `game_mode`.

### dropSelectedItem(): [Null](#null) {data-toc-label='dropSelectedItem'}

Drops the players selected item.

### getIp(): [String](#string) {data-toc-label='getIp'}

Returns the players IP address.

### getViewDistance(): [Integer](#integer) {data-toc-label='getViewDistance'}

Returns the players view distance.

### setExperienceLevels(experience_levels: [Integer](#integer)): [Null](#null) {data-toc-label='setExperienceLevels'}

Sets the players experience levels to `experience_levels`.

### setExperiencePoints(experience_points: [Integer](#integer)): [Null](#null) {data-toc-label='setExperiencePoints'}

Sets the players experience points to `experience_points`.



## String

Represents a string.

## Type


## Vec3d

Represents a 3D vector. Similar to [BlockPos](#blockpos) except values are float based.

| Field Name | Type            | Description      |
|------------|-----------------|------------------|
| `x`        | [Float](#float) | The x coordinate |
| `y`        | [Float](#float) | The y coordinate |
| `z`        | [Float](#float) | The z coordinate |


## World

Represents a world.

### canSetBlock(block_pos: [BlockPos](#blockpos)): [Boolean](#boolean) {data-toc-label='canSetBlock'}

Returns whether a block can be placed at `block_pos`.

### getTime(): [Integer](#integer) {data-toc-label='getTime'}

Returns the total time since the world was created.

### getTimeOfDay(): [Integer](#integer) {data-toc-label='getTimeOfDay'}

Returns the time of day.

### hasRain(block_pos: [BlockPos](#blockpos)): [Boolean](#boolean) {data-toc-label='hasRain'}

Returns whether it is raining at `block_pos`.

### isDay(): [Boolean](#boolean) {data-toc-label='isDay'}

Returns whether it is day.

### isNight(): [Boolean](#boolean) {data-toc-label='isNight'}

Returns whether it is night.

### isRaining(): [Boolean](#boolean) {data-toc-label='isRaining'}

Returns whether it is raining.

### isThundering(): [Boolean](#boolean) {data-toc-label='isThundering'}

Returns whether it is thundering.

### getPlayers(): [List\[Player\]](#list) {data-toc-label='getPlayers'}

Returns the players in the world.

### isFlat(): [Boolean](#boolean) {data-toc-label='isFlat'}

Returns whether the world is flat.

### isSleepingEnabled(): [Boolean](#boolean) {data-toc-label='isSleepingEnabled'}

Returns whether sleeping is enabled.

### getSeed(): [Integer](#integer) {data-toc-label='getSeed'}

Returns the seed.

### setSpawnPos(spawn_pos: [BlockPos](#blockpos)): [Null](#null) {data-toc-label='setSpawnPos'}

Sets the spawn position to `spawn_pos`.

### setTimeOfDay(time_of_day: [Integer](#integer)): [Null](#null) {data-toc-label='setTimeOfDay'}

Sets the time of day to `time_of_day`.

### setBlock(block_pos: [BlockPos](#blockpos), block: [Block](#block)): [Null](#null) {data-toc-label='setBlock'}

Sets the block at `block_pos` to `block`.
