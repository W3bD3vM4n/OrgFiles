# Medium

## 11. Return the N-th value of the Fibonacci sequence

### _Code:_

        function fibonacci(n) {
	        // write your solution here

	        return
        }

        console.log(`fibonacci value at position 5: ${fibonacci(5)}`)

### _Challenges (1):_

- function fibonacci(n) returns the N-th value of the Fibonacci sequence
<br/><br/>

## 12. Given a number from 0 to 999,999,999,999, spell out that number in English

### _Instructions:_

Given a number from 0 to 999,999,999,999, spell out that number in English.

**Step 1**

Handle the basic case of 0 through 99.

If the input to the program is 22, then the output should be 'twenty-two'.

Your program should complain loudly if given a number outside the blessed range.

Some good test cases for this program are:

0
14
50
98
-1
100

**Step 2**
Implement breaking a number up into chunks of thousands.

So 1234567890 should yield a list like 1, 234, 567, and 890, while the far simpler 1000 should yield just 1 and 0.

The program must also report any values that are out of range.

**Step 3**
Now handle inserting the appropriate scale word between those chunks.

So 1234567890 should yield '1 billion 234 million 567 thousand 890'

The program must also report any values that are out of range. It's fine to stop at "trillion".

**Step 4**
Put it all together to get nothing but plain English.

12345 should give twelve thousand three hundred forty-five.

The program must also report any values that are out of range.

### _Code:_

        const sayNumberInEnglish = (n /* ADD MORE PARAMETERS IF NEEDED */) => {
	        // Write your solution here

	        return
        }

        console.log(`5635 in english is: ${sayNumberInEnglish(5635)}`)

### _Challenges (2):_

- 14 becomes "fourteen"

- 1323 becomes "one thousand three hundred twenty-three"
<br/><br/>

## 13. Convert given seconds to space age on all planets of our solar system

### _Instructions:_

Given an age in seconds, calculate how old someone would be on:

- Mercury: orbital period 0.2408467 Earth years

- Venus: orbital period 0.61519726 Earth years

- Earth: orbital period 1.0 Earth years, 365.25 Earth days, or 31557600 seconds

- Mars: orbital period 1.8808158 Earth years

- Jupiter: orbital period 11.862615 Earth years

- Saturn: orbital period 29.447498 Earth years

- Uranus: orbital period 84.016846 Earth years

- Neptune: orbital period 164.79132 Earth years

- Pluto is not a planet

So if your function was called with 436575687 as the argument i.e spaceAge(436575687) it should return { "Mercury": 57.44, "Venus": 22.49, "Earth": 13.83, "Mars": 7.36, "Jupiter": 1.17, "Saturn": 0.47, "Uranus": 0.16, "Neptune": 0.08 }

**Important!!**

Your spaceAge function should return the (already given) yearsInAllPlanets object after setting age on each planet (each property of the object)

THE VALUE OF EACH PROPERTY SHOULD BE A NUMBER AND SHOULD HAVE MAXIMUM 2 DIGITS AFTER THE POINT example 4.34

### _Code:_

        const spaceAge = (seconds) => {
        	const yearsInAllPlanets = {
        		Mercury: 0,
        		Venus: 0,
        		Earth: 0,
        		Mars: 0,
        		Jupiter: 0,
        		Saturn: 0,
        		Uranus: 0,
        		Neptune: 0,
        	}

        	// Your solution starts here

        	// Your solution ends here

        	return yearsInAllPlanets
        }

        console.log(spaceAge(Math.round(Math.random() * 99999999)))

### _Challenges (2):_

- function spaceAge(436575687) should return { "Mercury": 57.44, "Venus": 22.49, "Earth": 13.83, "Mars": 7.36, "Jupiter": 1.17, "Saturn": 0.47, "Uranus": 0.16, "Neptune": 0.08 }

- spaceAge(65965561) should return { 'Mercury': 8.68 'Venus': 3.4 'Earth': 2.09 'Mars': 1.11 'Jupiter': 0.18 'Saturn': 0.07 'Uranus': 0.02 'Neptune': 0.01 }
<br/><br/>

## 14. Convert given array of digits of a base to another asked base

### _Instructions:_

Convert a number, represented as a sequence of digits in one base, to any other base.

Implement general base conversion. Given a number in base a, represented as a sequence of digits, convert it to base b.

**Example**

input: convertDigitsToAskedBase([5, 8], 10, 16)

output: [3, 10]

convertDigitsToAskedBase([5, 8], 10, 16) is passed to the convertDigitsToAskedBase function i.e 58 in base 10 as [5, 8] in array is passed and asked to convert to base 16 which is 310. This should be returned in array as [3, 10].

**Note**

[3, 10] is not other than [3, 10] is because 3 and 10 both are valid digits of base 16

[3, 1, 0] is WRONG because even though 1 and 0 are valid digits of base 16 it can be represented as 10 without taking the 3rd place.

### _Code:_

        /**
         *
         * @param {number[]} digits Array of valid digits of baseA
         * @param {number} baseA base a
         * @param {number} baseB base b in which digits are to be converted
         * @returns {number[]} Array of valid digits of baseB
         */
        const convertDigitsToAskedBase = (digits, baseA, baseB) => {
        	// Your code here

        	return
        }

### _Challenges (2)_

