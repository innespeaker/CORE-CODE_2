# CORE-CODE_2
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
