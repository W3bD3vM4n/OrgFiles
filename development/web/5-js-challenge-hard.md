# Day 41 - 50

## 41. Categorize New Member

### _Instructions:_

The Western Suburbs Croquet Club has two categories of membership, Senior and Open. They would like your help with an application form that will tell prospective members which category they will be placed.

To be a senior, a member must be at least 55 years old and have a handicap greater than 7. In this croquet club, handicaps range from -2 to +26; the better the player the lower the handicap.

**Input**
Input will consist of a array of pairs. Each pair contains information for a single potential member. Information consists of an integer for the person's age and an integer for the person's handicap.

**Output**
Output will consist of a list of string values stating whether the respective member is to be placed in the senior or open category.

**Example**
(openOrSenior([[45, 12],[55,21],[19, -2],[104, 20]]) returns ['Open', 'Senior', 'Open', 'Senior']

### _Code:_

        function openOrSenior(data) {
        // your code goes below
        }

        let output = openOrSenior([
        [45, 12],
        [55, 21],
        [19, -2],
        [104, 20],
        ]);

        console.log(output);

### _Challenges (3):_

- openOrSenior([[45, 12],[55,21],[19, -2],[104, 20]]) should return ['Open', 'Senior', 'Open', 'Senior']

- openOrSenior([[3, 12],[55,1],[91, -2],[53, 23]]) should return['Open', 'Open', 'Open', 'Open']

- openOrSenior([[59, 12],[55,-1],[12, -2],[12, 12]]) should return ['Senior', 'Open', 'Open', 'Open'])
<br/><br/>

## 42. Sum of two lowest positive integers

### _Instructions:_

Create a function that returns the sum of the two lowest positive numbers given an array of minimum 4 positive integers. No floats or non-positive integers will be passed.

For example, when an array is passed like [19, 5, 42, 2, 77], the output should be 7.

### _Code:_

        function sumTwoSmallestNumbers(numbers) {
        //Code below

        }

### _Challenges (3):_

- sumTwoSmallestNumbers([5, 8, 12, 19, 22]) should return 13

- sumTwoSmallestNumbers([15, 28, 4, 2, 43]) should return 6

- sumTwoSmallestNumbers([23, 71, 33, 82, 1]) should return 24
<br/><br/>

## 43. Highest Scoring Word

### _Instructions:_

Given a string of words, you need to find the highest scoring word.

Each letter of a word scores points according to its position in the alphabet: a = 1, b = 2, c = 3 etc.

You need to return the highest scoring word as a string.

If two words score the same, return the word that appears earliest in the original string.

All letters will be lowercase and all inputs will be valid.

### _Code:_

        function high(x) {
        //code your magic here

        }

### _Challenges (2):_

- high('man i need a taxi up to ubud') should return 'taxi'

- high('what time are we climbing up the volcano') should return 'volcano'
<br/><br/>

## 44. Count the divisors of a number

### _Instructions:_

Count the number of divisors of a positive integer n.

Examples (input --> output)
4 --> 3 (1, 2, 4)
5 --> 2 (1, 5)
12 --> 6 (1, 2, 3, 4, 6, 12)
30 --> 8 (1, 2, 3, 5, 6, 10, 15, 30)

### _Code:_

        function getDivisorsCnt(num) {
        // code below

        }

### _Challenges (3):_

- getDivisorsCnt(10) should return 4

- getDivisorsCnt(11) should return 2

- getDivisorsCnt(54) should return 8
<br/><br/>

## 45. Find The Parity Outlier

### _Instructions:_

You are given an array (which will have a length of at least 3, but could be very large) containing integers. The array is either entirely comprised of odd integers or entirely comprised of even integers except for a single integer N. Write a method that takes the array as an argument and returns this "outlier" N.

**Examples**
[2, 4, 0, 100, 4, 11, 2602, 36]
Should return: 11 (the only odd number)

[160, 3, 1719, 19, 11, 13, -21]
Should return: 160 (the only even number)

### _Code:_

        function findOutlier(integers) {
        //your code here

        }

### _Challenges (3):_

- findOutlier([2,6,8,10,3]) should return 3

- findOutlier([0,0,3,0,0]) should return 3

- findOutlier([1,1,0,1,1]) should return 0
<br/><br/>

## 46.  Needle in the Haystack

### _Instructions:_

Write a function findNeedle() that takes an array full of junk but containing one "needle"

After your function finds the needle it should return a message (as a string) that says:

