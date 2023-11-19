# Days 21 - 30

## 21. Union of Two Arrays

### _Instructions:_

Write the code for the function which returns the the union of the two given arrays

### _Code:_

        const unionOfArrays = (arr1, arr2) => {
            // code below here

            return;
        };

        console.log(`The union is ${unionOfArrays([1, 2, 34, 45, 3], [3, 24, 21])}`);

### _Challenges (3):_

- unionOfArrays(['a','b','c'],['a',1,2,'d']) should return ['a','b','c',1,2,'d']

- unionOfArrays(['array','object'],['value','object','key']) should return ['array','object', 'value', 'key']

- unionOfArrays([1, 2, 34, 45, 3], [3, 24, 21]) == [1,2,34,45,3,24,21]) should return [1,2,34,45,3,24,21]
<br/><br/>

## 22. Unique In Order

### _Instructions:_

Implement the function unique_in_order which takes as argument a sequence and returns a list of items without any elements with the same value next to each other and preserving the original order of elements.

The argument can contain a string or an array

For example: uniqueInOrder([1,2,2,3,3]) should return [1,2,3]

uniqueInOrder('ABBCcAD') should return ['A', 'B', 'C', 'c', 'A', 'D']

### _Code:_

        let uniqueInOrder = (iterable) => {
            //your code here - remember iterable can be a string or an array

        };

### _Challenges (3):_

- uniqueInOrder('AAAABBBCCDAABBB') should return ['A', 'B', 'C', 'D', 'A', 'B']

- uniqueInOrder('ABBCcAD') should return ['A', 'B', 'C', 'c', 'A', 'D']

- uniqueInOrder([1,2,2,3,3]) should return [1,2,3]
<br/><br/>

## 23. Equal Sides Of An Array

### _Instructions:_

You are going to be given an array of integers. Your job is to take that array and find an index N where the sum of the integers to the left of N is equal to the sum of the integers to the right of N. If there is no index that would make this happen, return -1.

**For example:**

Let's say you are given the array [1,2,3,4,3,2,1]: Your function will return the index 3, because at the 3rd position of the array, the sum of left side of the index ([1,2,3]) and the sum of the right side of the index ([3,2,1]) both equal 6.

Let's look at another one. You are given the array [1,100,50,-51,1,1] Your function will return the index 1, because at the 1st position of the array, the sum of left side of the index ([1]) and the sum of the right side of the index ([50,-51,1,1]) both equal 1.

Last one: You are given the array [20,10,-80,10,10,15,35] At index 0 the left side is [] The right side is [10,-80,10,10,15,35] They both are equal to 0 when added. (Empty arrays are equal to 0 in this problem) Index 0 is the place where the left side and right side are equal.

_Note:_ Please remember that in most programming/scripting languages the index of an array starts at 0.

_Input:_ An integer array of length 0 < arr < 1000. The numbers in the array can be any integer positive or negative.

_Output:_ The lowest index N where the side to the left of N is equal to the side to the right of N. If you do not find an index that fits these rules, then you will return -1.

_Note:_ If you are given an array with multiple answers, return the lowest correct index.

### _Code:_

        function findEvenIndex(arr) {
            //Code goes here!

        }

### _Challenges (4):_

