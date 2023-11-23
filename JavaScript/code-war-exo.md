# Code Wars Kata

### 1. evenOrOdd
```javascript
function evenOrOdd(number) {
    if (number % 2 == 0) {
        return "Even"
    } else {
        return "Odd"
    }
}
```

### 2. Multiply
```javascript
function multiply(a, b) {
    return a * b
}
```

### 3. Convert a Number to a String!
```javascript
function numberToString(num) {
    return num.toString();
}
```

### 4. Opposite number
```javascript
function opposite(number) {
    return -number;
}
```

### 5. Reversed Strings
```javascript
function solution(str) {
    return str.split("").reverse().join("");
}
```

### 6. Return Negative
```javascript
function makeNegative(num) {
    return num = -Math.abs(num);
}
```

### 7. Convert boolean values to strings 'Yes' or 'No'.
```javascript
function boolToWord(bool) {
    if (bool == 'true')
        return 'Yes';
    else
        return 'No';
}
```

### 8. Sum of positive

```javascript
function positiveSum(arr) {
    let sum = 0;
    for (let i = 0; i < arr.length; i++) {
        if (arr[i] > 0) {
            sum += arr[i];
        }
    }
    return sum;
}
```

### 9. String repeat

```javascript
function repeatStr(n, s) {
    return s.repeat(n);
}
```

### 10. Remove First & Last Character

```javascript
function removeChar(str) {
    return str.substring(1, str.length - 1);
}
```

Bien sûr, voici le code JavaScript mis en forme en Markdown :

### 11. Square(n) Sum

```javascript
function squareSum(numbers) {
    return numbers.reduce((sum, num) => sum + Math.pow(num, 2), 0);
}
```

### 12. Find the smallest integer in the array

```javascript
class SmallestIntegerFinder {
    findSmallestInt(args) {
        return Math.min(...args);
    }
}
```

### 13. Grasshopper - Summation

```javascript
var summation = function (num) {
    let sum = 0
    for (let i = num; i >= 1; i--) {
        sum += i;
    }
    return sum
}
```

### 14. Function 1 - hello world

```javascript
function greet() {
    let hello = "hello world!";
    return hello
}
```

### 15. Remove String Spaces

```javascript
function noSpace(x) {
    return x.replaceAll(' ', '')
}
```

### 16. Convert a String to a Number!

```javascript
const stringToNumber = function (str) {
    let sum = parseInt(str);
    return sum;
}
```

### 17. Counting sheep...

```javascript
function countSheeps(sheep) {
    let count = 0;
    for (let i = 0; i < sheep.length; i++) {
        if (sheep[i] === true) {
            count++;
        }
    }
    return count;
}
```

### 18. You Can't Code Under Pressure #1

```javascript
function doubleInteger(i) {
    i = i * 2;
    return i;
}
```

### 19. Returning Strings

```javascript
function greet(name) {
    return ("Hello, " + name + " how are you doing today?")
}
```

### 20. Convert a Boolean to a String

```javascript
function booleanToString(b) {
    return b.toString();
}
```

Voici le code JavaScript mis en forme en Markdown :

### 21. Keep Hydrated!

```javascript
function litres(time) {
    let waterDrink = 0.5 * time;
    let waterCount = Math.floor(waterDrink);
    return waterCount;
}
```

### 22. Basic Mathematical Operations

```javascript
function basicOp(operation, value1, value2) {
    switch (operation) {
        case '+':
            return value1 + value2;
        case '-':
            return value1 - value2;
        case '*':
            return value1 * value2;
        case '/':
            return value1 / value2;
    }
}
```

### 23. Century From Year

```javascript
function century(year) {
    if (year >= 1 && year <= 100) {
        return 1;
    }
    if (year >= 101) {
        return Math.ceil(year / 100);
    }
}
```

### 24. Beginner - Lost Without a Map

```javascript
function maps(x) {
    let newX = [];
    for (let i = 0; i < x.length; i++) {
        newX.push(x[i] * 2);
    }
    return newX;
}
```

### 25. Convert number to reversed array of digits

