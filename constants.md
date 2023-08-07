# Go Constants

If a variable should have a fixed value that cannot be changed, you can use the `const` keyword.

The `const` keyword declares the variable as "constant", which means that it is unchangeable and read-only.

## Syntax

``` go
const CONSTNAME type = value
```

# Declaring a Constant

Here is an example of declaring a constant in Go:

## Example

``` go
package main

import (
    "fmt"
)

const PI = 3.14

func main() {
    fmt.Println(PI)
}
```
