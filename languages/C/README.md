# C snippets
## content:

<br>
<br>
<br>
<br>





# Operations

In C the following Operators exists:
*,+,-,/,%,!,|,||,&,&&,^,~

## Number Operators
### devide /
### modolo %  
5%5=0  5%4=1  ergebnis ist der rest der / operation
## Logic Operators
### **!** 
//logisch invertieren -> !10 = 0 //ist die zahl nicht null so wird die zahl 0 gesetzt. sonst 1
### **||**
//logisch ODER -> 10 || 10 = 1 wenn einer der werte nicht 0 ist ist die ausgabe 1. sonst 0
### **&&**
//logisch UND -> 10 && 10 = 1 wenn einer der werte 0 ist, ist die ausgabe 0. sonst 1
## Bit Operators
### **|**
//bitweise ODER -> 0b10000001 | 0b00110000 = 0b10110001 // die 1 aus der ersten zahl werden auf die  zweite übertragen
### **&**
//bitweise UND -> 0b00000111 & 0b00000101 = 0b00000101 // wenn nicht in beiden zahlen eine eins an der stelle steht wird ein 0 gesetzt
### **~**
//bitweise invertieren -> ~0b00000001 = 0b11111110
### **^**
//bitweise EXOR -> 0b00000010 ^ 0b00000011 = 0b00000001 //es werden die mit 1 makierten bits invertiert



# Typdef Enum

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