```javascript
function digitize(n) {
    const nbrStr = String(n)
    const array = nbrStr.split('');
    const reverseArray = array.reverse();
    const reverseNumbers = reverseArray.map(Number);
    return reverseNumbers;
}
```

### 26. Simple multiplication

```javascript
function multiplyByEightOrNine(number) {
    // Vérifier si le nombre est pair ou impair
    if (number % 2 === 0) {
        return number * 8;
    } else {
        return number * 9;
    }
}
```

### 27. Beginner Series #2 Clock

```javascript
function past(h, m, s) {
    const millisecondesParHeure = 60 * 60 * 1000;
    const millisecondesParMinute = 60 * 1000;
    const tempsTotalEnMillisecondes = h * millisecondesParHeure + m * millisecondesParMinute + s * 1000;
    return tempsTotalEnMillisecondes;
}
```

### 28. Beginner Series #1 School Paperwork

```javascript
function paperwork(n, m) {
    if (n < 0 || m < 0) {
        return 0;
    }
    return n * m;
}
```

### 29. Abbreviate a Two Word Name

```javascript
function abbrevName(name) {
    let prenom;
    let nom;
    prenom = name.substr(0, 1);
    let espace = name.indexOf(' ');
    nom = name.substr(espace + 1, 1);
    return prenom.toUpperCase() + '.' + nom.toUpperCase();
}
```

### 30. Is he gonna survive?

```javascript
function hero(bullets, dragons) {
    let bulletsToDeafeat = dragons * 2;
    return bullets >= bulletsToDeafeat;
}
```

Voici le code JavaScript mis en forme en Markdown :

### 31. Opposites Attract

```javascript
function lovefunc(flower1, flower2) {
    if ((flower1 % 2 === 0 && flower2 % 2 === 1) || (flower1 % 2 === 1 && flower2 % 2 === 0)) {
        return true;
    } else {
        return false;
    }
}
```

### 32. Convert a string to an array

```javascript
function stringToArray(string) {
    let splitString = string.split(" ");
    return splitString;
}
```

### 33. Find Maximum and Minimum Values of a List

```javascript
var min = function (list) {
    let nbrMin = Math.min(...list);
    return nbrMin;
}
var max = function (list) {
    let nbrMax = Math.max(...list);
    return nbrMax;
}
```

### 34. MakeUpperCase

```javascript
function makeUpperCase(str) {
    let maj = str.toUpperCase();
    return maj;
}
```

### 35. Sum Arrays

```javascript
function sum(numbers) {
    let totalNbr = 0;
    for (let i = 0; i < numbers.length; i++) {
        totalNbr += numbers[i];
    }
    return totalNbr;
};
```

### 36. A Needle in the Haystack

```javascript
function findNeedle(haystack) {
    const foundWorld = haystack.find((element) => element === "needle");

    if (foundWorld !== undefined) {
        const foundWorldIndex = haystack.indexOf(foundWorld);
        return `found the needle at position ${foundWorldIndex}`;
    } else {
        return 'needle not found';
    }
}
```

### 37. Are You Playing Banjo?

```javascript
function areYouPlayingBanjo(name) {
    let firstLetter = name.substr(0, 1);

    if (firstLetter === "R" || firstLetter === "r") {
        return name + " plays banjo";
    } else {
        return name + " does not play banjo";
    }
}
```

### 38. Invert values

```javascript
function invert(array) {
    return array.map((number) => -number);
}
```

### 39. Calculate average

```javascript
function findAverage(array) {
    let sum = 0;
    for (let i = 0; i < array.length; i++) {
        sum += parseInt(array[i]);
    } if (array.length === 0) {
        return 0;
    }
    let avg = sum / array.length;
    return avg;
}
```

### 40. Count of positives / sum of negatives

```javascript
function countPositivesSumNegatives(input) {
    if (input === null || input.length === 0) {
        return [];
    }
    let posNbr = 0;
    let negNbr = 0;

    for (let i = 0; i < input.length; i++) {
        if (input[i] > 0) {
            posNbr++;
        } else {
            negNbr += input[i];
        }
    }
    return [posNbr, negNbr];
}
```

### 41. Beginner - Reduce but Grow

