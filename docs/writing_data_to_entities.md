# Writing Data to Entities

When reading/writing data to an entity you have to make sure it is an nbt element. That means you can not store custom classes on entities. This code would not work.

```dart
class Foo {

}

entity["my_data"] = Foo();
```

## Writing Data

```dart
entity["my_data"] = 1;
```

`my_data` is now stored in the entities nbt in `custom_data.my_data`.

## Reading Data

```dart
entity["my_data"] = 1;

var my_data = entity["my_data"];

print(my_data); // 1
```

## Valid NBT Elements

- `Float`
- `Integer`
- `List` (Every element has to be the same type)
- `String`
- `Dictionary`

Otherwise you will get the error `Type <class type> is not part of Minecraft NBT`.
