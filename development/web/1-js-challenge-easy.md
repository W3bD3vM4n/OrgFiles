# #50 Days Of JS Challenge

Level up your JavaScript skills with a daily coding challenge.

## Course Structure

50 lectures • 04:10:00 total duration

# Easy

## 1. Function which returns a random number in the given range

### _Instructions:_

Create a function which returns a random number in the given range of values both inclusive

### _Code:_

        function randomNumberGeneratorInRange(rangeStart, rangeEnd) {
            // write your solution here

            return
        }

        console.log(`My random number: ${randomNumberGeneratorInRange(5, 100)}`)

### _Challenges (2):_
- randomNumberGeneratorInRange(10, 50) should return a number between 10-50 (inclusive)

- randomNumberGeneratorInRange(100, 200) should return a number between 100-200 (inclusive)
<br/><br/>

## 2. Write a program to reverse a string

### _Instructions:_

- String can be reversed by iterating it and storing it in reverse order

- String can also be reversed by converting it to array, then joining it after reversing

### _Code:_

        sconst str = "JavaScript is awesome"

        function reverseAString(str) {
            // write your solution here

            return
        }

        console.log(`Reversed string is: ${reverseAString(str)}`)

### _Challenges (3):_

- reverseAString("JavaScript is awesome") should return "emosewa si tpircSavaJ"

- reverseAString("Peter Parker is Spiderman") should return "namredipS si rekraP reteP"

- reverseAString("codedamn") should return "nmadedoc"
<br/><br/>

## 3. Write a program to reverse a given integer number

### _Instructions:_

- The remainder of the number can be fetched and the number can be divided by 10 to remove the the digit in loop till number becomes 0

- A simple approach to reverse a number could also be to convert it in to a string and then reverse it

### _Code:_

        const num = 3849;

        function reverseGivenInteger(num) {
            // write your solution here

            return
        }

        console.log(`Reversed integer is: ${reverseGivenInteger(num)}`)

### _Challenges (3):_

- reverseGivenInteger(3849) returns 9483

- reverseGivenInteger(2222) returns 2222

- reverseGivenInteger(1002) returns 2001
<br/><br/>

## 4. Write a function which can convert the time input given in 12 hours format to 24 hours format

### _Instructions:_

- The check for 'AM' and 'PM' can be verified using endsWith String method

- An extra 0 would be needed if the hours have single digit

### _Code:_

        const time = '12:10AM';

        function convertTo24HrsFormat(time) {
            // write your solution here

            return
        }

        console.log(`Converted time: ${convertTo24HrsFormat(time)}`)

### _Challenges (6):_

- convertTo24HrsFormat("12:10AM") returns "00:10"

- convertTo24HrsFormat("5:00AM") returns "05:00"

- convertTo24HrsFormat("12:33PM") returns "12:33"

- convertTo24HrsFormat("01:59PM") returns "13:59"

- convertTo24HrsFormat("11:8PM") returns "23:08"

- convertTo24HrsFormat("10:02PM") returns "22:02"
<br/><br/>

## 5. Write a function which accepts a string argument and returns the count of characters between the first and last character 'X'

### _Instructions:_

- indexOf and lastIndexOf are the methods on String which returns the position of the given string in the input string from start and end respectively

- If the match is not found, these methods return -1

### _Code:_

        const str = 'XeroX';

        function getTheGapX(str) {
            // write your solution here

            return
        }

        console.log(`Gap between the X's: ${getTheGapX(str)}`)

### _Challenges (4):_

- getTheGapX('XeroX') returns 4

- getTheGapX('Xamarin') returns 0

- getTheGapX('JavaScript') returns -1

- getTheGapX("F(X) !== G(X) !== F(X)") returns 18
<br/><br/>

## 6. Write a function to truncate a string to a certain number of words

### _Instructions:_

Truncate a string to a certain number of words

### _Code:_

        const str = 'JavaScript is simple but not easy to master';
        const wordLimit = 3

        function truncateWithWordLimit(str, wordLimit) {
            // write your solution here

            return
        }

        console.log(`Truncated string: ${truncateWithWordLimit(str, wordLimit)}`)

### _Challenges (2):_

- truncateWithWordLimit("JavaScript is simple", 3) returns "JavaScript is simple"

- truncateWithWordLimit("Codedamn is the best place to learn to code", 5) returns "Codedamn is the best place"
<br/><br/>

## 7. Create a regular expression to validate if the given input is valid Indian mobile number or not

### _Instructions:_

- Regular expression check has to have an optional +91 or 0 in the beginning, then an optional space and 10 digits

- test method of regular expression can be used to validate if the mobile number pattern matches or not

### _Code:_

        const number = '+919876543210';

        function validateMobile(number) {
        // write your solution here

        return
        }

        console.log(`is a valid Indian mobile number: ${validateMobile(number)}`)

### _Challenges (5):_

- validateMobile('+919876543210') returns true

- validateMobile('+91 9876543210') returns true

- validateMobile('09876543210') returns true

- validateMobile('9876543210') returns true

- validateMobile('99876543210') returns false
<br/><br/>

## 8. Write a function which accepts two valid dates and returns the difference between them as number of days

### _Instructions:_

- The difference between 2 dates in JavaScript will give the time difference in milliseconds

- Time difference can be converted in to days by dividing the 24Hrs time in milliseconds

### _Code:_

        const DAY_IN_MILLISECONDS = 1000 * 60 * 60 * 24;

        function getDaysBetweenDates(dateText1, dateText2) {
        // write your solution here

        return
        }

        console.log(`Days difference: ${getDaysBetweenDates('10/15/2020', '12/1/2020')}`)

### _Challenges (3):_

- getDaysBetweenDates('10/15/2020', '12/1/2020') returns 47

- getDaysBetweenDates('11/10/2021', '11/12/2021') returns 2

- getDaysBetweenDates('11/01/2020', '11/05/2020') returns 4
<br/><br/>

## 9. Write a function to check if an object is empty or not in javaScript?

### _Instructions:_

How to check if an object is empty or not in javaScript?

### _Code:_

        const obj = { key: 1 };

        function isEmpty(obj) {
            // write your solution here

            return
        }

        console.log(`is empty object: ${isEmpty(obj)}`)

### _Challenges (2):_

- isEmpty({}) returns true

- isEmpty({key: 1}) returns false
<br/><br/>

## 10. Write a function to remove array element based on object property?

### _Instructions:_

How to remove array element based on object property?

### _Code:_

        const array = [
            { field: "id", operator: "eq" },
            { field: "cStatus", operator: "eq" },
            { field: "money", operator: "eq" },
        ];

        const filterField = "money"

        function removeArrayElement(filterField) {
            // write your solution here

            return
        }

        console.log(`filtered array: ${removeArrayElement(filterField)}`)

### _Challenges (3):_

- removeArrayElement("money") returns the array without the money object

- removeArrayElement("id") returns the array without the id object

- removeArrayElement("cStatus") returns the array without the cStatus object