```javascript
function grow(x) {
    let result = 1;
    for (let i = 0; i < x.length; i++) {
        result *= x[i];
    }
    return result
}
```

### 42. How good are you really?

```javascript
function betterThanAverage(classPoints, yourPoints) {
    let sumCp = 0;
    for (let i = 0; i < classPoints.length; i++) {
        sumCp += parseInt(classPoints[i]);
    }
    sumCp += parseInt(yourPoints);
    let avgCp = sumCp / (classPoints.length + 1);
    if (yourPoints > avgCp) {
        return true;
    } else {
        return false;
    }
}
```

### 43. Calculate BMI

```javascript
function bmi(weight, height) {
    let bmi = weight / (height * height);
    switch (true) {
        case bmi <= 18.5:
            return "Underweight";
            break;
        case bmi <= 25.0:
            return "Normal";
            break;
        case bmi <= 30.0:
            return "Overweight";
            break;
        default:
            return "Obese";
            break;
    }
}
```

### 44. Fake Binary 

```javascript
function fakeBin(x) {
    let res = '';
    for (let i = 0; i < x.length; i++) {
        if (parseInt(x[i]) < 5) {
            res += "0";
        } else {
            res += "1";
        }
    }
    return res;
}
```

### 45. Sentence Smash

```javascript
function smash(words) {
    return words.join(' ');
}
```

### 46. You only need one - Beginner

```javascript
function check(a, x) {
    return a.includes(x);
}
```

### 47. Will you make it?

```javascript
const zeroFuel = (distanceToPump, mpg, fuelLeft) => {
    if (distanceToPump <= mpg * fuelLeft) {
        return true
    } else {
        return false
    }
}
```

### 48. DNA to RNA Conversion

```javascript
function DNAtoRNA(dna) {
    return dna = dna.replace(/T/g, 'U');
}
```

### 49. Reversed sequence

```javascript
const reverseSeq = n => {
    const result = [];
    for (let i = n; i >= 1; i--) {
        result.push(i);
    }
    return result;
};
```

### 50. Count by X

```javascript
function countBy(x, n) {
    let z = [];
    if (n <= 0 || x <= 0) {
        return z;
    }
    for (let i = 1; i <= n; i++) {
        z.push(i * x);
    }
    return z;
}
```

Voici le code JavaScript formaté en Markdown :

### 51. If you can't sleep, just count sheep!!

```javascript
var countSheep = function (num) {
    let resultat = "";
    for (let i = 1; i <= num; i++) {
        resultat += `${i} sheep...`;
    }
    return resultat;
}
```

### 52. Quarter of the year

```javascript
function quarterOf(month) {
    if (month >= 1 && month <= 3) {
        return 1;
    } else if (month >= 4 && month <= 6) {
        return 2;
    } else if (month >= 7 && month <= 9) {
        return 3;
    } else {
        return 4;
    }
}
```

### 53. Grasshopper - Personalized Message

```javascript
function greet(name, owner) {
    if (name === owner) {
        return 'Hello boss';
    } else {
        return 'Hello guest';
    }
}
```

### 54. Rock Paper Scissors!

```javascript
const rps = (p1, p2) => {
    if ((p1 === "scissors" && p2 === "paper") || (p1 === "paper" && p2 === "rock") || (p1 === "rock" && p2 === "scissors")) {
        return "Player 1 won!";
    } if (p1 === p2) {
        return "Draw!";
    }
    return "Player 2 won!";
}
```

### 55. Grasshopper - Grade book

```javascript
function getGrade(s1, s2, s3) {
    let avr = (s1 + s2 + s3) / 3;

    if (avr >= 90 && 100) {
        return "A"
    } else if (avr >= 80 && 90) {
        return "B"
    } else if (avr >= 70 && 80) {
        return "C"
    } else if (avr >= 60 && 70) {
        return "D"
    } else (avr >= 0 && 60)
    return "F"
}
```

### 56. Volume of a Cuboid

```javascript
class Kata {
    static getVolumeOfCuboid(length, width, height) {
        let avr = length * width * height;
        return avr;
    }
}
```

