# CORE-CODE_2
_________________________________________________________________________________________________________________________________________________________________________________
# WEEK 1
_________________________________________________________________________________________________________________________________________________________________________________

# DAY 2 01/11/2022

1. 

R// Ready

2.
R// The Java language is both compiled and interpreted. The compiler converts the source code that resides in files whose extension is .java, to a set of instructions called bytecodes that are saved in a file whose extension is .class. These instructions are independent of the type of computer. The interpreter executes each of these instructions on a specific computer (Windows, Macintosh, etc). Therefore, it is only necessary to compile the program once, but it is interpreted each time it is run on a computer.

3.
R// 
```
INICIO
   VARIABLE Quetzales
   LEER <- Quetzales
   IMPRIMIR -> "Quetzales equivalentes en Dolares" Quetzales / 7.70
FIN
```
4.
R// Ready

5.
R// When you're writing code in a programming language, you’ll have to battle with strict syntax and rigid coding patterns. But you write pseudocode in a language or form with which you're very familiar.

6.
R//
```
INICIO
Funcion calculateAge(birthDate):
    today = 2022
    age = today - birthDate.year
     
   Imprimir(calculateAge(birthDate), "Years")
FIN
```
7.
R// Ready

8.
R//A software programmer can use flowcharts sketched on a whiteboard as part of efforts to explain his or her vision to a team of code developers.

9//
Most programming languages that you will have heard of are high-level languages. Python and C# are examples of high-level languages that are widely used in education and in the workplace. A high-level language is one that is user-oriented in that it has been designed to make it straightforward for a programmer to convert an algorithm into program code.

A low-level language is machine-oriented. Low-level programs are expressed in terms of the machine operations that must be performed to carry out a task. This makes writing programs more difficult, as the algorithm must be specified in terms of the capabilities and specifications of the processor. Low-level languages are named for the processor (or processor family) that they are designed for, and are often referred to as assembly language or machine code.
_________________________________________________________________________________________________________________________________________________________________________________

_________________________________________________________________________________________________________________________________________________________________________________

# DAY 3 01/12/2022

1.
R//
BINARY, DECIMAL, HEXADECIMAL NUMBERS

Decimals
To understand binary and hexadecimal numbers, it is best to have a good understanding of how decimal numbers work.
Each digit of a decimal number goes in one "place", and the decimal point tells us what position each one is.
The position just to the left of the point is the "units". Every time we move to the left it is worth 10 times more, and to the right it is worth 10 times less:

```
17.591

 1       7            .          5           9            1
Tens - Units - Decimal point - Decimos - Hundredths - thousandths
```

But this is only a way of writing numbers. There are other ways like Roman numerals, binary, hexadecimal, and more. You could even mark dots on a piece of paper!
_________________________________________________________________________________________________________________________________________________________________________________

The decimal numbering system is also called "base 10", because it is based on the number 10.
In decimal there are ten symbols (0 to 9), but notice this: there is no symbol for "ten". "10" are actually two symbols together, a "1" and a "0":

In decimal we count 0,1,2,3,4,5,6,7,8,9, then we say "I have run out of symbols, so I start again with 0, but first I will add 1 to the left"

But it is not mandatory to use 10 as a "base". You could use 2 ("binary"), 16 ("hex"), or whatever number you want! Just follow the same rule.

Binary numbers
Binary numbers are "base 2" instead of "base 10". You start by counting 0, then 1, you've run out of digits! So you go back to 0, but increase the number on the left by 1.

It works like this:


```
000
 
001
 
010 there is no "2" in binary, so we go back to 0 ...
    ... and we add 1 to the figure on the left

011
 
100  we go back to 0 again, and add 1 to the left ...
     ... but that number is already 1 so it is 0 again ...
     ... and the 1 is added to the next number to the left

101
 
110
etc...

```

