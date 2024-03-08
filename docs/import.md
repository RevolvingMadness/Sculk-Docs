# Import Statement

The import statement allows you to use code across multiple files.

```dart title="foo:bar"
var a = 1;
var b = 2;
```

```dart title="foo:load"
import "foo:bar";

print(a); // 1
print(b); // 2
print(c); // Error
```

## From Statement

```dart title="foo:bar"
var a = 1;
var b = 2;
var c = 3;
```

```dart title="foo:load"
from "foo:bar" import a, b;

print(a); // 1
print(b); // 2
print(c); // Error
```