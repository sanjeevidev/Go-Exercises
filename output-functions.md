# Go Output Functions

Go has three functions to output text:

- `Print()`
- `Println()`
- `Printf()`

## The Print() Function

The `Print()` function prints its arguments with their default format.

### Example

Print the values of `i` and `j`:

```go
package main

import (
    "fmt"
)

func main() {
    var i, j string = "Hello", "World"

    fmt.Print(i)
    fmt.Print(j)
}
```
