# Pattern Questions:

### How to approach:

Only three approach to solve pattern problems:
1. no.of lines = no.of rows = no.of times outer loop will run
2. Identify for every row no.
* How many colums are there.
* Types of elements in column (*, #, +) or so on.
3. What do you need to print (*, #) or any things.







Print these patterns using loops:

1.  
```
    *****
    *****
    *****
    *****
    *****
```

```javascript
// Ans: 1
const printPattern = function (n) {
  for (let row = 1; row <= n; row++) {
    // for every row, run the col
    let pattern = '';
    for (let col = 1; col <= n; col++) {
      pattern += '*';
    }
    console.log(pattern);
  }
};

printPattern(5);
```


2.  
```
    *
    **
    ***
    ****
    *****
```

```javascript
// Ans: 2
const printPattern = function (n) {
  for (let row = 1; row <= n; row++) {
    // for every row, run the col
    let pattern = '';
    for (let col = 1; col <= row; col++) {
      pattern += '*';
    }
    console.log(pattern);
  }
};

printPattern(5);
```


3.  
```
    *****
    ****
    ***
    **
    *
```

```javascript
const printPattern = function (n) {
  for (let row = 1; row <= n; row++) {
    // for every row, run the col
    let pattern = '';
    for (let col = 1; col <= n - row + 1; col++) {
      pattern += '*';
    }
    console.log(pattern);
  }
};

printPattern(5);

// same
const printPattern = function (n) {
  for (let row = 1; row <= n; row++) {
    // for every row, run the col
    let pattern = '';
    for (let col = row; col <= n; col++) {
      pattern += '*';
    }
    console.log(pattern);
  }
};

printPattern(5);
```


4.  
```
    1
    1 2
    1 2 3
    1 2 3 4
    1 2 3 4 5
```

```javascript
const printPattern = function (n) {
  for (let row = 1; row <= n; row++) {
    // for every row, run the col
    let pattern = '';
    for (let col = 1; col <= row; col++) {
      pattern += col;
    }
    console.log(pattern);
  }
};

printPattern(5);
```


5.  *
    **
    ***
    ****
    *****
    ****
    ***
    **
    *


6.       *
        **
       ***
      ****
     *****


7.   *****
      ****
       ***
        **
         *


8.      *
       ***
      *****
     *******
    *********


9.  *********
     *******
      *****
       ***
        *


10.      *
        * *
       * * *
      * * * *
     * * * * *


11.  * * * * *
      * * * *
       * * *
        * *
         *


12.  * * * * *
      * * * *
       * * *
        * *
         *
         *
        * *
       * * *
      * * * *
     * * * * *


13.      *
        * *
       *   *
      *     *
     *********


14.  *********
      *     *
       *   *
        * *
         *


15.      *
        * *
       *   *
      *     *
     *       *
      *     *
       *   *
        * *
         *


16.           1
            1   1
          1   2   1
        1   3   3   1
      1   4   6   4   1


17.      1
        212
       32123
      4321234
       32123
        212
         1


18.   **********
      ****  ****
      ***    ***
      **      **
      *        *
      *        *
      **      **
      ***    ***
      ****  ****
      **********


19.    *        *
       **      **
       ***    ***
       ****  ****
       **********
       ****  ****
       ***    ***
       **      **
       *        *


20.    ****
       *  *
       *  *
       *  *
       ****

21.    1
       2  3
       4  5  6
       7  8  9  10
       11 12 13 14 15

22.    1
       0 1
       1 0 1
       0 1 0 1
       1 0 1 0 1

23.        *      *
         *   *  *   *
       *      *      *

24.    *        *
       **      **
       * *    * *
       *  *  *  *
       *   **   *
       *   **   *
       *  *  *  *
       * *    * *
       **      **
       *        *

25.       *****
         *   *
        *   *
       *   *
      *****

26.   1 1 1 1 1 1
      2 2 2 2 2
      3 3 3 3
      4 4 4
      5 5
      6

27.   1 2 3 4  17 18 19 20
        5 6 7  14 15 16
          8 9  12 13
            10 11

28.      *
        * *
       * * *
      * * * *
     * * * * *
      * * * *
       * * *
        * *
         *

29.      
       *        *
       **      **
       ***    ***
       ****  ****
       **********
       ****  ****
       ***    ***
       **      **
       *        *

30.         1
          2 1 2
        3 2 1 2 3
      4 3 2 1 2 3 4
    5 4 3 2 1 2 3 4 5


31.      4 4 4 4 4 4 4  
         4 3 3 3 3 3 4   
         4 3 2 2 2 3 4   
         4 3 2 1 2 3 4   
         4 3 2 2 2 3 4   
         4 3 3 3 3 3 4   
         4 4 4 4 4 4 4   

32.    E
       D E
       C D E
       B C D E
       A B C D E

33.    a
       B c
       D e F
       g H i J
       k L m N o
     
34.    E D C B A
       D C B A
       C B A
       B A
       A
       
35.    1      1
       12    21
       123  321
       12344321