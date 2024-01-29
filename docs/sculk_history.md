# History

# 0.0.1

## Added

- The entire programming language

# 0.0.2

## Added

- [Folder support for resources](#folder-support-for-resources)
- `as` keyword to import statements
- [From statement](import.md#from-statement)
- [Switch statement](switch.md#switch-statement)
- [Switch expression](switch.md#switch-expression)
- [Increment/decrement operators](#incrementdecrement-operators)
- [Access to builtin classes](#access-to-built-in-classes)
- [Constructors for builtin classes](#constructors-for-built-in-classes)
- [Ternary expressions](#ternary-expressions)
- Division by zero error
- [Entity.raycast(distance: Float, target: Block, check_fluids: Boolean): Boolean](stdlib.md#raycastdistance-float-target-block-check_fluids-boolean-boolean)
- [base64decode(base64string: String): String](stdlib.md#base64decodebase64string-string-string)
- [base64encode(string: String): String](stdlib.md#base64encodestring-string-string)
- [EntityTypes](stdlib.md#entitytypes)
- [List.contains(object: Object): Boolean](stdlib.md#containsobject-object-boolean-data)

## Changed

- Entity.extinguish(): Null and Entity.extinguishWithSound(): Null have been merged into [Entity.extinguish(play_sound: Boolean): Null](stdlib.md#extinguishplay_sound-boolean-null)
- Fix circular imports
- Reverted custom load script tag
- Float now extends Integer

### Folder Support for Resources

The resource type now supports `foo:bar/foobar`.

### Increment/Decrement Operators

You can now apply unary and postfix `++` and `--` operators to numbers.

```dart
var x = 1;
print(x); // 1
x++;
print(x); // 2
```

```dart
var x = 1;
print(x++); // 1
print(x); // 2
```

```dart
var x = 1;
print(++x); // 2
print(x); // 2
```

### Access to Built-in Classes

You now have access to classes like `Integer` and `Boolean`. That means you can now do. Previously it would error.

```dart
var x = 1;

print(x instanceof Integer); // true
print(x instanceof Boolean); // false
```

### Constructors for Built-in Classes

You can now instantiate built-in classes. Previously it would error.

```dart
var x = CommandResult(1, true, null);
```

### Ternary Expressions

You can now do.

```dart
var x = true;

print(x ? "x is true" : "x is false");
```

# 0.0.3

## Added

- [abs(number: Integer | Float): Object](stdlib.md#absnumber-integer--float-integer--float)
- `String` is iterable
- Data can be written to an entity
- [String.startsWith(text: String): Boolean](stdlib.md#startswithprefix-string-boolean)
- [String.endsWith(text: String): Boolean](stdlib.md#endswithsuffix-string-boolean)
- `break` can now be used in switch statement
- [String.split(splitter: String): List\[String\]](stdlib.md#splitdelimiter-string-liststring)
- [Integer.parseInteger(integer: String): Integer](stdlib.md#static-parseintegerinteger-string-integer)
- [Float.parseFloat(float: String): Float](stdlib.md#static-parsefloatfloat-string-float)
- [ceil(number: Integer | Float): Integer](stdlib.md#ceilnumber-integer--float-integer--float)
- [floor(number: Integer | Float): Integer](stdlib.md#floornumber-integer--float-integer--float)
- [BlockHitResult](stdlib.md#blockhitresult)
- [World.breakBlock(pos: BlockPos, drop_items: Boolean): Boolean](stdlib.md#breakblockpos-blockpos-drop_items-boolean-null)
- [World.getBlock(pos: BlockPos): Block](stdlib.md#getblockpos-blockpos-block)
- [List.append(object: Object): Null](stdlib.md#appendobject-object-null)

### Changed

- `events.onPlayerBreakBlock(function: Function[Boolean, PlayerEntity, Block]): Null` is
  now `events.onPlayerBreakBlock(function: Function[Boolean, PlayerEntity, BlockPos, Block]): Null`
- `World.setBlock` renamed to `World.placeBlock`
- `maxArguments` renamed to `maxArgumentCount`

### Fixed

- String concatenation
- Event registration not clearing on reload

### Improved

- Error messages