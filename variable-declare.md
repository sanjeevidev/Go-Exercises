# Declaring (Creating) Variables
In Go, there are two ways to declare a variable:

<h3 >1. With the var keyword:</h3>
<p>Use the var keyword, followed by variable name and type:</p>

<h4>Syntax</h4>
<p><tt>var variablename type = value</tt><br>
Note: You always have to specify either type or value (or both).</p>

<h3>2. With the := sign:</h3>
<p>Use the := sign, followed by the variable value:</p>

<h4>Syntax</h4>
<p><tt>variablename := value</tt></p>

<h2> Example :</h2>
<i><tt>package main
import ("fmt")
func main() {
  var student1 string = "John" //type is string
  var student2 = "Jane" //type is inferred
  x := 2 //type is inferred
  fmt.Println(student1) #John
  fmt.Println(student2) #Jane
  fmt.Println(x) #2
}</tt></i><br><h2></h2>

<h2>Multiple Variable Declaration</h2>
<p>In Go, it is possible to declare multiple variables in the same line.<br>
<b>Example</b><br>
<h2>Example :</h2></p>

<i><tt>package main
import ("fmt")
func main() {
  var a, b, c, d int = 1, 3, 5, 7
  fmt.Println(a)
  fmt.Println(b)
  fmt.Println(c)
  fmt.Println(d)
}</tt></i>
