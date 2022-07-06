# Day 31 - 40

## 31. Write a Program to Find the Factorial of a Number

### _Instructions:_

The factorial of a number is the product of all the numbers from 1 to that number. For example,

factorial of 5 is equal to 1 * 2 * 3 * 4 * 5 = 120.

The factorial of a positive number n is given by:

factorial of n (n!) = 1 * 2 * 3 * 4.....n The factorial of negative numbers do not exist and the factorial of 0 is 1.

### _Code:_

        function factorial(n) {
	        // write your code here
	        return
        }

        let n = 4;
        console.log("The factorial of " + n + " is " + factorial(n));

### _Challenges (3):_

- factorial(2) is 2

- factorial(5) is 120

- factorial(10) is 3628800
<br/><br/>

## 32. Write a program to find the greatest common divisor (gcd) of two positive numbers

### _Instructions:_

The greatest common divisor (GCD), also called the greatest common factor, of two numbers is the largest number that divides them both. For instance, the greatest common factor of 20 and 15 is 5, since 5 divides both 20 and 15 and no larger number has this property.

### _Code:_

        function gcd(a, b) {
	        // write your code here
	        return
        }

        const a = 2154
        const b = 458

        console.log("The GCD of " + a + " ", b + " is " + gcd(a, b));

### _Challenges (3):_

- gcd(2154, 458)

- gcd(12, 4)

- gcd(333, 3333)
<br/><br/>

## 33. Write a program to print unique values from an array

### _Instructions:_

**Input**
const arrOfNum = [1, 2, 2, 4, 5, 6, 6]

**Output**
[1, 2, 4, 5, 6]

### _Code:_

        function set(arrOfNum) {
	        // write your code here
	        return
        }

        const arrOfNum = [1, 2, 2, 4, 5, 6, 6];

        console.log("result is + " + set(arrOfNum));

### _Challenges (2):_

- set([1, 2, 2, 4, 5, 6, 6]) returns [1, 2, 4, 5, 6]

- set([1, 1, 1, 1, 1]) returns [1]
<br/><br/>

## 34. Write a program to find the most frequent item of an array

### _Instructions:_

**Input**
const arr = [3, 'a', 'a', 'a', 2, 3, 'a', 3, 'a', 2, 4, 9, 3];

**Output**
a 5

### _Code:_

        function mostFreq(arr) {
	        // write your code here
	        return
        }

        const arr = [1, 2, 2, 4, 5, 6, 6];

        console.log(mostFreq(arr));

### _Challenges (2):_

- mostFreq([1, 2, 2, 4, 5, 6, 6]) returns 2 2

- mostFreq([3, 'a', 'a', 'a', 2, 3, 'a', 3, 'a', 2, 4, 9, 3]) returns a 5
<br/><br/>

## 35. Write a JavaScript function to get nth largest element from an unsorted array

### _Instructions:_

**Input**
nthlargest([ 43, 56, 23, 89, 88, 90, 99, 652], 4)

**Output**
89

### _Code:_

        function nthlargest(arr, highest) {
	        // write your code here
	        return
        }

        const arr = [43, 56, 23, 89, 88, 90, 99, 652];
        const highest = 4;

        console.log(nthlargest(arr, highest));

### _Challenges (2):_

- nthlargest([ 43, 56, 23, 89, 88, 90, 99, 652], 4) returns 89

- nthlargest([ 10, 100, 1000, 10000], 2) returns 1000
<br/><br/>

## 36. Rna Transcription

### _Instructions:_

Given a DNA strand, return its RNA complement (per RNA transcription).

Both DNA and RNA strands are a sequence of nucleotides.

The four nucleotides found in DNA are adenine (A), cytosine (C), guanine (G) and thymine (T).

The four nucleotides found in RNA are adenine (A), cytosine (C), guanine (G) and uracil (U).

Given a DNA strand, its transcribed RNA strand is formed by replacing each nucleotide with its complement:

G -> C
C -> G
T -> A
A -> U