### 57. Remove exclamation marks

```javascript
function removeExclamationMarks(s) {
    return s.replace(/!/g, '');
}
```

### 58. Third Angle of a Triangle

```javascript
function otherAngle(a, b) {
    return 180 - (a + b);
}
```

### 59. Grasshopper - Messi goals function

```javascript
function goals(laLigaGoals, copaDelReyGoals, championsLeagueGoals) {
    let allGoal = laLigaGoals + copaDelReyGoals + championsLeagueGoals;
    return allGoal;
}
```

### 60. Double Char

```javascript
function doubleChar(str) {
    let res = "";
    for (let i = 0; i < str.length; i++) {
        res += str[i].substr(0, 1).repeat(2);
    }
    return res;
}
```

### 61. Sum Mixed Array

```javascript
function sumMix(x) {
    let sumX = 0;
    for (let i = 0; i < x.length; i++) {
        sumX += parseInt(x[i]);
    }
    return sumX;
}
```

### 62. Total amount of points

```javascript
function points(games) {
    let win = 3;
    let loose = 0;
    let draw = 1;
    let sumGames = 0;

    for (let i = 0; i < games.length; i++) {
        let score = games[i].split(':');
        let x = +score[0];
        let y = +score[1];
        if (x > y) {
            sumGames += win;
        } else if (x === y) {
            sumGames += draw;
        } else if (x < y) {
            sumGames += loose;
        }
    }
    return sumGames
}
```

### 63. Get the mean of an array

```javascript
function getAverage(marks) {
    let sum = 0;

    for (let i = 0; i < marks.length; i++) {
        sum += marks[i];
    }
    let avr = sum / marks.length;
    let roundAvr = Math.floor(avr);
    return roundAvr;
}
```

### 64. Array plus array

```javascript
function arrayPlusArray(arr1, arr2) {
    let sumArr1 = 0;
    let sumArr2 = 0;
    for (let i = 0; i < arr1.length; i++) {
        sumArr1 += arr1[i];
    } for (let j = 0; j < arr2.length; j++) {
        sumArr2 += arr2[j];
    }
    return sumArr1 + sumArr2
}
```

### 65. Removing Elements

```javascript
function removeEveryOther(arr) {
    let rest = [];
    for (let i = 0; i < arr.length; i += 2) {
        rest.push(arr[i]);
    }
    return rest;
}
```

### 66. Count the Monkeys!

```javascript
function monkeyCount(n) {
    let sum = [];
    for (let i = 1; i <= n; i++) {
        sum.push(i);
    }
    return sum
}
```

### 67. Find the first non-consecutive number

```javascript
function firstNonConsecutive(arr) {
    if (arr.length <= 1) return null;

    for (let i = 0; i < arr.length - 1; i++) {
        if (arr[i + 1] !== arr[i] + 1) {
            return arr[i + 1];
        }
    }

    return null;
}
```

### 68. Transportation on vacation

```javascript
function rentalCarCost(d) {
    let total = 0;
    const fraisParJour = 40;
    const promo1 = 20;
    const promo2 = 50;

    total += d * fraisParJour;

    if (d >= 3 && d < 7) {
        total -= promo1;
    } else if (d >= 7) {
        total -= promo2;
    }
    return total;
}
```

### 69. Thinkful - Logic Drills: Traffic light

```javascript
function updateLight(current) {
    if (current === "green") {
        return "yellow";
    } else if (current === "yellow") {
        return "red";
    } else {
        return "green";
    }
}
```

### 70. Jenny's secret message

```javascript
function greet(name) {
    if (name === "Johnny") {
        return "Hello, my love!";
    }
    return "Hello"
}
```

Voici le code JavaScript formaté en Markdown :

### 71. Get Planet Name By ID

```javascript
function getPlanetName(id) {
    var name;
    switch (id) {
        case 1:
            return name = 'Mercury';
        case 2:
            return name = 'Venus';
        case 3:
            return name = 'Earth';
        case 4:
            return name = 'Mars';
        case 5:
            return name = 'Jupiter';
        case 6:
            return name = 'Saturn';
        case 7:
            return name = 'Uranus';
        case 8:
            return name = 'Neptune';
    }
}
```

