# Import Statement

To import a script type the following syntax.

```dart title="bar.sk"
var a = 1;
var b = 2;
var c = 3;
```

```dart title="load.sk"
import foo:bar;

print(a); // 1
print(b); // 2
```

## From Statement

```dart title="bar.sk"
var a = 1;
var b = 2;
var c = 3;
```

```dart title="load.sk"
from foo:bar import a;

print(a); // 1
print(b); // Error
```