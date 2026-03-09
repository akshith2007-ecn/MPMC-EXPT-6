AIM:-

To write and execute an Assembly language program to perform the factorial of a number using 8051 Keil.

APPARATUS REQUIRED:-

Personal computer with Keil software

ALGORITHM:-

1.Start

2.Input: Read the number n.

3.Initialize:

Set factorial to 1.

Set i to 1.

4.Loop: While i is less than or equal to n:

Multiply factorial by i.

FLOWCHART:-

<img width="506" height="525" alt="image" src="https://github.com/user-attachments/assets/26e3349e-d546-4155-b56d-54d374ba53a8" />

PROGRAM:-

ORG 0000H

MOV DPTR,#4500H

MOVX A,@DPTR

MOV R0,A

INC DPTR

ACALL FACTORIAL

MOVX @DPTR,A

SJMP THIN

FACTORIAL:DEC R0

CJNE R0,#01H,PRODUCT

SJMP THICK

PRODUCT:MOV B,R0

MUL AB

ACALL FACTORIAL

THICK: RET

THIN:RET

END

OUTPUT:-

<img width="1688" height="732" alt="image" src="https://github.com/user-attachments/assets/d909c661-0e22-44a2-9319-9565b24d8717" />

MANUAL CALCULATION:-

<img width="1600" height="892" alt="image" src="https://github.com/user-attachments/assets/f2d70d71-724a-4583-b380-3e2062abe337" />

RESULT:-

Thus, the factorial of a number was calculated and executed successfully using 8051 Keil.






Increment i by 1.

5.Output: Store or print the value of factorial.

End