### _Code:_

        const transcription = (dna) => {
	        // code here

	        return
        }

### _Challenges (2):_

- transcription('GCT') should return 'CGA'

- transcription('GATC') should return 'CUAG'
<br/><br/>

## 37. Tell if its a leap year

### _Instructions:_

Given a year, report if it is a leap year.

The tricky thing here is that a leap year in the Gregorian calendar occurs:

on every year that is evenly divisible by 4 except every year that is evenly divisible by 100 unless the year is also evenly divisible by 400

For example, 1997 is not a leap year, but 1996 is. 1900 is not a leap year, but 2000 is.

Notes Though our exercise adopts some very simple rules, there is more to learn!

### _Code:_

        const isLeap = (year) => {
	        // code here

	        return
        }

### _Challenges (2):_

- isLeap(2022) should return false

- isLeap(2020) should return true
<br/><br/>

## 38. Luhn algorithm

### _Instructions:_

Given a number determine whether or not it is valid per the Luhn formula.

The Luhn algorithm is a simple checksum formula used to validate a variety of identification numbers, such as credit card numbers and Canadian Social Insurance Numbers.

The task is to check if a given string is valid.

**Validating a Number**
Strings of length 1 or less are not valid. Spaces are allowed in the input, but they should be stripped before checking. All other non-digit characters are disallowed.

_Example 1:_ valid credit card number
4539 3195 0343 6467

The first step of the Luhn algorithm is to double every second digit, starting from the right. We will be doubling

4_3_ 3_9_ 0_4_ 6_6_

If doubling the number results in a number greater than 9 then subtract 9 from the product. The results of our doubling:

8569 6195 0383 3437

Then sum all of the digits:

8+5+6+9+6+1+9+5+0+3+8+3+3+4+3+7 = 80

If the sum is evenly divisible by 10, then the number is valid. This number is valid!

_Example 2:_ invalid credit card number
8273 1232 7352 0569

Double the second digits, starting from the right

7253 2262 5312 0539

Sum the digits

7+2+5+3+2+2+6+2+5+3+1+2+0+5+3+9 = 57

57 is not evenly divisible by 10, so this number is not valid.

### _Code:_

        const valid = (string) => {
	        // code here

	        return
        }

### _Challenges (2):_

- valid(string) should return true or false accordingly

- valid(string) should return true or false accordingly
<br/><br/>

## 39. Mixed Juices

### _Instructions:_

Your friend Li Mei runs her own juice bar where she sells delicious mixed fruit juices. You are a frequent customer in her shop and realized you could make your friend's life easier. You decide to use your coding skills to help Li Mei with her job.

**1. Determine how long it takes to mix a juice**
Li Mei likes to tell her customers in advance how long they have to wait for a juice from the menu that they ordered. She has a hard time remembering the exact numbers, because the time it takes to mix the juices varies. 'Pure Strawberry Joy' takes 0.5 minutes, 'Energizer' and 'Green Garden' take 1.5 minutes each, 'Tropical Island' takes 3 minutes and 'All or Nothing' takes 5 minutes. For all other drinks (e.g., special offers) you can assume a preparation time of 2.5 minutes.

To help your friend, write a function timeToMixJuice that takes a juice from the menu as an argument and returns the number of minutes it take to mix that drink.

`timeToMixJuice('Tropical Island'); // => 3

timeToMixJuice('Berries & Lime'); // => 2.5`

**2. Replenish the lime wedge supply**
A lot of Li Mei's creations include lime wedges, either as an ingredient or as part of the decoration. So when she starts her shift in the morning she needs to make sure the bin of lime wedges is full for the day ahead.

Implement the function limesToCut which takes the number of lime wedges Li Mei needs to cut and an array representing the supply of whole limes she has at hand. She can get 6 wedges from a 'small' lime, 8 wedges from a 'medium' lime and 10 from a 'large' lime. She always cuts the limes in the order in which they appear in the list, starting with the first item. She keeps going until she reached the number of wedges that she needs or until she runs out of limes.

