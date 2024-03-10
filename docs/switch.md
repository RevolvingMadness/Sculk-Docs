# Switch

## Switch Statement

```dart title="load.sk"
var x = 1;

switch (x) {
    case 1 {
        print("x is one");
    }
    case 2 -> print("x is two");
    default {
        print("idk");
    }
}
```

# Switch Expression

```dart title="load.sk"
var x = 1;

function toString(x) -> String {
    return switch (x) {
        case 1 -> "one";
        case 2 -> "two";
        case 3 {
            print("x is three");
            
            yield "three";
        }
        default -> "idk";
    };
}

print(toString(x)); // one
```