Hexadecimal numbers
Hexadecimal numbers are interesting. There are 16 different digits! They are like decimals up to 9, but then there are letters ("A '," B "," C "," D "," E "," F ") for the values 10 to 15.

So with a single hexadecimal number you can give 16 different values instead of the usual 10:

```
Decimal: 0 1 2 3 4 5 6 7 8 9 10 11 12 13 14 15
Hexadecimal: 0 1 2 3 4 5 6 7 8 9 A B C D E F
```

```
Decimal      Binary       Hexadecimal
  0           0000            0
  1           0001            1
  2           0010            2
  3           0011            3
  4           0100            4
  5           0101            5
  6           0110            6
  7           0111            7
  8           1000            8
  9           1001            9 
 10           1010            A
 11           1011            B
 12           1100            C
 13           1101            D
 14           1110            E
 15           1111            F
```

2.
R//

```
Date of birth 1997
Binary 11111001101
Hexadecimal 7CD
```

3.
R//

```
51966
Hexadecimal: CAFE
Binary: 1100101011111110
```
5.2

R//
```
.data
	message: .asciiz "\nSUMA DE DOS NUMEROS\n"
	number1: .asciiz "\nIngrese el primer numero: "
	number2: .asciiz "\nIngrese el segundo numero: "
	result_message: .asciiz "\nEl resultado es: "
.text
	main:
		#MENSAJE SUMA DE DOS NUMEROS
		li $v0, 4
                la $a0, message
                syscall
                
		
		#INGRESO DEL PRIMER NUMERO
		li $v0, 4
		la $a0, number1
		syscall

		li $v0, 5
		syscall
		
		move $t0, $v0
		
		#INGRESO DEL SEGUNDO NUMERO
		li $v0, 4
		la $a0, number2
		syscall

		li $v0, 5
		syscall

		move $t1, $v0
		
		#OPERACION SUMA
		
		add $t2, $t0, $t1
		
		#MENSAJE DEL RESULTADO
		li $v0, 4
		la $a0 result_message
		syscall

		li $v0, 1
		move $a0, $t2
		syscall
```

5.2

R//

```
.data
    message: .asciiz "\nJosé Carlos Tiño Maxía\n"
  .text
    main:
      li $v0, 4
      la $a0, message
      syscall

```      
_________________________________________________________________________________________________________________________________________________________________________________      
# WEEK 2
_________________________________________________________________________________________________________________________________________________________________________________

# DAY TUESDAY 18/01/2022
#Multiply
```
function multiply(a, b){
  return a * b;
}
```
#ASCII Total
```
function uniTotal (string) {
  let counter = 0;
  
  for (let i = 0; i < string.length; i++){
    counter += string.charCodeAt(i);
  }
  return counter;
}
```
#get character from ASCII Value
```
function getChar(c){
  return String.fromCharCode(c)
}
```
#Binary Addition
```
function addBinary(a,b) {
  let c = a + b
  
  let cBinary = c.toString(2)
  
  return cBinary
}
```
#Student's Final Grade
```
function finalGrade (exam, projects) {
  if(exam > 90 || projects > 10) {
    
    return 100;
  }
  
  if(exam > 75 && projects >= 5) {
     return 90;
  }
  
  if(exam > 50 && projects >= 2) {
    return 75;
  }else{
   return 0; 
  }
}
```
_________________________________________________________________________________________________________________________________________________________________________________
# DAY WEDNESDAY 19/01/2022
#Holiday VIII - Duty Free
```
function dutyFree(normPrice, discount, hol){
  let amount = hol / (normPrice * (discount * 0.01))
  amount = Math.floor(amount)
  
  return amount;
}

```
#Twice as old
```
function twiceAsOld(dadYearsOld, sonYearsOld) {
  return Math.abs(dadYearsOld - (sonYearsOld * 2))
}
```
#Valid Spacing
```
function validSpacing(s) {
  let last = s[0];
  if(s[0] === " " || s[s.length - 1] === " "){
    return false
  }
  
  for(let i =1; i < s.length; i++){
    if(last === " " && last === s[i]){
      return false
    }
    last = s[i];
  }
  
  return true;
}
```
#Fake Binary
```
function fakeBin(x){
  let result = [];
  for(let i = 0; i < x.length; i++) {
    if(parseInt(x[i], 10) < 5)
      result.push('0')
    
    if(parseInt(x[i]) >= 5)
       result.push('1');
  }
  return result.join(""); 
}
```
# DAY THURSDAY
#Exclamation marks series #2: Remove all exclamation marks from the end of sentence
```
function remove (string) {  
  return string.replace(/!*$/g,'');
}

```
#Rock Paper Scissors!
```
const rps = (p1, p2) => {
    if(p1 === p2){
      return 'Draw!'
    }
    
    if(p1 === 'scissors' && p2 === 'paper'){
      return 'Player 1 won!'
    }else if(p1 === 'paper' && p2 === 'rock'){
      return 'Player 1 won!'
    }else if(p1 === 'rock' && p2 === 'scissors'){
      return 'Player 1 won!'
    }else{
      return 'Player 2 won!'
    }
  };
```    
#Persistent Bugger
```
function persistence(num) {
  if (num.toString().length === 1) {
    return 0;
  }
  var mult = 1;
  var splitStr = num.toString().split("");
  for (var i = 0; i < splitStr.length; i++) {
    mult *= parseFloat(splitStr[i])
  }
  return 1 + persistence(parseFloat(mult));
}
```
_________________________________________________________________________________________________________________________________________________________________________________      
# WEEK 3
_________________________________________________________________________________________________________________________________________________________________________________
#MONDAY
#Who likes it
```
function likes(names) {
  var templates = [
    'no one likes this',
    '{name} likes this',
    '{name} and {name} like this',
    '{name}, {name} and {name} like this',
    '{name}, {name} and {n} others like this'
  ];
  var idx = Math.min(names.length, 4);
  
  return templates[idx].replace(/{name}|{n}/g, function (val) {
    return val === '{name}' ? names.shift() : names.length;
  });
}
```
#Bit Counting
```
var countBits = function(n) {
  const base = (n).toString(2).split('');
   const result = base.reduce((sum, num) => sum + Number(num), 0);
   return result;
};
```
#Decode the Morse code
```
decodeMorse = function(morseCode){
  let string = '';
  let counterWords = 1;
  let arrayWords = morseCode.trim().split('   ');
  
  arrayWords.forEach(word => {
    let letters = word.split(' ');
    
    letters.forEach(letter =>{
      string+=MORSE_CODE[letter]
    })
    if(counterWords != arrayWords.length){
      string+=' ';
    }
    
    counterWords++;
    
  });
  
  return string;
} 
```

#TUESDAY
#Your order, please
```
function order(words){
  return words.split(' ').sort(function(a,b){
    return a.match(/\d/) - b.match(/\d/);
  }).join(' ');
}
```

#Counting Duplicates
```
function duplicateCount(text){
  let result = 0, soltingObject = {};
  text.toLowerCase().split('').map(str => {
      if (!soltingObject.hasOwnProperty(str)) {
        soltingObject[str] = 0;
      } 
      else {
        if (soltingObject[str] === 0) {
          result += 1;
        }
        soltingObject[str] = soltingObject[str] + 1;
      }
  });
  return result;
}
```
#Simple Pig Latin
```
function pigIt(str){
  str = str.trim().split(/\s{1,}/);
    return str.map(val => {
      if (/^[A-Za-z]+$/.test(val)) {
        return `${val.slice(1)}${val.slice(0, 1)}ay`;
      }
      return val;
    }).join(' ');
}
```

#WEDNESDAY

#Valid Parentheses
```
function validParentheses(parens) {
  const reg = /\(\)/g;
  while(reg.test(parens)) {
    parens = parens.replace(reg, '');
  }
    
  return parens === '';
}
```
#Convert string to camel case
```
function toCamelCase(str){
  str = str.split('');
  return str.map(function(el, i){
    if(el == '-' || el == '_'){
      el = str[i+1].toUpperCase();
      str.splice(i+1, 1);
    }
    return el;
  }).join('');
}
```
#Unique In Order
```
var uniqueInOrder=function(iterable){
  if (typeof iterable === 'string') {
    let newArray = [];
    const [...arr] = [...iterable];
    for (let i = 0; i < arr.length; i++) {
      if (arr[i] != arr[i + 1]) {
        newArray.push(arr[i])
      }
    }
             return newArray;
  }
  else{
    let newArray = [];
    for (let i = 0; i < iterable.length; i++) {
      if (iterable[i] != iterable[i + 1]) {
        newArray.push(arr[i])
      }
    }
  return newArray;
  }
}
```
#THURSDAY

#Fold an array
```
function foldArray(array, runs)
{
  const r = [], c = array.slice();
  while (c.length) r.push(c.pop() + (c.shift() || 0));
  return runs - 1 ? foldArray(r, runs - 1) : r;
}
```
#Encrypt this!
```
var encryptThis = function(text) {
    return text.split(' ').map(e => {
      if (e.length === 1) return e.charCodeAt(0);
      if (e.length === 2) return `${e[0].charCodeAt(0)}${e[1]}`;
      if (e.length === 3) return `${e[0].charCodeAt(0)}${e.slice(-1)}${e[1]}`;
      if (e.length > 3) return `${e[0].charCodeAt(0)}${e.slice(-1)}${e.slice(2, -1)}${e[1]}`;
    }).join(' ');
}
```
#Format a string of names like 'Bart, Lisa & Maggie'. (retired)
```
function list(names){
  let len = names.length;
  if(len==0) return '';
  return names.slice(0, len-1).map(p=>p.name).join(", ") + (len>1 ? ' & ' : '') + names[len-1].name;
}
```
_________________________________________________________________________________________________________________________________________________________________________________      
# WEEK 4
_________________________________________________________________________________________________________________________________________________________________________________

#MONDAY
#Regex Exercise
```
const ex1 = 'The quick brown fox jumped over the lazy dog';
const ex2 = 'A1B2C3D4E5F6G7H8I9J10';
const ex3 = 'The salad costs $9.99';
const ex4 = 'Contact customer support on 0800 300 500';
const ex5 = 'You can contact me on Twitter @codebubb or james@juniordevelopercentral.com';

// Exercise 01
// Using a regex pattern, get the 3 letter words in the ex1 string.
console.log(ex1.match(/(^|\s)[a-zA-Z]{3}($|\s)/g))

// Exercise 02
// Using a regex pattern, remove all of the numbers from the ex2 string.
console.log(ex2.replace(/\d/g, ""))

// Exercise 03
// Using a regex pattern, find the monetary value contained within the ex3 string.
console.log(ex3.match(/\$\d+(\.\d+)?/g)[0])

// Exercise 04
// Using a regex pattern, find the telephone number contained within the ex4 string.
console.log(ex4.match(/\d(\d|\s)*\d/g)[0])

// Exercise 05
// Using a regex pattern, find the email address contained within the ex5 string.
console.log(ex5.match(/\w+@\w+\.\w+/g)[0])
```
#Promises

```
const ride = new Promise((resolve, reject) =>{ // executor: function that resolves a value or rejects (error)
    if(arrived){
        resolve('driver arrived'); // resolve: fulfills promise with passed value
    } else {
        reject('driver bailed'); // reject: operation failed
    }
});

ride
    .then(value => { // then: function that handles fulfillment
        console.log(value); // driver arrived
    })
    .catch(error =>{ // catch: handle rejection
        console.log(error); // driver bailed
    })
    .finally(() => { // if you just want to run some code no matter what you can use finally to handle both possibilities 
        console.log('all settled');
    });

/* ============================================================= */

let p = new Promise((resolve, reject) => {
    let a = 1 + 2;
    if (a == 2) {
        resolve('Success');
    } else {
        reject('Failed');
    }
});

p.then((message) => {
    console.log('This is in the the ' + message);
}).catch((message) => {
    console.log('This is in the catch ' + message);
});

/* ============================================================= */

// Callback Function

const userLeft = false;
const userWatchingCatMeme = true;

function watchTutorialCallback(callback, errorCallback) {
    if (userLeft){
        errorCallback({
            name: 'User Left',
            message: ':('
        });
    } else if(userWatchingCatMeme){
        errorCallback({
            name: 'User Watching Cat Meme',
            message: 'WeDevSimplified < Cat'
        });
    } else{
        callback('Thumbs up and Subscribe');
    }
}

watchTutorialCallback((message) =>{
    console.log('Success: ' + message);
}, (error) => {
    console.log(error.name + ' ' + error.message);
});

// Promises
function watchTutorialPromises(){
    return new Promise((resolve, reject) => {
        if (userLeft){
            reject({
                name: 'User Left',
                message: ':('
            });
        } else if(userWatchingCatMeme){
            reject({
                name: 'User Watching Cat Meme',
                message: 'WeDevSimplified < Cat'
            });
        } else{
            resolve('Thumbs up and Subscribe');
        }
    });
}

watchTutorialPromises().then((message) =>{
    console.log('Promises Success: ' + message);
}).catch((error) => {
    console.log('Promises ' + error.name + ' ' + error.message);
});

/* ============================================================= */

const recordVideoOne = new Promise((resolve, reject) => {
    resolve('Video 1 Recorded');
});

const recordVideoTwo = new Promise((resolve, reject) => {
    resolve('Video 2 Recorded');
});

const recordVideoThree = new Promise((resolve, reject) => {
    resolve('Video 3 Recorded');
});

Promise.all([
    recordVideoOne,
    recordVideoTwo,
    recordVideoThree
]).then((messages) => {
    console.log(messages)
});

Promise.race([ // Ampliar race (retorna la primer promesa en cumplirse, creo (?))
    recordVideoOne,
    recordVideoTwo,
    recordVideoThree
]).then((message) => {
    console.log(message)
});

```
#Promises-Async-Await.js
```
const datos = [{
    id:1,
    title: 'Iron Man',
    year: 2008
},{
    id:2,
    title: 'Spiderman: Homecoming',
    year: 2017
},{
    id:3,
    title: 'Avengers: Endgame',
    year: 2019
}];

// const getDatos = () =>{
//     return datos;
// }; // Es síncrono, la respuesta es inmediata

// const getDatos = () => {
//     setTimeout(() =>{
//         return datos;
//     }, 1500);
// }; // Simulando una peticion web, existe un delay en el retorno de la respuesta, es asincrono.

// console.log(getDatos());

// Promesas
const getDatos = () => {
    return new Promise((resolve, reject) => {
        setTimeout(() =>{
            resolve(datos);
        }, 1500);
    });
    
};

// getDatos()
//     .then((datos) => console.log(datos))

// Async/Await

async function fetchingData(){
    const datosFetched = await getDatos();
    console.log(datosFetched);
}

fetchingData();
```
#TUESDAY

#TYPESCRIPT OBJECT TYPE
```
export type User = {
    name: string;
    age: number;
    occupation: string;
};

export const users: User[] = [
    {
        name: 'Max Mustermann',
        age: 25,
        occupation: 'Chimney sweep'
    },
    {
        name: 'Kate Müller',
        age: 23,
        occupation: 'Astronaut'
    }
];

export function logPerson(user: User) {
    console.log(` - ${user.name}, ${user.age}`);
}

console.log('Users:');
users.forEach(logPerson);
```
#TYPESCRIPT UNION TYPES
```
interface User {
    name: string;
    age: number;
    occupation: string;
}

interface Admin {
    name: string;
    age: number;
    role: string;
}

export type Person = User | Admin;

export const persons: Person[] /* <- Person[] */ = [
    {
        name: 'Max Mustermann',
        age: 25,
        occupation: 'Chimney sweep'
    },
    {
        name: 'Jane Doe',
        age: 32,
        role: 'Administrator'
    },
    {
        name: 'Kate Müller',
        age: 23,
        occupation: 'Astronaut'
    },
    {
        name: 'Bruce Willis',
        age: 64,
        role: 'World saver'
    }
];

export function logPerson(user: Person) {
    console.log(` - ${user.name}, ${user.age}`);
}

persons.forEach(logPerson);
```
#TYPESCRIPT IN OPERATOR4
```
interface User {
    name: string;
    age: number;
    occupation: string;
}

interface Admin {
    name: string;
    age: number;
    role: string;
}

export type Person = User | Admin;

export const persons: Person[] = [
    {
        name: 'Max Mustermann',
        age: 25,
        occupation: 'Chimney sweep'
    },
    {
        name: 'Jane Doe',
        age: 32,
        role: 'Administrator'
    },
    {
        name: 'Kate Müller',
        age: 23,
        occupation: 'Astronaut'
    },
    {
        name: 'Bruce Willis',
        age: 64,
        role: 'World saver'
    }
];

export function logPerson(person: Person) {
    let additionalInformation: string;
    if ('role' in person) {
        additionalInformation = person.role;
    } else {
        additionalInformation = person.occupation;
    }
    console.log(` - ${person.name}, ${person.age}, ${additionalInformation}`);
}

persons.forEach(logPerson);
```
#Find the odd int.
```
function findOdd(A) {
    A = A.sort()
    if(A.length === 1) return A.pop();
    let num = 0, count = 1;
    for(let i = 0, l = A.length; i < l; i++){
    if(A[i] === A[i+1]){
        count++;
    }else{
        if((count % 2) !== 0){
            return A[i]
        }
        count = 1;
    }
    }
    
    return 0;
}
```
#Stop gninnipS My sdroW!.
```
function spinWords(string){
    return string.split(" ")
            .map((word) => {
                if(word.length >= 5) return word.split("").reverse().join("");
                return word;
            }).join(" ");
}
```

#WEDNESDAY

#Array.diff.
```
function arrayDiff(a, b) {
    return a.filter((element) => !b.includes(element));
}
```
#Create Phone Number.
```
function createPhoneNumber(numbers){
    return `(${numbers.slice(0,3).join("")}) ${numbers.slice(3,6).join("")}-${numbers.slice(6,).join("")}`
}
```

#THURSDAY

#Detect Pangram
```
function isPangram(string){
    string  = string.toLowerCase();
    for(let i = 97; i<=122; i++){
        if(!string.includes(String.fromCharCode(i))) return false;
    }
    return true;
}
```

#Find the missin letter.
```
function findMissingLetter(array){
    for(let i =1, l = array.length; i < l; i++){
        if((array[i].charCodeAt() - (array[i-1]).charCodeAt() !== 1)) return String.fromCharCode((array[i].charCodeAt()-1));
    }
}
```

#Find the unique number.
```
function findUniq(arr) {
    let count = 1, unique = 0;
    arr.sort().map((num, i, arr) => {
        num !== arr[i+1] ? (count === 1 ? unique = num : count = 1) : count++;
    });
    return unique;
}
```
#Reverse or rotate?.
```
function revrot(str, sz) {
    if(str === "" || sz > str.length || sz === 0) return "";
    
    let aux = [];
    for(let i = 0, count = Math.trunc(str.length/sz); i < count; i++){
        aux.push(str.slice(i*sz, (i+1)*sz));
    }
    
    return aux.map((chunk) => {
        let a = chunk.split("").reduce((prev, curr) => {
        return prev + Math.pow(Number(curr), 3);
        }, 0);
        
        if(a%2 === 0) return chunk.split("").reverse().join("");
        return chunk.slice(1) + chunk[0];
    }).join("");

}
```
#What's Your Poison?.
```
export function find(rats: number[]): number {
    return rats.reduce((prev, curr) => {
        return prev + Math.pow(2, curr);
    }, 0);
}
```