Li Mei would like to know in advance how many limes she needs to cut. The limesToCut function should return the number of limes to cut.

limesToCut(25, ['small', 'small', 'large', 'medium', 'small']); // => 4

**3. Finish up the shift**
Li Mei always works until 3pm. Then her employee Dmitry takes over. There are often drinks that have been ordered but are not prepared yet when Li Mei's shift ends. Dmitry will then prepare the remaining juices.

To make the hand-over easier, implement a function remainingOrders which takes the number of minutes left in Li Mei's shift and an array of juices that have been ordered but not prepared yet. The function should return the orders that Li Mei cannot start preparing before the end of her work day.

The time left in the shift will always be greater than 0. Furthermore the orders are prepared in the order in which they appear in the array. If Li Mei starts to mix a certain juice, she will always finish it even if she has to work a bit longer. If there are no remaining orders left that Dmitry needs to take care of, an empty array should be returned.

remainingOrders(5, ['Energizer', 'All or Nothing', 'Green Garden']); // => ['Green Garden']

### _Code:_

        const timeToMixJuice = (name) => {
	        // code here

	        return
        }

        const limesToCut = (wedgesNeeded, limes) => {
	        // code here

	        return
        }

        const remainingOrders = (timeLeft, orders) => {
	        // code here

	        return
        }

### _Challenges (3):_

- function timeToMixJuice(name) should return asked values

- function limesToCut(wedgesNeeded, limes) should return asked values

- function remainingOrders(timeLeft, orders) should return asked values
<br/><br/>

## 40. Vehicle Purchase

### _Instructions:_

In this exercise you are going to write some code to help you prepare to buy a vehicle.

You have three tasks, one to determine if you will need to get a licence, one to help you choose between two vehicles and one to estimate the acceptable price for a used vehicle.

**1. Determine if you will need a drivers licence**
Some kinds of vehicles require a drivers license to operate them. Assume only the kinds 'car' and 'truck' require a license, everything else can be operated without a license.

Implement the needsLicense(kind) function that takes the kind of vehicle and returns a boolean indicating whether you need a license for that kind of vehicle.

`needsLicense('car'); // => true

needsLicense('bike'); // => false`

**2. Choose between two potential vehicles to buy**
You evaluate your options of available vehicles. You manage to narrow it down to two options but you need help making the final decision. For that implement the function chooseVehicle(option1, option2) that takes two vehicles as arguments and returns a decision that includes the option that comes first in dictionary order.

`chooseVehicle('Wuling Hongguang', 'Toyota Corolla'); // => 'Toyota Corolla is clearly the better choice.'

chooseVehicle('Volkswagen Beetle', 'Volkswagen Golf'); // => 'Volkswagen Beetle is clearly the better choice.'`

**3. Calculate an estimation for the price of a used vehicle**
Now that you made your decision you want to make sure you get a fair price at the dealership. Since you are interested in buying a used vehicle, the price depends on how old the vehicle is. For a rough estimate, assume if the vehicle is less than 3 years old, it costs 80% of the original price it had when it was brand new. If it is more than 10 years old, it costs 50%. If the vehicle is at least 3 years old but not older than 10 years, it costs 70% of the original price.

Implement the calculateResellPrice(originalPrice, age) function that applies this logic using if, else if and else (there are other ways but you want to practice). It takes the original price and the age of the vehicle as arguments and returns the estimated price in the dealership.

`calculateResellPrice(1000, 1); // => 800

calculateResellPrice(1000, 5); // => 700

calculateResellPrice(1000, 15); // => 500`

### _Code:_

        const needsLicense = (kind) => {
	        // code here

	        return
        }

        const chooseVehicle = (option1, option2) => {
	        // code here

	        return
        }

        const calculateResellPrice = (originalPrice, age) => {
	        // code here

	        return
        }

### _Challenges (3):_

- needsLicense(kind) should work as asked

- chooseVehicle(option1, option2) should work as asked

- calculateResellPrice(originalPrice, age) should work as asked