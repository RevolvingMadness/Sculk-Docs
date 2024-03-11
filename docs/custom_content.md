# Custom Content

Adding custom content is the **main** part of datapacks in my opinion. In Beta 0.0.5 Sculk adds support for custom blocks & items.

Custom content always has to be registered in the `start` tag.

## Blocks

In this example, we will be adding a calcite brick, similar to stone bricks but calcite.

### Registering the Block

In your `start` script add the following.

```dart title="start.sk"
var brickSettings = BlockSettings.of(Blocks.get("stone_bricks")); // Copy the settings of stone bricks

// If you want an item to be registered too, use registerWithItem otherwise just use register
Blocks.registerWithItem(Block("calcite_bricks", brickSettings));
```

There are a few settings you can tweak to customize your block. They are listed below:

#### hardness

`hardness` determines the breaking speed of the block.

#### resistance

`resistance` determines the blast resistance of the block.

#### collidable

`collidable` determines whether the block has a hitbox / is collidable with entities.

#### luminance

`luminance` determines the light level that  the block emits.

#### slipperiness

`slipperiness` determines the slipperiness of the block.

#### burnable

`burnable` determines whether the block is burnable.

#### pistonBehavior

`pistonBehavior` determines what the block will do when a piston tries to push it.

##### NORMAL

The block will get pushed.

##### DESTROY

The block will get destroyed.

##### BLOCK

The block will not get pushed.

##### IGNORE

No noticeable difference to `BLOCK` while testing.

##### PUSH_ONLY

The block will only be able to get pushed and not pulled even with a sticky piston.

#### hasBlockBreakParticles

`hasBlockBreakParticles` determines whether the block will spawn particles when broken.

#### instrument

`instrument` determines what instrument a noteblock will play.

#### requiresTool

`requiresTool` determines whether the block requires a tool to drop loot.

### Adding a Loot Table

In `Datapack Name/data/namespace/loot_tables/blocks`, create a file named `<block id>.json`.

```json title="calcite_bricks.json"
{
    "type": "minecraft:block",
    "pools": [
        {
            "bonus_rolls": 0.0,
            "conditions": [
                {
                    "condition": "minecraft:survives_explosion"
                }
            ],
            "entries": [
                {
                    "type": "minecraft:item",
                    "name": "useful_calcite:calcite_bricks"
                }
            ],
            "rolls": 1.0
        }
    ]
}
```

### Making a Pickaxe Required to Drop Loot

To make the block break faster with a certain tool, create a file in `Datapack Name/data/minecraft/tags/blocks/mineable/<tool>.json` where `<tool>` is one of the following: `pickaxe`, `axe`, `shovel`, `sword`.

```json title="pickaxe.json"
{
    "replace": false,
    "values": [
        "useful_calcite:calcite_bricks"
    ]
}
```

### Creating the Resourcepack

#### Creating the Blockstates

In `Resourcepack Name/assets/datapack_namespace/blockstates` create a file named `<block id>.json`.

```dart title="calcite_bricks.json"
{
  "variants": {
      "": {
          "model": "useful_calcite:block/calcite_bricks"
      }
  }
}
```

Currently, blockstates are not supported but *may* in the future.

#### Creating the Language File

In `Resourcepack Name/assets/datapack_namespace/lang` create a file named `en_us.json`. You can replace `en_us` with any other language you want.

```dart title="en_us.json"
{
  "item.useful_calcite.calcite_bricks": "Calcite Bricks",
  "block.useful_calcite.calcite_bricks": "Calcite Bricks"
}
```

#### Creating the Item & Block Models

##### The Block Model

In `Resourcepack Name/assets/datapack_namespace/models/block` create a file named `<block id>.json`.

```dart title="calcite_bricks.json"
{
  "parent": "minecraft:block/cube_all",
  "textures": {
    "all": "useful_calcite:block/calcite_bricks"
  }
}
```

You can use [Blockbench](https://www.blockbench.net/) for more complex models.

##### The Item Model

If you didn't use `registerWithItem` you can skip this step.

In `Resourcepack Name/assets/datapack_namespace/models/item` create a file named `<block id>.json`.

```dart title="calcite_bricks.json"
{
  "parent": "useful_calcite:block/calcite_bricks"
}
```

##### Adding Textures

In `Resourcepack Name/assets/datapack_namespace/textures/block` add your block texture in the format `<block id>.png`.

## Items

### Registering the Item

In your `start` script add the following.

```dart title="start.sk"
var itemSettings = ItemSettings();

Items.register(Item("my_item", itemSettings));
```

There are a few settings you can tweak to customize your item. They are listed below:

##### maxCount

The max amount of items in a stack. Cannot be above 64.

##### maxDamage

The max amount of the damage the item can take before it breaks. `maxCount` has to be 1.

##### fireproof

Whether the item is immune to lava.

#### Creating the Resourcepack

##### The Item Model

In `Resourcepack Name/assets/datapack_namespace/models/item` create a file named `<item id>.json`.

```dart title="item_id.json"
{
  "parent": "minecraft:item/generated",
  "textures": {
    "layer0": "useful_calcite:item/my_item"
  }
}
```

##### Adding Textures

In `Resourcepack Name/assets/datapack_namespace/textures/item` add your item texture in the format `<item id>.png`.











###### Make a pull request if you have any suggestions to make this better