# Go Data Types

Data type is an important concept in programming. A data type specifies the size and type of variable values.

Go is statically typed, meaning that once a variable type is defined, it can only store data of that type.

Go has three basic data types:

- `bool`: represents a boolean value and is either true or false
- `Numeric`: represents integer types, floating-point values, and complex types
- `string`: represents a string value

## Example

This example shows some of the different data types in Go:

```go
package main

import (
    "fmt"
)

func main() {
    var a bool = true     // Boolean
    var b int = 5         // Integer
    var c float32 = 3.14  // Floating-point number
    var d string = "Hi!"  // String

    fmt.Println("Boolean: ", a)
    fmt.Println("Integer: ", b)
    fmt.Println("Float:   ", c)
    fmt.Println("String:  ", d)
}
```

# Boolean Data Type

A boolean data type is declared with the `bool` keyword and can only take the values `true` or `false`.

The default value of a boolean data type is `false`.

## Example

This example shows different ways to declare Boolean variables:

```go
package main

import (
    "fmt"
)

func main() {
    var b1 bool = true      // Typed declaration with initial value
    var b2 = true           // Untyped declaration with initial value
    var b3 bool             // Typed declaration without initial value
    b4 := true              // Untyped declaration with initial value

    fmt.Println(b1)         // Returns true
    fmt.Println(b2)         // Returns true
    fmt.Println(b3)         // Returns false
    fmt.Println(b4)         // Returns true
}
```

# Go Integer Data Types

Integer data types are used to store a whole number without decimals, like 35, -50, or 1345000.

The integer data type has two categories:

- Signed integers: can store both positive and negative values
- Unsigned integers: can only store non-negative values

**Tip:** The default type for integer is `int`. If you do not specify a type, the type will be `int`.

# Signed Integers

Signed integers, declared with one of the `int` keywords, can store both positive and negative values.

## Example

```go
package main

import (
    "fmt"
)

func main() {
    var x int = 500
    var y int = -4500
    fmt.Printf("Type: %T, value: %v\n", x, x)
    fmt.Printf("Type: %T, value: %v\n", y, y)
}
```
