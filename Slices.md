# Go Slices
Slices are similar to arrays, but are more powerful and flexible.

Like arrays, slices are also used to store multiple values of the same type in a single variable.

However, unlike arrays, the length of a slice can grow and shrink as you see fit.

In Go, there are several ways to create a slice:

- Using the []datatype{values} format
- Create a slice from an array
- Using the make() function
- Create a Slice With []datatype{values}
### Syntax
`slice_name := []datatype{values}`

A common way of declaring a slice is like this:

`myslice := []int{}`

The code above declares an empty slice of 0 length and 0 capacity.

To initialize the slice during declaration, use this:

`myslice := []int{1,2,3}`

The code above declares a slice of integers of length 3 and also the capacity of 3.

In Go, there are two functions that can be used to return the length and capacity of a slice:

- len() function - returns the length of the slice (the number of elements in the slice)
- cap() function - returns the capacity of the slice (the number of elements the slice can grow or shrink to)
### Example
This example shows how to create slices using the []datatype{values} format:
``` go
package main
import ("fmt")

func main() {
  myslice1 := []int{}
  fmt.Println(len(myslice1))
  fmt.Println(cap(myslice1))
  fmt.Println(myslice1)

  myslice2 := []string{"Go", "Slices", "Are", "Powerful"}
  fmt.Println(len(myslice2))
  fmt.Println(cap(myslice2))
  fmt.Println(myslice2)
}
```

## Create a Slice From an Array
You can create a slice by slicing an array:

### Syntax
`var myarray = [length]datatype{values} // An array`

`myslice := myarray[start:end] // A slice made from the array`
### Example
This example shows how to create a slice from an array:
``` go
package main
import ("fmt")

func main() {
  arr1 := [6]int{10, 11, 12, 13, 14,15}
  myslice := arr1[2:4]

  fmt.Printf("myslice = %v\n", myslice)
  fmt.Printf("length = %d\n", len(myslice))
  fmt.Printf("capacity = %d\n", cap(myslice))
}
```

## Create a Slice With The make() Function
The make() function can also be used to create a slice.

### Syntax
`slice_name := make([]type, length, capacity)`

Note: If the capacity parameter is not defined, it will be equal to length.

### Example
This example shows how to create slices using the make() function:
``` go
package main
import ("fmt")

func main() {
  myslice1 := make([]int, 5, 10)
  fmt.Printf("myslice1 = %v\n", myslice1)
  fmt.Printf("length = %d\n", len(myslice1))
  fmt.Printf("capacity = %d\n", cap(myslice1))

  // with omitted capacity
  myslice2 := make([]int, 5)
  fmt.Printf("myslice2 = %v\n", myslice2)
  fmt.Printf("length = %d\n", len(myslice2))
  fmt.Printf("capacity = %d\n", cap(myslice2))
}
```

## Access Elements of a Slice
You can access a specific slice element by referring to the index number.

In Go, indexes start at 0. That means that [0] is the first element, [1] is the second element, etc.

### Example
This example shows how to access the first and third elements in the prices slice:
``` go
package main
import ("fmt")

func main() {
  prices := []int{10,20,30}

  fmt.Println(prices[0])
  fmt.Println(prices[2])
}
```

## Change Elements of a Slice
You can also change a specific slice element by referring to the index number.

### Example
This example shows how to change the third element in the prices slice:
``` go
package main
import ("fmt")

func main() {
  prices := []int{10,20,30}
  prices[2] = 50
  fmt.Println(prices[0])
  fmt.Println(prices[2])
}
```

## Append Elements To a Slice
You can append elements to the end of a slice using the append()function:

### Syntax
`slice_name = append(slice_name, element1, element2, ...)`

### Example
This example shows how to append elements to the end of a slice:
``` go
package main
import ("fmt")

func main() {
  myslice1 := []int{1, 2, 3, 4, 5, 6}
  fmt.Printf("myslice1 = %v\n", myslice1)
  fmt.Printf("length = %d\n", len(myslice1))
  fmt.Printf("capacity = %d\n", cap(myslice1))

  myslice1 = append(myslice1, 20, 21)
  fmt.Printf("myslice1 = %v\n", myslice1)
  fmt.Printf("length = %d\n", len(myslice1))
  fmt.Printf("capacity = %d\n", cap(myslice1))
}
```
