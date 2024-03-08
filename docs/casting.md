# Casting

Casting types is a fundamental part of statically typed programming languages.

## Upcasting

```dart
class Base {}

class Super extends Base {}

var x: Base = Super();

print(type(x)); // Base (not Super!)
```

## Downcasting

```dart
class Base {}

class Super extends Base {}

var x: Base = Super();

var y = (Super) x;

print(type(y)); // Super
```