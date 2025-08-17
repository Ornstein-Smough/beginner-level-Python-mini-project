General Best Practices for Commenting
	1.	File-level documentation (docstring or block comment):
	•	State the overall purpose of the file.
	•	List the key features or modules (temperature converter, calculator, etc.).
	•	Optionally include author and date.
	2.	Function-level documentation (docstring inside each function):
	•	One or two sentences describing what the function does.
	•	List inputs (user choices, numbers).
	•	List outputs (printed results, return values if any).
	3.	Inline comments within functions:
	•	Explain non-obvious logic or formulas.
	•	Justify validation checks (e.g., division by zero, negative values).
	•	Clarify steps in sequence (for example: first read input, then compute, then display result).
	4.	Main program section:
	•	Separate with a comment header (e.g., # Main program loop).
	•	Describe how the menu system works.
	•	Make it clear this is the entry point of the program.

⸻

How to Comment Each Part of This Project

1. File Header

At the very top of the file, add a descriptive block comment or docstring such as:
	•	Purpose of the program (practice project for Python basics).
	•	Overview of included modules: temperature conversion, calculator, time conversion, unit converter.
	•	Instructions: how to run the file.

⸻

2. Temperature Converter
	•	Function-level docstring: Explain it converts between Celsius and Fahrenheit depending on user choice.
	•	Inputs: User provides a letter (C or F) and a numeric temperature.
	•	Outputs: The converted temperature.
	•	Inline comments should explain:
	•	Why you check the user’s choice.
	•	The formula being applied (C → F or F → C).
	•	Why you wrap input parsing in try/except (to catch invalid numbers).

⸻

3. Simple Calculator
	•	Function-level docstring: State that it performs basic arithmetic operations.
	•	Inputs: Two numbers and an operation choice.
	•	Outputs: Result of the chosen operation.
	•	Inline comments:
	•	Before showing the operations menu, state its purpose.
	•	When checking division, explain why dividing by zero is not allowed.
	•	When catching invalid input, explain that it prevents program crashes.

⸻

4. Seconds Converter
	•	Function-level docstring: State that it converts total seconds into hours, minutes, and seconds.
	•	Inputs: An integer number of seconds.
	•	Outputs: Time in h:m:s format.
	•	Inline comments:
	•	Explain the integer division for hours and minutes.
	•	Note why you check that seconds are non-negative.
	•	State that input must be an integer.

⸻

5. Unit Converter
	•	Function-level docstring: State it can convert between currency, length, and weight.
	•	Inputs: A numeric value depending on choice.
	•	Outputs: Converted value.
	•	Inline comments:
	•	For each choice (currency, length, weight), explain what unit conversion is being done.
	•	Document why negative values are rejected.
	•	State that numbers are validated with try/except.

⸻

6. Main Program
	•	Add a comment block clearly labeled # Main Program.
	•	Function-level docstring for main(): explain that it provides the user with a menu and calls other functions based on user choice.
	•	Inline comments:
	•	Explain that the loop keeps the program running until the user chooses Exit.
	•	Describe each menu option’s link to its function.
	•	Note that input is checked for validity (user must enter 1–5).
