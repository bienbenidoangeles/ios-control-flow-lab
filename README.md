# Control Flow Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit

## Question 1

What will be printed when the code below is run?  Select all that apply.

```swift
let conditionOne = !(4 < 5) || !(3 > 8)
let conditionTwo = !(!true)

if conditionOne {
 print("A")
} else if conditionTwo {
 print("B")
}
if conditionTwo {
 print("C")
}
print("D")
```

- A
- B
- C
- D

"A", "C", and "D" will be printed

***
## Question 2

What will the code block below print?  Select all that apply:

```swift
let appInfo = (name: "myCoolApp", version: 0.4)
switch appInfo {
 case (_, 0.0..<1.0):
 print("\(appInfo.0) hasn't released yet")
 case ("myCoolApp", _):
 print("Thanks for looking at myCoolApp!")
 default:
 print("I'm not quite sure what you are looking at")
}
```

- appInfo.0 hasn't released yet
- myCoolApp hasn't released yet
- Thanks for looking at myCoolApp!
- I'm not quite sure what you are looking at
- It will give a compile-time error

It will print below:
"myCoolApp hasn't released yet"

***
## Question 3

What will be printed to the console when the code below is run?  Select all that apply.

```swift
let x: Int = 4
switch x {
case 0..<4:
 print("A")
case 5..<10:
 print("B")
case is Double:
 print("C")
default:
 print("D")
}
```

- A
- B
- C
- D

"D" will be printed to the console.

***
## Question 4

What are the errors in the code below for the switch statement? Select all that apply.

```swift
let candyType : String = "skittles"

switch candyType {
case "mAndM":
 print("Melts in your mouth, not in your hand")
case "skittles":
 print("Taste the rainbow")
case "snickers":
 print("Hungry? Grab a Snickers")
}
```

- No parentheses around the conditions
- No opening and closing brackets in each of the cases
- No default case in the switch statement
- No print statement right outside the switch statement

No default case in the switch statement

***
## Question 5

Given the current weather conditions (rain, sunny, snow), use a switch statement to print an appropriate message to the user

```swift
let currentWeather = "rain"

// enter code below
```

My code:
```swift
let message = "The current weather is "
switch currentWeather {
case "rain": 
    print(message + currentWeather)
case "sunny":
    print(message + currentWeather)
case "snow":
    print(message + currentWeather)
}
"
```

***
## Question 6

Given the first name and last name of a Fellow, declare `fullName` variable and use string interpolation to concatenate the Fellow's full name and print to the console e.g The Fellow's full name is John Appleseed

```swift
let firstName = "John"
let lastName = "Appleseed"

// enter code below
```
My code:
```swift
let fullName = firstName + lastName
print("The Fellow's full name is \(fullName)")
```

***

## Question 7

Convert the if/else statement below into a switch statement.

```swift
if temperatureInFahrenheit <= 40 {
 print("It's cold out.")
} else if temperatureInFahrenheit >= 85 {
 print("It's really warm.")
} else {
 print("Weather is moderate.")
}

//Re-written statement here

```
My Code:
```swift
var temperatureInFahrenheit:Int
switch temperatureInFarenheit {
case ...40:
    print("It's cold out.")
case 85...:
    print("It's really warm.")
default:
    print("Weather is moderate.")
}
```

***

## Question 8

Complete the following code so that "You win!" is printed.

```swift
if {
 print("You win!")
} 
else {
 print("You lose!")
}
```

My code:
```swift
let aiNum = Int.random(in: 0 ... 10)
if aiNum%2 == 0 {
    print("You win!")
} 
else {
    print("You lose!")
}
```
***

## Question 9

Given a variable called numberOfSides, write code using a switch so that it prints out the name of the shape. Account for shapes with 3 to 10 sides and print an error message if out of range.

var numberOfSides = 6

```swift
Example 1:

Input:
var numberOfSides = 4

Output:
Square

Example 2:

Input:
var numberOfSides = 2

Output:
Error

```

My code:
```swift

let var message = "Error"
switch numberOfSides {
case 3...10:
    if numberOfSides == 3 {
        print("Triangle")
    }
    else if numberOfSides == 4 {
        print("Square")
    }
    else if numberOfSides == 5 {
        print("Pentagon")
    }
    else if numberOfSides == 6 {
        print("Hexagon")
    }
    else if numberOfSides == 7 {
        print("Heptagon")
    }
    else if numberOfSides == 8 {
        print("Octagon")
    }
    else if numberOfSides == 9 {
        print("Nonagon")
    }
    else if numberOfSides == 10 {
        print("Decagon")
    }
default:
    print(message)
}
```

***

## Question 10