- convertDigitsToAskedBase([5, 8], 10, 16) should return [3, 10]

- convertDigitsToAskedBase() with any random value passed should return correct array as asked
<br/><br/>

## 15. Determine if a sentence is a pangram

### _Instructions:_

Determine if a sentence is a pangram. A pangram (Greek: παν γράμμα, pan gramma, "every letter") is a sentence using every letter of the alphabet at least once. The best known English pangram is:

The quick brown fox jumps over the lazy dog.

The alphabet used consists of ASCII letters a to z, inclusive, and is case insensitive. Input will not contain non-ASCII symbols.

### _Code:_

        const isPangram = (input) => {
        	// Code here

        	return
        }


- Determine if a sentence is a pangram

- Determine if a sentence is a pangram
<br/><br/>

## 16. Ask the Bob

### _Instructions:_

Bob is a lackadaisical teenager. In conversation, his responses are very limited.

Bob answers 'Sure.' if you ask him a question, such as "How are you?".

He answers 'Whoa, chill out!' if you YELL AT HIM (in all capitals).

He answers 'Calm down, I know what I'm doing!' if you yell a question at him.

He says 'Fine. Be that way!' if you address him without actually saying anything.

He answers 'Whatever.' to anything else.

Bob's conversational partner is a purist when it comes to written communication and always follows normal rules regarding sentence punctuation in English.

### _Code:_

        function hey(message) {
        	// Code here

        	return
        }

### _Challenges (2):_

- Any random string will be passed, it should work as asked

- Any random string will be passed, it should work as asked
<br/><br/>

## 17. Longest Consecutive Sequence

### _Instructions:_

Given an array of elements, find a subsequence in the array such that all the elements in the sequence are consecutive irrespective of their order.

**Example**

_Input:_ [100,4,200,1,3,2]

_Output:_ 4 // LCS [1, 2, 3, 4]

Conceptually this is how it should work.

Copy all the elements of the array in a set. Iterate the array and in each iteration determine if the current element will lead to new subsequence by checking if there is no element less than the current, present in the set. Then find how long this subsequence can be by incrementing the count till there is consecutive elements in the set. In the end return the longest consecutive sequence.

### _Code:_

        /**
         *
         * @param {number[]} inputArray Array of numbers
         */
        const longestConsecutiveSequence = (inputArray) => {
        	// Your code here

        	return
        }

### _Challenges (2):_

- longestConsecutiveSequence([100,4,200,1,3,2]) returns 4

- longestConsecutiveSequence([0,3,7,2,5,8,4,6,0,1]) returns 9
<br/><br/>

## 18. Calculate Grains on a given square on a chessboard

### _Instructions:_

Calculate the number of grains of wheat on a chessboard given that the number on each square doubles.

There once was a wise servant who saved the life of a prince. The king promised to pay whatever the servant could dream up. Knowing that the king loved chess, the servant told the king he would like to have grains of wheat. One grain on the first square of a chess board, with the number of grains doubling on each successive square.

There are 64 squares on a chessboard (where square 1 has one grain, square 2 has two grains, and so on).

Write code that shows:

How many grains were on a given square
Total number of grains that can exist on the chessboard given the condition

**Note**

Answer sould be a BigInt value

Both function is given to you separate and you should write code in both functions

### _Code:_

        const totalGrains = () => {
        	// Code here

        	return
        }

        const grainsOn = (input) => {
        	// Code here

        	return
        }

        console.log(`Grains on 5th square: ${grainsOn(5)}`)
        console.log(`Total grains upto 5th square: ${totalGrains(5)}`)

### _Challenges (2):_

- How many grains were on a given square

- Total number of grains that can exist on the chessboard given the condition
<br/><br/>

## 19. Resistor Color map

### _Instructions:_

If you want to build something using a Raspberry Pi, you'll probably use resistors. For this exercise, you need to know two things about them:

Each resistor has a resistance value.
Resistors are small - so small in fact that if you printed the resistance value on them, it would be hard to read.
To get around this problem, manufacturers print color-coded bands onto the resistors to denote their resistance values. Each band has a position and a numeric value.

The first 2 bands of a resistor have a simple encoding scheme: each color maps to a single number.

In this exercise you are going to create a helpful program so that you don't have to remember the values of the bands.

These colors are encoded as follows:

Black: 0
Brown: 1
Red: 2
Orange: 3
Yellow: 4
Green: 5
Blue: 6
Violet: 7
Grey: 8
White: 9

The goal of this exercise is to create a way:

to look up the numerical value associated with a particular color band
to list the different band colors
Mnemonics map the colors to the numbers, that, when stored as an array, happen to map to their index in the array: Better Be Right Or Your Great Big Values Go Wrong.

**Note**

Although the color names are capitalised in the description, the function colorCode will always be called with the lowercase equivalent, e.g brown instead of Brown.

### _Code:_

        const colorCode = (color) => {
        	// Code here

        	return
        }

### _Challenges (2):_

- colorCode('blue') should return 6

- colorCode('white') should return 9
<br/><br/>

## 20. Add two numbers

### _Instructions:_

Add two numbers

### _Code:_

        const addTwoNumbers = (a, b) => {
        	// code here

        	return
        }

### _Challenges (2):_

- add Two Numbers

- JUST ADD TWO NUMBERS! YAAAY