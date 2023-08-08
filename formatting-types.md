# Go Formatting Verbs

Formatting Verbs for `Printf()`
Go offers several formatting verbs that can be used with the `Printf()` function.

# General Formatting Verbs

The following verbs can be used with all data types:

| Verb | Description |
| ---- | ----------- |
| `%v` | Prints the value in the default format |
| `%#v` | Prints the value in Go-syntax format |
| `%T` | Prints the type of the value |
| `%%` | Prints the % sign |

## Example

```go
package main

import (
    "fmt"
)

func main() {
    var i = 15.5
    var txt = "Hello World!"

    fmt.Printf("%v\n", i)
    fmt.Printf("%#v\n", i)
    fmt.Printf("%v%%\n", i)
    fmt.Printf("%T\n", i)

    fmt.Printf("%v\n", txt)
    fmt.Printf("%#v\n", txt)
    fmt.Printf("%T\n", txt)
}
```

# Integer Formatting Verbs

The following verbs can be used with the integer data type:

| Verb   | Description                                  |
| ------ | -------------------------------------------- |
| `%b`   | Base 2                                       |
| `%d`   | Base 10                                      |
| `%+d`  | Base 10 and always show sign                 |
| `%o`   | Base 8                                       |
| `%O`   | Base 8, with leading 0o                      |
| `%x`   | Base 16, lowercase                           |
| `%X`   | Base 16, uppercase                           |
| `%#x`  | Base 16, with leading 0x                     |
| `%4d`  | Pad with spaces (width 4, right justified)   |
| `%-4d` | Pad with spaces (width 4, left justified)    |
| `%04d` | Pad with zeroes (width 4)                    |

## Example

```go
package main

import (
    "fmt"
)

func main() {
    var i = 15

    fmt.Printf("%b\n", i)
    fmt.Printf("%d\n", i)
    fmt.Printf("%+d\n", i)
    fmt.Printf("%o\n", i)
    fmt.Printf("%O\n", i)
    fmt.Printf("%x\n", i)
    fmt.Printf("%X\n", i)
    fmt.Printf("%#x\n", i)
    fmt.Printf("%4d\n", i)
    fmt.Printf("%-4d\n", i)
    fmt.Printf("%04d\n", i)
}
```
