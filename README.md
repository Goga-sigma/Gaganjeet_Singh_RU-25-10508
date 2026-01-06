**Project Title**

Electricity Bill Calculator in C

**1. Project Details**
- Topic: Electricity Bill Calculator (Slab-wise billing)
- Language Used: C
- Concepts Used: Input/Output, Variables, if–else ladder, arithmetic operations
- Tools/IDE: VS Code (or any C IDE), GCC/MinGW compiler
- Type of Project: Console-based utility program

The program calculates the total electricity bill based on the number of units consumed, using different rates for different slabs and adding fixed extra charges.

**2. Aim of the Project**

The aim of this project is to:
- Develop a simple electricity bill calculator using the C programming language.
- Implement slab-wise billing logic using an if–else ladder.
- Add a fixed extra charge to the calculated amount.
- Display the final bill amount in a clear and formatted way to the user.

**3. Features of the Project**
User Input:
- Takes the total number of units consumed from the user using scanf().

Slab-wise Billing:
- Uses three slabs with different rates:
  - 0–100 units → ₹5 per unit
  - 101–200 units → ₹7 per unit
  - Above 200 units → ₹10 per unit

Fixed Extra Charges:

- Adds a fixed extra charge of ₹50 to every bill (extra_charges = 50.0).

Validation:

- Checks if the entered units are negative and prints an error message if so.

Clear Output Format:

- Prints:
  - Units consumed
  - Energy charges (calculated from slabs)
  - Extra charges
  - Total bill amount

Simple and Easy to Understand:
- Code is small, clear, and suitable for beginners in C.

**4. Why I Made This Project**
- To practice basic C programming concepts like input/output, conditions, and operators.
- To understand how real-life billing systems (like electricity boards) use slab-based rates.
- To build a small but practical utility that looks like a real-world application.
- To have a simple project that can be uploaded to GitHub and shown in college/school as a mini-project.

**5. Learning Outcomes**

By making this project, I learned:

1. Basic C Syntax:
   - How to use printf() and scanf() for input and output.
   - How to declare and use different data types (int, float).

2. Conditional Statements:
   - How to use an if–else ladder to handle multiple conditions (different slabs).
   - How to apply different logic based on range of values.

3. Arithmetic and Slab Calculation:
   - How to break down a total value (units) into multiple slabs.
   - How to calculate step-by-step bill amounts for each part of the units.

4. Error Handling:
   - How to check for invalid input (like negative units) and stop the program.

5. Formatting Output:
   - Using %.2f to print floating values up to 2 decimal places.
   - Designing an output that looks like a mini bill / receipt.

6. Project Structuring:
   - How to convert a simple idea into a complete project with aim, features, and documentation.

**6. How This Project Was Made**

1. Problem Understanding:
   - Objective: Given the number of units consumed, calculate the electricity bill using slab-wise rates plus a fixed extra charge.

2. Planning the Slabs and Rates:
   - I decided the following slab rates:
     - First 100 units → ₹5 per unit (rate1 = 5.0)
     - Next 100 units (101–200) → ₹7 per unit (rate2 = 7.0)
     - Above 200 units → ₹10 per unit (rate3 = 10.0)
   - Fixed extra charge: extra_charges = 50.0

3. Designing the Logic (Algorithm):
   - Step 1: Take units as input.
   - Step 2: If units < 0 → print error and exit.
   - Step 3: If units ≤ 100 → bill = units × rate1.
   - Step 4: Else if units ≤ 200 →
bill = (100 × rate1) + (units − 100) × rate2.
   - Step 5: Else (units > 200) →
bill = (100 × rate1) + (100 × rate2) + (units − 200) × rate3.
   - Step 6: final_amount = bill_amount + extra_charges.
   - Step 7: Print all details.

4. Coding in C:
   - Declared variables: units, bill_amount, final_amount, extra_charges, rate1, rate2, rate3.
   - Wrote the if–else ladder for slab checking.
   - Calculated bill_amount based on slabs.
   - Added extra charges and stored in final_amount.

5. Testing:
   - Tested with different values of units:
     - units = 50 → only first slab.
     - units = 150 → first + second slab.
     - units = 250 → all three slabs.
     - units = −10 → invalid input check.

6. Final Touches:
   - Added a header line: "----- ELECTRICITY BILL -----".
   - Printed the values in a clean and formatted way.

**7. Utilities / Uses of the Project**

- Can be used as a learning tool to understand:
  - Slab-based billing
  - Conditional logic in C

- Can serve as a mini-project for:
  - School / College practicals
  - Internal assessments
  - Portfolio / GitHub profile

- Can be easily modified to:
  - Change slab rates and charges according to different electricity boards.
  - Add more slabs or different types of charges.

- Good example of:
  - Turning a real-life scenario (electricity bill) into a programming problem.

**8. Future Scope of the Project**

This simple project can be extended in many ways:

1. More Slabs and Dynamic Rates:
   - Add more slabs (e.g., above 500 units, separate rate).
   - Allow user to enter slab rates instead of fixing them in code.

2. Tax and GST:
   - Add percentage-based charges like tax, GST, surcharge, etc.

3. User Details:
   - Add input for:
     - Customer name
     - Customer ID
     - Address / City
     - Print these details on the bill.

4. Different Consumer Categories:
  - Domestic, Commercial, Industrial – each with different rate structures.

5. File Handling:
  - Save the generated bill in a text file (e.g., bill.txt).
  - Maintain a history of bills.

6. Menu-Driven Program:
  - Create a menu:
    - Calculate new bill
    - View rate chart
    - Exit

7. GUI / Web Version (Advanced):
  - Later convert this logic into:
    - A GUI application using other languages.
    - A web-based tool using HTML/CSS/JS with backend.

**9. Output(screenshot).**

