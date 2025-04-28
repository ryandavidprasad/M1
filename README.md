# EX-01-Datatypes-Operators  
## AIM:  
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## PROGRAM:
```c
#include <stdio.h>
int main() {
    char ch1, ch2, ch3;
    scanf(" %c", &ch1);
    scanf(" %c", &ch2);
    scanf(" %c", &ch3);
    printf("%c %c %c\n", ch3, ch2, ch1);
    return 0;
}
```

## OUTPUT:
```
Input:
A
B
C
Output:
C B A
```

## RESULT:  
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02-Conditional-Statements  
## AIM:  
Write a C program to read A value and check whether A is positive number or not.

## PROGRAM:
```c
#include <stdio.h>
int main() {
    int A;
    scanf("%d", &A);
    if (A > 0) {
        printf("A is a positive number.\n");
    } else {
        printf("A is not a positive number.\n");
    }
    return 0;
}
```

## OUTPUT:
```
Input:
5
Output:
A is a positive number.
```
or
```
Input:
-3
Output:
A is not a positive number.
```

## RESULT:  
Thus the program to read A values and check whether A is positive number or not has been executed successfully.


# EX-03-Operators-Expressions  
## AIM:  
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## PROGRAM:
```c
#include <stdio.h>
int main() {
    int num1, den1, num2, den2;
    float frac1, frac2, min;
    scanf("%d%d", &num1, &den1);
    scanf("%d%d", &num2, &den2);
    frac1 = (float)num1 / den1;
    frac2 = (float)num2 / den2;
    min = (frac1 < frac2) ? frac1 : frac2;
    printf("Minimum fraction value: %.2f\n", min);
    return 0;
}
```

## OUTPUT:
```
Input:
1 2
2 3
Output:
Minimum fraction value: 0.50
```

## RESULT:  
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.


# EX-04-Using Conditional Statements  
## AIM:  
Write a C program to check whether the input value is equal to 1 using simple if statement.

## PROGRAM:
```c
#include <stdio.h>
int main() {
    int value;
    scanf("%d", &value);
    if (value == 1) {
        printf("The input value is equal to 1.\n");
    } else {
        printf("The input value is not equal to 1.\n");
    }
    return 0;
}
```

## OUTPUT:
```
Input:
1
Output:
The input value is equal to 1.
```
or
```
Input:
5
Output:
The input value is not equal to 1.
```

## RESULT:  
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully.

---

# EX-05-Calculating Total, Percentage, And Division Using Conditional Statements  
## AIM:  
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division.

## PROGRAM:
```c
#include <stdio.h>
int main() {
    int m1, m2, m3;
    float tot, per;
    scanf("%d%d%d", &m1, &m2, &m3);
    tot = m1 + m2 + m3;
    per = tot / 3;
    printf("Total Marks: %.2f\n", tot);
    printf("Percentage: %.2f%%\n", per);
    if (m1 >= 40 && m2 >= 40 && m3 >= 40) {
        if (per >= 60) {
            printf("Division = First\n");
        } else if (per >= 48) {
            printf("Division = Second\n");
        } else if (per >= 36) {
            printf("Division = Pass\n");
        } else {
            printf("Division = Fail\n");
        }
    } else {
        printf("Division = Fail\n");
    }
    return 0;
}
```

## OUTPUT:
```
Input:
70 65 80
Output:
Total Marks: 215.00
Percentage: 71.67%
Division = First
```
or
```
Input:
40 45 50
Output:
Total Marks: 135.00
Percentage: 45.00%
Division = Pass
```
or
```
Input:
30 55 60
Output:
Total Marks: 145.00
Percentage: 48.33%
Division = Fail
```

## RESULT:  
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.



