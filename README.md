## 1. Check Even or Odd Number

Design an algorithm and flowchart that take a number as input and
determine whether it is even or odd.

### ✔ Pseudocode

```text
START
    INPUT number
    IF number % 2 == 0 THEN
        PRINT Even
    ELSE
        PRINT Odd
    ENDIF
END
```

### ✔ Flowchart

```mermaid
graph TD
    A([Start]) --> I[/Get input N/]
    I --> B{N % 2 == 0 ?}
    B -->|Yes| C[/Print Even/]
    B -->|No| D[/Print Odd/]
    C --> E([End])
    D --> E([End])
```

---

## 2. Calculate Total and Average Marks

Write the algorithm and draw the flowchart for a program that inputs
marks for 3 subjects, calculates the total and average, and displays
both.
### ✔ Pseudocode
```text
START
    INPUT mark1, mark2, mark3
    total = mark1 + mark2 + mark3
    average = total / 3
     PRINT total
     print average
    
END
```
### ✔ Flowchart
```mermaid
    graph TD
    Start([Start]) --> Input[/Input mark1, mark2, mark3/]
    Input --> Calc[total = mark1 + mark2 + mark3]
    Calc --> Output[/Print total/]
    Output --> End([End])
    
```

---

## 3. Display Multiplication Table

Create an algorithm and flowchart that input a number and display its
multiplication table from 1 to 10 using a loop.

### ✔ Pseudocode
```text
START

INPUT number
counter = 1
WHILE counter <= 10 DO
result = number * counter
PRINT number + " x " + counter + " = " + result
counter = counter + 1
ENDWHILE

END
```
### ✔ Flowchart
```mermaid
graph TD
    Start([Start]) --> Input[/Input number/]
    Input --> Init[counter = 1]
    Init --> Loop{counter <= 10?}
    Loop -- Yes --> Calc[result = number * counter]
    Calc --> Output[/Print number x counter = result/]
    Output --> Increment[counter = counter + 1]
    Increment --> Loop
    Loop -- No --> End([End])

```

---

## 4. Positive, Negative, or Zero Check

Write the algorithm and flowchart to input a number and display whether
it is positive, negative, or zero.
### ✔ Pseudocode

```text

START
   INPUT number
   IF number > 0 THEN
   PRINT "positive"
   ELSE IF number < 0 THEN
   PRINT "negative"
   ELSE
   PRINT "zero"
   ENDIF
    
END

```
### ✔ Flowchart

```mermaid
graph TD
    Start([Start]) --> Input[/Input number/]
    Input --> CheckPos{number > 0?}
    CheckPos -- Yes --> PrintPos[/Print 'Positive'/]
    CheckPos -- No --> CheckNeg{number < 0?}
    CheckNeg -- Yes --> PrintNeg[/Print 'Negative'/]
    CheckNeg -- No --> PrintZero[/Print 'Zero'/]
    PrintPos --> End([End])
    PrintNeg --> End
    PrintZero --> End

```

---

## 5. Simple Interest Calculator

Create an algorithm and flowchart for a program that calculates simple
interest using the formula:

**SI = (P × R × T) / 100**

- **P = Principal** → original amount of money
- **R = Rate of Interest** → percentage per year
- **T = Time** → number of years

### ✔ Pseudocode
```text
START
INPUT P, R, T 
SI = (P * R * T) / 100
PRINT SI
END
```
### ✔ Flowchart
```mermaid
graph TD
    Start([Start]) --> Input[/Input P, R, T/]
    Input --> Calc[SI = P * R * T / 100]
    Calc --> Output[/Print SI/]
    Output --> End([End])

```

---

## 6. Average Temperature Calculation

Write the algorithm and draw the flowchart for a program that takes the
temperature of 7 days, finds the average temperature, and displays it.

### ✔ Pseudocode
```text
START
totalTemp = 0
counter = 1
WHILE counter <= 7 DO
INPUT temp
totalTemp = totalTemp + temp
counter = counter + 1
ENDWHILE
avgTemp = totalTemp / 7
PRINT avgTemp
END
```
### ✔ Flowchart
```mermaid
graph TD
    Start([Start]) --> Init[totalTemp = 0<br/>counter = 1]
    Init --> Loop{counter <= 7?}
    Loop -- Yes --> Input[/Input temp/]
    Input --> Calc[totalTemp = totalTemp + temp<br/>counter = counter + 1]
    Calc --> Loop
    Loop -- No --> Avg[avgTemp = totalTemp / 7]
    Avg --> Output[/Print avgTemp/]

```

---

## 7. Calculate Area of a Rectangle

Create an algorithm and flowchart to input length and width, calculate
the area (**Area = Length × Width**), and display the result.

### ✔ Pseudocode
```text
START
INPUT length, width
area = length * width
PRINT area
END
```

### ✔ Flowchart
```mermaid
graph TD
    Start([Start]) --> Input[/Input length, width/]
    Input --> Calc[area = length * width]
    Calc --> Output[/Print area/]
    Output --> End([End])
```

## 8. 

Write the algorithm and draw the flowchart for a program that takes a
student's average marks and displays **"Pass"** if average ≥ 50,
otherwise **"Fail"**.

### ✔ Pseudocode
```text
START
INPUT average
IF average >= 50 THEN
PRINT "Pass"
ELSE
PRINT "Fail"
ENDIF
END
```
### ✔ Flowchart
```mermaid
graph TD
    Start([Start]) --> Input[/Input average/]
    Input --> Check{average >= 50?}
    Check -- Yes --> Pass[/Print 'Pass'/]
    Check -- No --> Fail[/Print 'Fail'/]
    Pass --> End([End])
    Fail --> End

```
---
```
## 9. Calculate Factorial of a Number

Write the algorithm and draw the flowchart that input a number and
calculate its factorial using a loop.

### ✔ Pseudocode
```text
START
INPUT number
factorial = 1
counter = 1
WHILE counter <= number DO
factorial = factorial * counter
counter = counter + 1
ENDWHILE
PRINT factorial
END
```
### ✔ Flowchart
```mermaid
graph TD
    Start([Start]) --> Input[/Input number/]
    Input --> Init[factorial = 1<br/>counter = 1]
    Init --> Loop{counter <= number?}
    Loop -- Yes --> Calc[factorial = factorial * counter<br/>counter = counter + 1]
    Calc --> Loop
    Loop -- No --> Output[/Print factorial/]
    Output --> End([End])

```
---

## 10. Calculate Discount on Purchase

Write the algorithm and draw the flowchart for a program that inputs the
purchase amount and gives a **10% discount** if the amount is greater
than 1000.

### ✔ Pseudocode
```text
START
INPUT purchaseAmount
IF purchaseAmount > 1000 THEN
discount = purchaseAmount * 0.10
purchaseAmount = purchaseAmount - discount
ENDIF
PRINT purchaseAmount
END

```
### ✔ Flowchart
```mermaid
graph TD
    Start([Start]) --> Input[/Input purchaseAmount/]
    Input --> Check{purchaseAmount > 1000?}
    Check -- Yes --> Disc[discount = purchaseAmount * 0.10<br/>purchaseAmount = purchaseAmount
 - discount]
    Check -- No --> Output
    Disc --> Output[/Print purchaseAmount/]
    Output --> End([End])

```

---
