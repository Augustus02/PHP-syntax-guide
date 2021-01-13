
# PHP Syntax Guide

## PHP Comments
### To comment out a single line you can use both // and .# 
#### ignore the . infront of .#
#### EXAMPLE

1.  // this is commented out
 
2.  .# this is also commented out

### To comment out multiple lines you can use /* */
#### EXAMPLE

/*
this text is commented out
 
this is also commented out
*/

## PHP Variables
Variables are used to store data types.
Once a variable has been declared you can then use it throughout your script.
All variables must begine with a $

#### EXAMPLE

$demo = "Hello World";
 
echo $demo;

## PHP Echo / Print
Echo and print are both used to display data onto the screen.
Echo has no return value while print returns 1.
Echo is a little faster then print.
Echo can take multiple arguments while print can only take 1.
You can display strings, variables, and inbed HTML into it.
#### EXAMPLE
$test = "variable";
 
echo "string";
 
echo $test;
 
## PHP Data Types

#### Strings
A string is any kind of text inside of either double or single quotes.
##### EXAMPLE
$demo = "this is a string";
 
echo $demo;

#### Integer
An integer is a non-decimal negative or positive number.
##### EXAMPLE
$demo = 10;
 
echo $demo;

#### Floating point number
Floating point numbers are decimal or fractional numbers.
##### EXAMPLE
$demo = 1.987;
 
echo $demo;
#### Boolean
A boolean is a TRUE or FALSE statement.
##### EXAMPLE
$demo = true;

#### Array
An array is a variable that can store multiple values.
##### EXAMPLE
$colours = ("blue","green","red","yellow");
 
var_dump($colours);

#### Object
An object data structure that stores pairs of data.

#### NULL
An empty variable is represented by the value NULL.
##### EXAMPLE
$demo = NULL;
 
var_dump($demo);

#### Resource
A resource is a variable holding references to external resources like a database or an open file.
##### EXAMPLE
$demo = fopen("test.txt", "r");
 
var_dump($demo);

## PHP Constants
A constant has a value that can't be changed.
it is written like define(name, value);
##### EXAMPLE
define("demo", "test");
 
var_dump(demo);
## PHP Operators
There are many different kinds of operators that perform operations on variables and values.
##### EXAMPLE OF JUST 2 OF MANY
addition $x + $y
 
subtraction $x - $y

## PHP If & Else & Elseif
The if statement runs the code inside if the condition is true.
The else statement goes after an if and runs the code inside if the if condition is false.
elseif chains if and else together and runs code for more than two conditions.
##### EXAMPLE
###### if and else
$demo = 10;
 
// if
 
if($demo == 10) {
 
echo "Hello World";
 
}
 
// else
 
else {
 
echo "change the demo number to 10";
 
}

###### elseif
$price = 10;
 

if($price < 25) {
 
  echo "change the price to be higher than 25";
   
} elseif($price < 50) {
 
  echo "change the price to be higher than 50";
   
} elseif ($price < 75) {
 
  echo "change the price to be higher than 75";
   
} elseif($price < 100) {
 
  echo "change the price to be higher than 100";
   
} else {
 
  echo "this is a good price";
   
}

## PHP Functions
There are many built in functions for php, there are also User-Defined functions.
User-Defined functions allow you to create your own reusable code that can perform specific tasks
##### EXAMPLE
function test(){
 
echo "the function worked";
 
}
 
test();

## PHP Loop
Loops continue to run the same code as long as the condition is true.
There are 4 different loops. While, Do while, for, and foreach.
##### EXAMPLE
###### while 
$number = 10;
 
while($number > 0){
    $number--;
    echo $number;
}
###### Do while
$number = 10;
do{
    $number--;
    echo $number;
}
while($number > 0);
###### For: for loops take 3 parameters
for($number=10; $number > 0; $number--){
    echo $number;
}
###### foreach
$food = array("steak", "chicken", "soup");
 
foreach($food as $value){
    echo $value;
}



