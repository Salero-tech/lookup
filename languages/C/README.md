# C snippets



<details>
<summary>Typdef Enum</summary>


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

</details>