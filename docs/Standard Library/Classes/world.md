# World

Represents a world.

## breakBlock(pos: [BlockPos](blockpos.md), drop_items: [Boolean](boolean.md)) -> [Null](null.md) {data-toc-label='breakBlock'}

Breaks the block at `pos` and drops the items if `drop_items` is true.

## canSetBlock(block_pos: [BlockPos](blockpos.md)) -> [Boolean](boolean.md) {data-toc-label='canSetBlock'}

Returns whether a block can be placed at `block_pos`.

## getBlock(pos: [BlockPos](blockpos.md)) -> [Block](block.md) {data-toc-label='getBlock'}

Returns the block at `pos`.

## getTime() -> [Integer](integer.md) {data-toc-label='getTime'}

Returns the total time since the world was created.

## getTimeOfDay() -> [Integer](integer.md) {data-toc-label='getTimeOfDay'}

Returns the time of day.

## hasRain(block_pos: [BlockPos](blockpos.md)) -> [Boolean](boolean.md) {data-toc-label='hasRain'}

Returns whether it is raining at `block_pos`.

## isDay() -> [Boolean](boolean.md) {data-toc-label='isDay'}

Returns whether it is day.

## isNight() -> [Boolean](boolean.md) {data-toc-label='isNight'}

Returns whether it is night.

## isRaining() -> [Boolean](boolean.md) {data-toc-label='isRaining'}

Returns whether it is raining.

## isThundering() -> [Boolean](boolean.md) {data-toc-label='isThundering'}

Returns whether it is thundering.

## getPlayers() -> [List\[Player\]](list.md) {data-toc-label='getPlayers'}

Returns the players in the world.

## isFlat() -> [Boolean](boolean.md) {data-toc-label='isFlat'}

Returns whether the world is flat.

## isSleepingEnabled() -> [Boolean](boolean.md) {data-toc-label='isSleepingEnabled'}

Returns whether sleeping is enabled.

## getSeed() -> [Integer](integer.md) {data-toc-label='getSeed'}

Returns the seed.

## setSpawnPos(spawn_pos: [BlockPos](blockpos.md)) -> [Null](null.md) {data-toc-label='setSpawnPos'}

Sets the spawn position to `spawn_pos`.

## setTimeOfDay(time_of_day: [Integer](integer.md)) -> [Null](null.md) {data-toc-label='setTimeOfDay'}

Sets the time of day to `time_of_day`.

## placeBlock(block_pos: [BlockPos](blockpos.md), block: [Block](block.md)) -> [Null](null.md) {data-toc-label='setBlock'}

Places the block `block` at `block_pos`.