- findEvenIndex([1,2,3,4,3,2,1] should return 3

- findEvenIndex([1,100,50,-51,1,1]) should return 1

- findEvenIndex([1,2,3,4,5,6]) should return -1

- findEvenIndex([20,10,30,10,10,15,35]) should return 3
<br/><br/>

## 24. Write Number in Expanded Form

### _Instructions:_

You will be given a number and you will need to return it as a string in Expanded Form.

**For example:**

expandedForm(12); // Should return '10+2'

expandedForm(42); // Should return '40+2'

### _Code:_

        function expandedForm(num) {
            // Your code here

        }

### _Challenges (3):_

- (12) should return '10+2'

- expandedForm(42) should return '40+2'

- expandedForm(734) should return '700+30+4'
<br/><br/>

## 25. Stop gninnipS My sdroW!

### _Instructions:_

Write a function that takes in a string of one or more words, and returns the same string, but with all five or more letter words reversed (Just like the name of this Kata). Strings passed in will consist of only letters and spaces. Spaces will be included only when more than one word is present.

**Examples:**

spinWords( "Hey fellow warriors" ) => returns "Hey wollef sroirraw" 

spinWords( "This is a test") => returns "This is a test" 

spinWords( "This is another test" ) => returns "This is rehtona test"

### _Code:_

        function spinWords(string) {
            //TODO Have fun :)

        }

### _Challenges (3):_

- spinWords("Hey fellow warriors") should return"Hey wollef sroirraw"

- spinWords("You are almost to the last test") should return "You are tsomla to the last test"

- spinWords("Seriously this is the last one") should return "ylsuoireS this is the last one"
<br/><br/>

## 26. Find the odd int

### _Instructions_

Given an array of integers, find the one that appears an odd number of times.

There will always be only one integer that appears an odd number of times.

**Examples:**

[7] should return 7, because it occurs 1 time (which is odd). 

[0] should return 0, because it occurs 1 time (which is odd). 

[1,1,2] should return 2, because it occurs 1 time (which is odd). 

[0,1,0,1,0] should return 0, because it occurs 3 times (which is odd). 

[1,2,2,3,3,3,4,3,3,3,2,2,1] should return 4, because it appears 1 time (which is odd).

### _Code:_

        function findOdd(arr) {
            //happy coding!

            return 0;
        }

### _Challenges (3):_

- findOdd([20,1,-1,2,-2,3,3,5,5,1,2,4,20,4,-1,-2,5]) should return 5

- findOdd([1,1,1,1,1,1,10,1,1,1,1]) should return 10

- findOdd([5,4,3,2,1,5,4,3,2,10,10]) should return 1
<br/><br/>

## 27. Vowel Count

### _Instructions:_

Return the number (count) of vowels in the given string.

We will consider a, e, i, o, u as vowels

The input can consit of Lower case and upper case letters so make sure to count both of them.

### _Code:_

        function getCount(str) {
            let vowelsCount = 0;
            // enter your magic here

            return vowelsCount;
        }

        console.log(getCount("abracadabra"));

### _Challenges (3):_

- getCount("abracadabra") should return 5

- getCount("THe Strings are SOO COOL") should return 8

- getCount("There exists only 5 vowels") should return 7
<br/><br/>

## 28. WeIrD StRiNg CaSe

### _Instructions:_

Write a function toWeirdCase that accepts a string, and returns the same string with all even indexed characters in each word upper cased, and all odd indexed characters in each word lower cased. The indexing just explained is zero based, so the zero-ith index is even, therefore that character should be upper cased and you need to start over for each word.

The passed in string will only consist of alphabetical characters and spaces(' '). Spaces will only be present if there are multiple words. Words will be separated by a single space(' ').

### _Code:_

        function toWeirdCase(string) {
            // Your code goes here
        }

        console.log(`The weird case of ${"A test case"} is ${toWeirdCase("A test case")}`
        );

### _Challenges (3):_

- toWeirdCase('This') returns 'ThIs'

- toWeirdCase('This is a test') returns 'ThIs iS A TeSt'

- toWeirdCase('A test case') returns 'A TeSt cAsE'
<br/><br/>

## 29. Mumbling

### _Instructions:_

Each char becomes n*chars where n is the index + 1, and the first char is capitalized divided by - instead of space.

Only alphabets are passed as arguments for the accum(s) funciton

Example: accum("ZpglnRxqenU") should return "Z-Pp-Ggg-Llll-Nnnnn-Rrrrrr-Xxxxxxx-Qqqqqqqq-Eeeeeeeee-Nnnnnnnnnn-Uuuuuuuuuuu"

### _Code:_

        function accum(s) {
            // your code goes below

        }

### _Challenges (3):_

- accum("ZpglnRxqenU") returns "Z-Pp-Ggg-Llll-Nnnnn-Rrrrrr-Xxxxxxx-Qqqqqqqq-Eeeeeeeee-Nnnnnnnnnn-Uuuuuuuuuuu"

- accum("NyffsGeyylB") returns "N-Yy-Fff-Ffff-Sssss-Gggggg-Eeeeeee-Yyyyyyyy-Yyyyyyyyy-Llllllllll-Bbbbbbbbbbb"

- accum("MjtkuBovqrU") returns "M-Jj-Ttt-Kkkk-Uuuuu-Bbbbbb-Ooooooo-Vvvvvvvv-Qqqqqqqqq-Rrrrrrrrrr-Uuuuuuuuuuu"
<br/><br/>

## 30. Mexican Wave

### _Instructions:_

**Mexican Wave Origin**

The wave (known as the Mexican wave in the English-speaking world outside North America) is an example of metachronal rhythm achieved in a packed stadium when successive groups of spectators briefly stand, yell, and raise their arms. Immediately upon stretching to full height, the spectator returns to the usual seated position.

The result is a wave of standing spectators that travels through the crowd, even though individual spectators never move away from their seats. In many large arenas the crowd is seated in a contiguous circuit all the way around the sport field, and so the wave is able to travel continuously around the arena; in discontiguous seating arrangements, the wave can instead reflect back and forth through the crowd. When the gap in seating is narrow, the wave can sometimes pass through it. Usually only one wave crest will be present at any given time in an arena, although simultaneous, counter-rotating waves have been produced. (Source Wikipedia)

**Task**

To create a function that turns a string into a Mexican Wave. You will be passed a string and you must return that string in an array where an uppercase letter is a person standing up.

**Rules**

The input string will always be lower case but maybe empty.
If the character in the string is whitespace then pass over it as if it was an empty seat

**Example**

wave("hello") returns the array ["Hello", "hEllo", "heLlo", "helLo", "hellO"]

### _Code:_

        function wave(str) {
            // Your code goes below

        }

        console.log(wave("hello"));

### _Challenges (3):_

- `wave("hello")` should return `["Hello", "hEllo", "heLlo", "helLo", "hellO"]`

- `wave("two words")` should return `["Two words", "tWo words", "twO words", "two Words", "two wOrds", "two woRds", "two worDs", "two wordS"]`

- `wave(" gap ")` should return `[" Gap ", " gAp ", " gaP "]`