### 72. Basic variable assignment

```javascript
let a = "code";
let b = "wa.rs";
let name = a + b;
```

### 73. Unfinished Loop - Bug Fixing #1

```javascript
function createArray(number) {
    var newArray = [];
    for (var counter = 1; counter <= number; counter++) {
        newArray.push(counter);
    }
    return newArray;
}
```

### 74. Capitalization and Mutability

```javascript
function capitalizeWord(word) {
    let wordS = word.slice(0, 1);
    wordS = wordS.toUpperCase();
    return wordS + word.slice(1);
}
```

### 75. Grasshopper - If/else syntax debug

```javascript
function checkAlive(health) {
    if (health <= 0) {
        return false;
    } else {
        return true;
    }
}
```

### 76. FIXME: Replace all dots

```javascript
var replaceDots = function (str) {
    return str = str.replace(/\./g, '-');
}
```

### 77. Is this my tail?

```javascript
function correctTail(bod, tail) {
    let sub = bod.substring(bod.length - tail.length);
    if (sub === tail) {
        return true;
    } else {
        return false;
    }
}
```

### 78. Grasshopper - Debug

```javascript
function weatherInfo(temp) {
    var c = convertToCelsius(temp);
    if (c <= 0) {
        return (c + " is freezing temperature");
    } else {
        return (c + " is above freezing temperature");
    }
}

function convertToCelsius(temperature) {
    var celsius = (temperature - 32) * (5 / 9)
    return celsius
}
```

### 79. 101 Dalmatians - squash the bugs, not the dogs!

```javascript
function howManyDalmatians(number) {
    var dogs = ["Hardly any", "More than a handful!", "Woah that's a lot of dogs!", "101 DALMATIONS!!!"];
    var respond = number <= 10 ? dogs[0] : number <= 50 ? dogs[1] : number === 101 ? dogs[3] : dogs[2];
    console.log(dogs);
    return respond;
}
```

### 80. Return to Sanity

```javascript
function mystery() {
    var results = { sanity: 'Hello' };
    return results;
}
```

### 81. Swap Values

```javascript
function swapValues(args) {
    var temp = args[0];
    args[0] = args[1];
    args[1] = temp;
}
```

### 83. String Templates - Bug Fixing #5

```javascript
function buildString(...template) {
    return `I like ${template.join(', ')}!`;
}
```

### 84. Incorrect division method

```javascript
const solve = (x, y) => x / y;
```

### 85. Fix your code before the garden dies

```javascript
function rainAmount(mm) {
    const seuil = 40;
    if (mm < seuil) {
        console.log(mm);
        return "You need to give your plant " + (seuil - mm) + "mm of water";
    } else {
        return "Your plant has had more than enough water for today!";
    }
}
```

### 87. Unexpected parsing

```javascript
function getStatus(isBusy) {
    var msg = (isBusy ? "busy" : "available");
    return {
        status: msg
    };
}
```

### 88. Switch/Case - Bug Fixing #6

```javascript
function evalObject(value) {
    var result = 0;
    switch (value.operation) {
        case '+':
            result = value.a + value.b;
            return result;
        case '-':
            result = value.a - value.b;
            return result;
        case '/':
            result = value.a / value.b;
            return result;
        case '*':
            result = value.a * value.b;
            return result;
        case '%':
            result = value.a % value.b;
            return result;
        case '^':
            result = Math.pow(value.a, value.b);
            return result;
    }
    return;
}
```

### 89. Push a hash/an object into array

```javascript
items = [];
items.push({ a: "b", c: "d" });
```

### 90. Fix the Bugs (Syntax) - My First Kata

```javascript
function myFirstKata(a, b) {
    if (typeof (a) != "number" || typeof (b) != "number") {
        return false;
    } else {
        return a % b + b % a;
    }
}
```

### 91. Semi-Optional

```javascript
function wrap(value) {
    return {
        value: value
    };
}
```

### 92. Shifty Closures

