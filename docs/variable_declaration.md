# Variable Declaration

## Declaring a Variable

### With a Value

```java
var x: Integer = 1;
print(x); // 1
```

The type of a variable can be optionally be ignored.

```java
var x = 1;
print(x); // 1
```

### Without a Value

If you don't specify a value, the variable defaults to [Null](stdlib.md#null).

```java
var x: Integer;
print(x); // null
```

## Assigning a Variable

```java
var x: Integer = 1;
print(x); // 1
x = 2;
print(x); // 2

x = "Invalid type"; // Error
```

## Declaring a Function

### Block

```java
function add(a: Number, b: Number) -> Number {
    print("Adding");
    return a + b;
}

print(add(1, 1));     // 2
print(add(1.5, 1));   // 2.5
print(add(1, 1.5));   // 2.5
print(add(1.5, 1.5)); // 3.0
```

### In-Line

```java
function add(a: Number, b: Number) -> Number => a + b;

print(add(1, 1));     // 2
print(add(1.5, 1));   // 2.5
print(add(1, 1.5));   // 2.5
print(add(1.5, 1.5)); // 3.0
```

## Declaring a Class

### Constructors

```java
class Person {
    function init(name: String, age: Integer) -> Null {
        print(name + " is " + age.toString() + " years old.");
    }
}
```

### Superclasses

```java
class BaseClass {
    function baseMethod() -> Null {
        print("Base Method");
    }
}

class SuperClass extends BaseClass {

}

class SuperClassOverride extends BaseClass {
    function baseMethod() -> Null {
        super.baseMethod(); // Base Method
        print("Super Method");
    }
}

var baseClass = BaseClass();
var superClass = SuperClass();
var superClassOverride = SuperClassOverride();

baseClass.baseMethod(); // Base Method

superClass.baseMethod(); // Base Method

superClassOverride.baseMethod(); // Base Method & Super Method

print(BaseClass() instanceof BaseClass); // true

print(BaseClass() instanceof SuperClass); // false

print(SuperClass() instanceof BaseClass); // true

print(SuperClass() instanceof SuperClass); // true
```

### Abstraction

```java
abstract class Person {
    abstract function getGender() -> String;
}

class Male extends Person {
    function getGender() -> String {
        return "Male";
    }
}

var male = Male();
print(male.getGender());
```

### Fields

```java
class Person {
    var name: String;
    var age: Integer;
    
    function init(name: String, age: Integer) -> Null {
        this.name = name;
        this.age = age;
    }
}
```

### Methods

```java
class Calculator {
    function add(a: Number, b: Number) -> Number {
        return a + b;
    }
}

var calc = Calculator();

print(calc.add(1, 1));     // 2
print(calc.add(1.5, 1));   // 2.5
print(calc.add(1, 1.5));   // 2.5
print(calc.add(1.5, 1.5)); // 3.0
```