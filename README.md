# Arithmetic-operation-using-8086
# 8086 Assembly Language Programs for Arithmetic Operations

## AIM

To write and execute Assembly Language Programs to perform arithmetic operations for the 8086 microprocessor.

---

## APPARATUS REQUIRED

* Personal Computer with MASM Software

---

## 1. ADDITION

#### Algorithm

1. Initialize memory location in HL register.
2. Store 1st data.
3. Increment HL to enter 2nd data.
4. Move 2nd number to accumulator.
5. Decrement HL.
6. Add value in memory with accumulator.
7. Store result.
8. Stop.


## FLOW CHART
<img width="707" height="1024" alt="image" src="https://github.com/user-attachments/assets/b5a7062d-e294-47cd-9683-a40de25e82de" />


#### Program

```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,2000H
MOV CL,00H
MOV AX,[SI]
MOV BX,[SI+02H]
ADD AX,BX
JNC L1
INC CL
L1:
MOV [SI+04H],AX
MOV [SI+06H],CL
MOV AH,4CH
INT 21H
CODE ENDS
END
```

#### Output Table

<img width="644" height="246" alt="image" src="https://github.com/user-attachments/assets/e4cb0271-96e7-410f-ab5f-8a2bfc412ef7" />


#### Manual Calculations

<img width="803" height="584" alt="image" src="https://github.com/user-attachments/assets/5527aea1-cf2b-4f7f-9633-46cd1dfdfd87" />


---

## OUTPUT IMAGE FROM MASM SOFTWARE
![roshan 1 prog](https://github.com/user-attachments/assets/6678a4f8-11f3-4d04-ad02-735519488f6e)
![roshan1 out](https://github.com/user-attachments/assets/f406143d-a77d-4b4b-9336-f49a18919765)



## 2. SUBTRACTION

#### Algorithm

1. Initialize memory and store 1st data.
2. Increment to get 2nd data.
3. Move 2nd data to accumulator.
4. Subtract memory content.
5. Store result.

## FLOWCHART

<img width="578" height="797" alt="image" src="https://github.com/user-attachments/assets/564c3c7a-33ce-4a1c-8920-beb5c24b9b47" />


#### Program



#### Output Table

<img width="646" height="241" alt="image" src="https://github.com/user-attachments/assets/0d6cc0ba-559f-425e-a8c3-a68619a73d97" />


#### Manual Calculations

<img width="603" height="614" alt="image" src="https://github.com/user-attachments/assets/01fe497b-d7d0-4887-84f2-a55315fa231e" />


---


## OUTPUT SCREEN FROM MASM SOFTWARE
![WhatsApp Image 2025-09-06 at 9 34 13 AM](https://github.com/user-attachments/assets/2939bb8e-c7d8-4ce0-9c51-a00d7fd2d835)
![WhatsApp Image 2025-09-06 at 9 34 14 AM](https://github.com/user-attachments/assets/2530d0ba-878d-488d-a5a8-1cf18a2ac276)



## 3. MULTIPLICATION

#### Algorithm

1. Initialize memory and store operands.
2. Move operands to registers.
3. Multiply.
4. Store result.

##FLOWCHART

<img width="569" height="906" alt="image" src="https://github.com/user-attachments/assets/88be88ff-2896-4a88-b73d-84ccffd2fcf9" />



#### Program

```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,2000H
MOV DX,0000H
MOV AX,[SI]
MOV BX,[SI+02H]
MUL BX
MOV [SI+04H],AX
MOV [SI+06H],DX
MOV AH,4CH
INT 21H
CODE ENDS
END
```

#### Output Table

<img width="496" height="191" alt="image" src="https://github.com/user-attachments/assets/c83edd02-78f7-4c3f-94ff-fc9b830daa81" />


#### Manual Calculations

<img width="580" height="561" alt="image" src="https://github.com/user-attachments/assets/c7207d2b-05fd-4049-a835-4ec39e2371d6" />


---

## OUTPUT SCREEN FROM MASM SOFTWARE
![WhatsApp Image 2025-09-06 at 9 34 14 AM (1)](https://github.com/user-attachments/assets/3aec26b5-7439-453f-badb-c2964533b853)
![WhatsApp Image 2025-09-06 at 9 34 14 AM (2)](https://github.com/user-attachments/assets/12ca66ed-cbc7-4153-8310-4887ac281c9e)


## 4. DIVISION

#### Algorithm

1. Load memory location of operands.
2. Perform division.
3. Store result.

   ## FLOWCHART
<img width="1065" height="802" alt="image" src="https://github.com/user-attachments/assets/25b4a483-0d42-494b-8639-1af3ea17191b" />


#### Program

```asm
CODE SEGMENT
ASSUME CS: CODE, DS: CODE
ORG 1000H
MOV SI,2000H
MOV DX,0000H
MOV AX,[SI]
MOV BX,[SI+02H]
DIV BX
MOV [SI+04H],AX
MOV [SI+06H],DX
MOV AH,4CH
INT 21H
CODE ENDS
END
```

#### Output Table

<img width="508" height="192" alt="image" src="https://github.com/user-attachments/assets/a283f261-e314-42b2-9fb1-e9377143d3b4" />


#### Manual Calculations

<img width="603" height="518" alt="image" src="https://github.com/user-attachments/assets/718527fe-ad4c-4666-8928-1bdcf641bbef" />


---
## OUTPUT FROM MASM SOFTWARE
![WhatsApp Image 2025-09-06 at 9 34 16 AM](https://github.com/user-attachments/assets/f319c1f8-9401-4689-b499-6212d7976311)
![WhatsApp Image 2025-09-06 at 9 34 16 AM (1)](https://github.com/user-attachments/assets/9aabd728-41a3-49b7-8c08-e1d0c2492df9)





## RESULT

Thus, the Assembly Language Programs for 8086 to perform arithmetic operations (Addition, Subtraction, Multiplication, and Division) using both direct and indirect methods were successfully written and executed using MASM.
