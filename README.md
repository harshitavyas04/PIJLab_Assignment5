# PIJLab_Assignment5
Part 1:

Problem Statement:

Implement the generic Shapes class as an interface s so that we can implement concrete classes like circle, triangle, rectangle class from it.

Description:

The provided description outlines the implementation of three different shapes (Circle, Triangle, and Rectangle) in Java, following an interface named `Shape`. Each shape class has its constructor and implements the `area()` and `perimeter()` methods as specified in the `Shape` interface.

Here is a summary of each shape's implementation:

1. **Circle:**
   - Constructor: Takes the radius as a parameter.
   - Methods:
      - area(): Calculates the area using the formula \( \pi \times \text{radius} \times \text{radius} \).
      - perimeter(): Calculates the perimeter using the formula \( 2 \times \pi \times \text{radius} \).

2. **Triangle:**
   - Constructor: Takes the base, height, side1, and side2 as parameters.
   - Methods:
      - area(): Calculates the area using the formula \( 0.5 \times \text{base} \times \text{height} \).
      - perimeter(): Calculates the perimeter using the formula \( \text{base} + \text{side1} + \text{side2} \).

3. **Rectangle:**
   - Constructor: Takes the length and width as parameters.
   - Methods:
      - area(): Calculates the area using the formula \( \text{length} \times \text{width} \).
      - perimeter(): Calculates the perimeter using the formula \( 2 \times (\text{length} + \text{width}) \).

**Main Class:**
   - Contains the main() method, the program's entry point.
   - Prompts the user to select a shape and enter the required parameters.
   - Uses a switch statement to determine the selected shape and creates an instance of that shape.
   - Calls the area() and perimeter() methods on the created shape and displays the results.
   - Utilizes the Scanner class to read input from the user and closes the scanner when the program is finished.

Overall, this program allows users to interactively select a shape, input its parameters, and receive the calculated area and perimeter.

Part 2:

Problem Statement: Implement Employee as an abstract and derive 2 classes such as NormalEmployee and BonusEmployee from it and perform the salary calculations based on the formulas as per the excel attachment

Description:

  - Employee: This is an abstract class containing details of an employee such as name, designation, department, bank name, date of joining, employee ID, total working days, loss of pay days, leaves taken, account number, UAN, PF number, ESINo, gross wage, basic wage, hra, conveyance allowance, medical allowance, other allowance, EPF, health insurance amount, PT, loan recovery, total deductions, net salary, total earnings, bonus, and bonus salary. It also contains getter and setter methods for all these fields.
  - NormalEmployee: This class extends the Employee class and contains the method theMonthly() to calculate the net salary of a normal employee. It calculates basic wage, hra, conveyance allowance, medical allowance, other allowance, total earnings, EPF, health insurance amount, PT, loan recovery, and total deductions based on the gross wage, total working days, loss of pay days, and other details provided.
  - BonusEmployee: This class also extends the Employee class and contains the method theMonthly() to calculate the net salary of a bonus employee. It calculates basic wage, hra, conveyance allowance, medical allowance, other allowance, total earnings, EPF, health insurance amount, PT, loan recovery, and total deductions based on the gross wage, total working days, loss of pay days, and other details provided. Additionally, it also calculates the bonus salary.
  - Main: This class contains the main method and takes inputs for gross wage, total working days, loss of pay days, and bonus (if any) from the user. It creates an object of NormalEmployee or BonusEmployee based on the bonus input and calls the theMonthly() method to calculate the net salary. It then prints the payslip with all the details using the printPaySlip() method.
  - printPaySlip(): This method prints the payslip for the employee with all the details such as employee name, ID, designation, department, date of joining, bank name, account number, gross wage, total working days, loss of pay days, allowances, deductions, and net salary. It also checks and prints whether the employee is a normal or bonus employee.