```javascript
var name1 = 'Abe';
var greet_abe = function () {
    return "Hello,

 " + name1 + '!';
};
name2 = 'Ben';
var greet_ben = function () {
    return "Hello, " + name2 + '!';
};
```

### 93. Broken Counter

```javascript
function Counter() {
    this.value = 0;
}
Counter.prototype.increase = function () {
    return this.value++;
};
Counter.prototype.getValue = function () {
    return this.value;
};
Counter.prototype.reset = function () {
    return this.value = 0;
};
```

### 94. Max Headroom and JavaScript style

```javascript
function getMax1(name) {
    var max;
    max = { name: 'Max Headroom' }
    return max;
}
```

### 95. Is n divisible by x and y?

```javascript
function isDivisible(n, x, y) {
    return n % x === 0 && n % y === 0;
}
```

### 96. Area or Perimeter

```javascript
const areaOrPerimeter = function (l, w) {
    if (l === w) {
        return l * w;
    } else {
        return 2 * (l + w);
    };
}

<<<<<<< HEAD
//95. Invalid Login - Bug Fixing #11
function validate(username, password) {
    if(password.indexOf('||') > -1 || password.indexOf('//') > -1) return 'Wrong username or password!';
    return new Database().login(username, password);
=======
//97. Reversed Words
function reverseWords(str) {
    let test = '';
    test = str.split(' ');
    console.log(test);
    test = test.reverse().join(' ');
    console.log(test);
    return test;
}
```

### 98. Sum without highest and lowest number

```javascript
function sumArray(array) {
    if (!Array.isArray(array) || array.length <= 1) {
        return 0;
    }
    let min = Math.min(...array);
    let max = Math.max(...array);
    let sum = 0;
    for (let i = 0; i < array.length; i++) {
        sum += array[i];
    }
    sum -= min + max;
    return sum;
}
```

### 99. The Feast of Many Beasts

```javascript
function feast(beast, dish) {
    let beastStart = beast[0];
    let beastEnd = beast[beast.length - 1];
    let dishStart = dish[0];
    let dishEnd = dish[dish.length - 1];
    return beastStart === dishStart && beastEnd === dishEnd;
}
```

### 100. Parse nice int from char problem

```javascript
function getAge(inputString){  
    let test = inputString.slice(0, 1);
    let isspi = parseInt(test)
    return isspi; 
}
```

### 101. Beginner Series #4 Cockroach

```javascript
function cockroachSpeed(s) {
    let vitesse = 27.778;
    let sum = 0; 
    sum = s * vitesse; 
    let result = Math.floor(sum);
    return result;
}
```

### 102. FIXME: Get Full Name

```javascript
class Dinglemouse {
    constructor(firstName, lastName) {
        this.firstName = firstName;
        this.lastName = lastName;
        console.log(firstName, lastName);
    }
    getFullName() {
        return `${this.firstName} ${this.lastName}`.trim();
    }
}
```

### 103. getNames()

```javascript
function getNames(data) {
    return data.map(item => item.name);
}
```

### 104. Debug Sum of Digits of a Number

```javascript
function getSumOfDigits(integer) {
    var sum = 0;
    var digits = integer.toString();
    for(var ix = 0; ix < digits.length; ix++) {
        sum += parseInt(digits[ix]);
    }
    return sum;
}
```

### 105. Multiples of 3 or 5

```javascript
function solution(number) {
    if (number < 0) {
        return 0;
    }
    let sum = 0;
    for (let i = 0; i < number; i++) {
        if (i % 3 === 0 || i % 5 === 0) {
            sum += i;
        }
    }
    return sum;
}
```

### 106. Vowel Count

```javascript
function getCount(str) { 
    let nbV = 0;  
    for (let index = 0; index < str.length; index++) {
        if (str[index] === 'a' || str[index] === 'e' || str[index] === 'i' || str[index] === 'o' || str[index] === 'u') {   
        nbV++;   
      }
    }
    return nbV;   
}
```

### 107. Disemvowel Trolls

```javascript
function disemvowel(str) { 
    return str.replace(/[aeiouAEIOU]/g, '');
>>>>>>> a6252376a80fa2b7534778c8d7780dff90059b93
  }

//96. 
