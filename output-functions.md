# Go Output Functions

Go has three functions to output text:

- `Print()`
- `Println()`
- `Printf()`

# The Print() Function

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

## Example

If we want to print the arguments on new lines, we can use the `\n` escape sequence.

```go
package main

import (
    "fmt"
)

func main() {
    var i, j string = "Hello", "World"

    fmt.Print(i, "\n")
    fmt.Print(j, "\n")
}
```

# The Println() Function

The `Println()` function is similar to `Print()` with the difference that a whitespace is added between the arguments, and a newline is added at the end.

### Example

```go
package main

import (
    "fmt"
)

func main() {
    var i, j string = "Hello", "World"

    fmt.Println(i, j)
}
```
