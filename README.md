# Strings Lab 1

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit

## Question 1

Write code that prints out all the numbers from 1 to 10 as a single string.
(Hint: the `String()` function can convert an Int to a String)

``` swift
var emptyString = " "

var x = 1...10
for i in x{
emptyString = emptyString + "\(i)" + " "
}
print (emptyString)

```

***
## Question 2

Write code that prints out all the even numbers from 5 to 51 as a single string.
``` swift 
var emptyString = " "

var x = 5...51
for i in x{
if i % 2 == 0{
emptyString = emptyString + "\(i)" + " "
}
}
print (emptyString)

```

***
## Question 3

Write code that prints out every number ending in 4 between 1 and 60 as a single string.

``` swift
var x = 1...60
for i in x{
if i % 10 == 4 {
emptyString = emptyString + "\(i)" + " "
}
}
print (emptyString)
```


***
## Question 4

Print each character in the string `"Hello world!"`
``` Swift
var greet = "Hello World"


for i in greet {
print (i)
}
```

***
## Question 5

Print out the last character in the string below.  You cannot use the Character literal "!" (i.e you must access `myStringSeven`'s characters).

`let myStringSeven = "Hello world!"`

``` swift
let myStringSeven = "Hey Buddy"

print (myStringSeven[myStringSeven.index(before: myStringSeven.endIndex)])
```
***
## Question 6

Write code that switches on a string, given the following conditions:
- If the string's length is even, print out every character.
- If the string's length is odd, print out every other character.

``` swift
var greet = "hello poppet0"
var evenOrOdd = 2
if greet.count % 2 == 0{
print(greet)
}
else {
for i in greet{
if evenOrOdd % 2 == 1{
print (i, terminator: "")
}
evenOrOdd += 1
}
}
```

***
## Question 7

Initialize a String with a character. Show that it is a Character, and not another String, that you're using to initialize it.

***
## Question 8

Build five pairs of **canonically equivalent** strings, the first of each being a pre-composed character and the second being one that uses combinable unicode scalars. Show that they are equivalent.

***
## Question 9

**Using only Unicode**, print out `"HELLO WORLD!"`
```
var greet =  "\u{0048}"+"\u{0045}"+"\u{004c}"+"\u{004c}"+"\u{004f}"+" "+"\u{0057}"+"\u{004f}"+"\u{0052}"+"\u{004c}"+"\u{0044}"

print(greet)
```

***
## Question 10

**Using only Unicode**, print out your name.
```
var name = "\u{0054}" + "\u{0049}"+"\u{0041}"+" "+" \u{004C}"+"\u{0045}"+"\u{004e}"+"\u{0044}"+"\u{004f}"+"\u{0052}"

print (name)

```

***
## Question 11

**Using only Unicode**, print out `"HELLO WORLD!"` in another language.
```
var greet = "\u{0042}\u{004f}\u{004e}\u{004a}\u{004f}\u{0055}\u{0052} \u{004c}\u{0045} \u{004d}\u{004f}\u{004e}\u{0044}\u{0045}"

print (greet)
```


***
## Question 12

Print the below flower box using the following information.

- The unicode number for ⚘ is U-2698
- The top and bottom of the box are represented by dashes and the rows are |
- Use the terminator argument in your print statements to print on the same line.
- Hint: It may be useful to try printing out a box of just one character to start then work your way from there.

```swift
Flower Box:
- - - - - - - - - - -
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
| ⚘ | ⚘ | ⚘ | ⚘ | ⚘ |
- - - - - - - - - - -
```
```swift
var flowerRow = 1...7
var flowerBox = "| \u{2698} | \u{2698} | \u{2698} | \u{2698} | \u{2698} | "
var woodenBox = "- - - - - - - - - - -"
print (woodenBox)
for i in flowerRow{
print (flowerBox)
}
print (woodenBox)
```

***
## Question 13

Write a program that sets up a chess board using Unicode.

```swift
Chess Board:
♖ ♘ ♗ ♕ ♔ ♗ ♘ ♖
♙ ♙ ♙ ♙ ♙ ♙ ♙ ♙




♟ ♟ ♟ ♟ ♟ ♟ ♟ ♟
♜ ♞ ♝ ♛ ♚ ♝ ♞ ♜
```
```
var chessRoyalsLight = "\u{2656} \u{2658} \u{2657} \u{2655} \u{2654} \u{2657} \u{2658} \u{2656}"
var chessPawnsLight = "\u{2659} \u{2659} \u{2659} \u{2659} \u{2659} \u{2659} \u{2659} \u{2659}"
var chessPawnsDark = "\u{265f} \u{265f} \u{265f} \u{265f} \u{265f} \u{265f} \u{265f} \u{265f}"
var chessRoyalsDark = "\u{265c} \u{265e} \u{265d} \u{265a} \u{265b} \u{265d} \u{265e} \u{265c}"
print (chessRoyalsLight)
print (chessPawnsLight)
print (" ")
print (" ")
print (" ")
print (" ")
print (chessPawnsDark)
print (chessRoyalsDark)

```
***
## Question 14

You are given a string stored in the variable `aString`. Create new string named `replacedString` that contains the characters of the original string with all the occurrences of the character `"e"` replaced by `"\*"`.

```swift
var aString = "Replace the letter e with \*"
// Your code here
 ```
 ```
 var aString = "Replace the letter e with *"
 
 var newString = aString.replacingOccurrences(of: "e", with: "*")
 print(newString)
 ```

Example:

Input:
`var aString = "Replace the letter e with *"`

Expected values:
`replacedString = "R*plac* th* l*tt*r * with *"`

***
## Question 15

You are given a string stored in variable `aString`. Create a new string called `reverse` that contains the original string in reverse order. Print the reversed string.

```swift
var aString = "this string has 29 characters"
var reverse = ""

// var aString = "la, la, dee dah dee"
var reversed = String (aString.reversed())
print (reversed)
```


Example:
Input:
`var aString = "Hello"`

Output:
`"olleH"`

***
## Question 16

You are given a string stored in variable `aString`. Print `true` if `aString` is a palindrome, and `false` otherwise. A **palindrome** is a string which reads the same backward or forward.

```swift
let aString = "anutforajaroftuna"

// let aString = "anutforajaroftuna"
var reversed = String (aString.reversed())

if aString == reversed{
print (true)
}
else{
print(false)
}
```

Example 1:
Input:
`var aString = "anutforajaroftuna"`

Output:
`true`

Example 2:
Input:
`var aString = "Hello"`

Output:
`false`

***
## Question 17

You are given a string stored in variable `problem`. Write code so that you print each word of the string on a new line.

```swift
var problem = "split this string into words and print them on separate lines"

//var problem = "split this string into words and print them on separate lines"
var newProblem = problem.replacingOccurrences(of: " ", with: "\n")

print(newProblem)
```

Example:
Input:
`var problem ="split this string into words and print them on separate lines"`

Output:
```swift
split
this
string
into
words
and
print
them
on
separate
lines
```

***
## Question 18

You are given a string stored in variable `problem`. Write code that prints the longest word in the string.

```swift
var problem = "find the longest word in the problem description"

// var problem = "find the longest word in the problem description"
var word = problem.split(separator: " ")
var longWord = ""

for i in word{
if i.count >= longWord.count {
longWord = String(i)
}
}
print(longWord)
```

Example:
Input:
`var problem = "find the longest word in the problem description"`

Output:
`description`

Hint: Keep track of the longest word you encounter and also keep track of its length.

***
## Question 19

Given a string in English, create a tuple containing the number of vowels and consonants.

```swift
let vowels = "aeiou"
let consonants = "bcdfghjklmnpqrstvwxyz"
let input = "Count how many vowels I have!"
```
```
let vowels = "aeiou"
let consonants = "bcdfghjklmnpqrstvwxyz"
let input = "Count how many vowels I have!"

var quest19 = (vowels: "\(vowels.count)", consonants: "\(consonants.count)")

print (quest19)
```

***
## Question 20

Given a string of words separated by a `" "`. Write code that prints out the length of the last word.

If there is no last word print out `"No last word"`.

Example:
Input: `"How are you doing this Monday?"`

Output: `7`

```
var quest20 = "How are you doing this Monday?"
var word = quest20.split(separator: " ")

if word.count > 0{
print (word.last!.count)
}
else {
print ("No last word")
}
```

***