Create a switch statement that will convert a number grade into a letter grade as shown below:

```swift
Numeric Score 	Letter Grade
100 	A+
90 - 99	A
80 - 89	B
70 - 79 	C
65 - 69 	D
Below 65 	F
```
My code:

```swift

var letterGrade:Character
let numbericScore:ClosedInterval = 65...100

switch numbericScore {
    case 100:
        letterGrade = "A+"
    case 90...99:
        letterGrade = "A"
    case 80...89:
        letterGrade = "B"
    case 70...79:
        letterGrade = "C"
    case 65...69:
        letterGrade = "D"
    default:
        letterGrade = "F"
}
```
***

## Question 11

What is wrong with the block of code below?  Correct it so it behaves as expected.

```swift
let firstName = "Peter"

if firstName == "Peter" {
 let lastName = "Gabriel"
} else if firstName == "Phil" {
 let lastName = "Collins"
}
let fullName = firstName + " " + lastName
```
1.The variable lastName is not initialized before being used for fullName <br/>
1.lastName is declared as an immutable datatype within a local scope of the the if-else control flow sequence

My code:
```swift
let firstName = "Peter"
var lastName:String = ""

if firstName == "Peter" {
 lastName = "Gabriel"
} else if firstName == "Phil" {
 lastName = "Collins"
}
let fullName = firstName + " " + lastName
```
***

## Question 12

Write an if statement that prints out what decade of life someone is in (e.g "You are in your twenties). Then, write it as a switch statement.

//try to captures 20s,30s,40s
```swift
let nameAndBirthYear: (String, Int)

```

My Code:
```swift
let nameAndBirthYear: (String, Int)
nameAndBirthYear = ("Bienbenido", 1998)
var birthYear = nameAndBirthYear.1
let currentYear = 2019
var age = currentYear - birthYear

if (age >= 20 && age < 30) {
    print("\(nameAndBirthYear.0), you are in your twenties")
} else if (age >= 30 && age < 40) {
    print("\(nameAndBirthYear.0), you are in your thirties")
} else if (age >= 40 && age < 50) {
    print("\(nameAndBirthYear.0), you are in your fourties")
}

switch age {
case 20..<30:
    print("\(nameAndBirthYear.0), you are in your twenties")
case 30..<40:
    print("\(nameAndBirthYear.0), you are in your twenties")
case 40..<50:
    print("\(nameAndBirthYear.0), you are in your twenties")
default:
    print("\(nameAndBirthYear.0), you are \(age1) years old")
}
```
***


## Question 13

Consider the below switch statement. What should your system currently print?

```swift
let number = 42

switch number {
case 365:
 print("Days in year")
case 1024:
 print("Bytes in a Kilobyte")
case 0:
 print("Where arrays start")
case 42:
 print("The answer to life, the universe and everything")
default:
 print("Some uninteresting number")
```
What happens when you change number to:

-a. 365?
<br/>
it will print "Days in year" </br>
-b. 1024?
<br/>
it will print "Bytes in a kilobyte" </br>
-c. 65?
<br/>
it will print "Some uninteresting number" </br>

What happens when you remove the default clause?
The switch control flow statement will not compile as the variable number is not finite

***


## Question 14

Consider the variable below called population and the if-condition.

a. Add an else-if-condition that states if population is less than 10000 but greater than 5000, then message changes to say it's "a medium size town".

b. Add an else-condition where message changes to say it's a mid-size town.

c. Convert your final if-else statement to a switch statement.

```swift
var population: Int = 10000
var message = String()

if population > 10000 {
 message = "\(population) is a large town"
}
```
My code:

```swift
var population: Int = 10000
var message = String()

if population > 10000 {
 message = "\(population) is a large town"
} else if population < 10000 && population > 5000 {
 message = "\(population) is a medium size town"
} else {
 message = "\(population) It's a medium size town"
}

switch population {
case 10000...:
    message = "\(population) is a large town"
case 5000..<10000:
    message = "\(population) is a medium size town"
default:
    message = "\(population) is a medium size town"
}
```
***

## Question 15

Complete the code below so that it prints out and tells the user if the sum of the two numbers in the tuple is at least 15.

a. Using a conditional

b. Using a switch statement

```swift
let myTuple: (Int, Int) = (5, 10)

```

My code:

```swift
let myTuple: (Int, Int) = (5, 10)
let sum = myTuple.0 + myTuple.1

if (sum >= 15){
    print("\(myTuple) the sum of those numbers are at least 15")
}

switch sum {
case 15...:
    print("\(myTuple) the sum of those numbers are at least 15")
default:
    print("\(myTuple) the sum of those numbers are not at least 15")
}
```
***
