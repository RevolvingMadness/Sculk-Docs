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