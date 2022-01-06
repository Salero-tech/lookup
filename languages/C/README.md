# C snippets
## content:

* [operations](#operations)
* [data types](#datatypes)
* [typdef Enum](#typdef-enum)

<br>
<br>
<br>
<br>





# operations

In C the following Operators exists:
*,+,-,/,%,!,|,||,&,&&,^,~

## number operators
### / devide
Simple division.
<br>
**example:**
10 / 2 = 5


### % modolo <br>
modolo returns the rest of an division. There is no decimal point!
<br>
5 / 2 = 2 &rarr; rest = 1

**example:** <br>
5%5=0
<br>
5%4=1

## logic operators
### **! logical invertion** 
Logical invertion returns the oposit of the local value of the input.

[When is a number true?](#How-to-find-out-if-a-number-is-true-or-false?)

**example:** <br>
!12 = false
<br>
!1 = false
<br>
!0 = true

### **|| logical OR**
Logical OR findsout if one of your two input variables is true.

[When is a number true?](#How-to-find-out-if-a-number-is-true-or-false?)

**example:** <br>
15 || 10 = 1
<br>
5 || 0 = 1
<br>
0 || 0 = 0

### **&& logical AND**
Logical AND findsout if both of your two input variables are true.

[When is a number true?](#How-to-find-out-if-a-number-is-true-or-false?)

**example:** <br>
15 && 10 = 1
<br>
5 && 0 = 0
<br>
0 && 0 = 0


## bit operators
### **~ bit invertion**
Bit invertion inverts the provided variable in binary.
<br>
this means: <br>
1 &rarr; 0
<br>
0 &rarr; 1

**example:** <br>
~0b00000001 = 0b11111110
<br>
~0b00000000 = 0b11111111
<br>
~0b11001111 = 0b00110000

### **| bit OR**
0b10000001 <br>
0b00110000 <br>
&darr;&darr;&darr;&darr;&darr;&darr;&darr;&darr;&darr; <br>
0b10110001 <br>
Every where where the first or the second number has a 1 the result will have one too.

**example:** <br>
0b10000001 | 0b00110000 = 0b10110001
<br>
0b10000001 | 0b10000001 = 0b10000001
<br>
0b00000000 | 0b10000001 = 0b10000001

### **& bit AND**
0b10000001 <br>
0b10110000 <br>
&darr;&darr;&darr;&darr;&darr;&darr;&darr;&darr;&darr; <br>
0b10000000 <br>
Every where where the first and the second number has a 1 the result will have one too.

**example:** <br>
0b10000001 & 0b10110000 = 0b10000000
<br>
0b10000001 & 0b00000000 = 0b00000000
<br>
0b10101001 & 0b00110001 = 0b00100001

### **^ bit EXOR**
0b10000001 <br>
0b10110000 <br>
&darr;&darr;&darr;&darr;&darr;&darr;&darr;&darr;&darr; <br>
0b00110001 <br>
basicly the first number is the output but every where where the second number has a 1 the bit will be inverted

**example:** <br>
0b10000001 ^ 0b10110000 = 0b00110001




# data types

## bool
## How to find out if a number is true or false?: <br>
**A number is false when it is not 0!**
otherwise its true!


# typdef enum

``` C
typedef enum {
    ON, OFF, PLAY
}state_t; //state_t can be used to create a variable that holds the previous defined states

//create variable
state_t	state = ON;
```
## Numbering
The First *define (ON)* in the list will receive the number 1 (int). The next 2 and so on. <br>
<br>
You can start at a custom number the following way:
 ``` C
typedef enum {
    ON = 10, OFF, PLAY
}state_t;

```


## Attention
This might not work depending on your compiler
``` C
    variable++;
```
