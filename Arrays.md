# Go Arrays

Arrays are used to store multiple values of the same type in a single variable, instead of declaring separate variables for each value.

## Declare an Array

In Go, there are two ways to declare an array:

1. With the `var` keyword:

    Syntax:
    `
    var array_name = [length]datatype{values} // here length is defined
    `

    or

    `
    var array_name = [...]datatype{values} // here length is inferred
    `

2. With the `:=` sign:

    Syntax:
    `
    array_name := [length]datatype{values} // here length is defined
    `

    or

    `
    array_name := [...]datatype{values} // here length is inferred
    `

**Note:** The length specifies the number of elements to store in the array. In Go, arrays have a fixed length. The length of the array is either defined by a number or is inferred (meaning that the compiler decides the length of the array based on the number of values).