"found the needle at position " plus the index it found the needle, so:

findNeedle(['hay', 'junk', 'hay', 'hay', 'moreJunk', 'needle', 'randomJunk']) should return "found the needle at position 5"

### _Code:_

        function findNeedle(haystack) {
        // your code here

        }

### _Challenges (3):_

- findNeedle(['3', '123124234', undefined, 'needle', 'world', 'hay', 2, '3', true, false]) should return 'found the needle at position 3'

- findNeedle(['283497238987234', 'a dog', 'a cat', 'some random junk', 'a piece of hay', 'needle', 'something somebody lost a while ago']) should return 'found the needle at position 5'

- findNeedle([1,2,3,4,5,6,7,8,8,7,5,4,3,4,5,6,67,5,5,3,3,4,2,34,234,23,4,234,324,324,'needle',1,2,3,4,5,5,6,5,4,32,3,45,54]) should return 'found the needle at position 30'
<br/><br/>

## 47. Isograms

### _Instructions:_

An isogram is a word that has no repeating letters, consecutive or non-consecutive. Implement a function that determines whether a string that contains only letters is an isogram. Assume the empty string is an isogram. Ignore letter case.

**Example**

"Dermatoglyphics" --> true
"aba" --> false
"moOse" --> false (ignore letter case)

_Note:_ An empty string is also an isogram

### _Code:_

        function isIsogram(str) {
        // your code here

        }

### _Challenges (3):_

- isIsogram("isogram") should return true

- isIsogram("") should return true

- isIsogram("moOse") should return false
<br/><br/>

## 48. Human readable duration format

### _Instructions:_

Your task is to write a function which formats a duration, given as a number of seconds, in a human-friendly way.

The function must accept a non-negative integer. If it is zero, it just returns "now". Otherwise, the duration is expressed as a combination of years, days, hours, minutes and seconds.

It is much easier to understand with an example:

formatDuration(62)    // returns "1 minute and 2 seconds"
formatDuration(3662)  // returns "1 hour, 1 minute and 2 seconds"
For the purpose of this challenge, a year is 365 days and a day is 24 hours.

Note that spaces are important.

**Detailed rules**
The resulting expression is made of components like 4 seconds, 1 year, etc. In general, a positive integer and one of the valid units of time, separated by a space. The unit of time is used in plural if the integer is greater than 1.

The components are separated by a comma and a space (", "). Except the last component, which is separated by " and ", just like it would be written in English.

A more significant units of time will occur before than a least significant one. Therefore, 1 second and 1 year is not correct, but 1 year and 1 second is.

Different components have different unit of times. So there is not repeated units like in 5 seconds and 1 second.

A component will not appear at all if its value happens to be zero. Hence, 1 minute and 0 seconds is not valid, but it should be just 1 minute.

A unit of time must be used "as much as possible". It means that the function should not return 61 seconds, but 1 minute and 1 second instead. Formally, the duration specified by of a component must not be greater than any valid more significant unit of time.

### _Code:_

        function formatDuration(seconds) {
        // your code here

        }

### _Challenges (3):_

- formatDuration(1) should return "1 second"

- formatDuration(3662) should return "1 hour, 1 minute and 2 seconds"

- formatDuration(62) should return "1 minute and 2 seconds"
<br/><br/>

## 49. Is this a triangle?

### _Instructions:_

Implement a function that accepts 3 integer values a, b, c. The function should return true if a triangle can be built with the sides of given length and false in any other case.

(In this case, all triangles must have surface greater than 0 to be accepted).

Hint You can check whether the sum of the two sides of a triangle is greater than the third side in all possible combinations.

### _Code:_

        function isTriangle(a, b, c) {
        // your code here

        }

### _Challenges (3):_

- isTriangle(1,2,2) should return true

- isTriangle(7,2,2) should return false

- isTriangle(7,14,16) should return true
<br/><br/>

## 50. Get the Middle Character

### _Instructions:_

You are going to be given a word. Your job is to return the middle character of the word. If the word's length is odd, return the middle character. If the word's length is even, return the middle 2 characters.

Kata.getMiddle("test") should return "es"

Kata.getMiddle("testing") should return "t"

Kata.getMiddle("middle") should return "dd"

Kata.getMiddle("A") should return "A"

### _Code:_

        function getMiddle(s) {
        // your code here

        }

### _Challenges (3):_

- getMiddle("testing") should return "t"

- getMiddle("middle") should return "dd"

- getMiddle("A") should return "A"