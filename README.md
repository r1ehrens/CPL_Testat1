# CPL_Testat1

## Simple calculator
`*` implement a function for performing different operations on function parameters and return the result.
read formatted input from an std::istream

`*` split a project containing an implementation and tests into tree projects: library (with implementation), tests and executable. This is a repetition of the modularization you have already performed on the SayHello project last week.

###Implement a calc function
Create a function with the signature int calc(int, int, char) that takes two numbers an a character denoting an operator symbol ('+', '-', '*', '/' and '%'). The function calc should interpret the operator character and compute its result by combining the two integers accordingly. To give you a headstart you can use the code below in a CUTE Project as Test.cpp. Add additional test cases for the corner cases of the function. Consider and test valid and invalid input, e.g. unknown operators and division by zero. What options for error handling are feasible? Discuss them with your supervisor and your peers.

Use the functions implemented in the previous weeks to create a simple pocket calculator simulation. Allow the user to enter a calculation using two integers and an infix operator symbol. This input should stand on a single line and the result of the calculation should be displayed in a large way using your seven segment display simulation from last week. In this exercise the display width should be limited to a maximum number of eight digits (<=8) including a large minus sign for negative numbers. This limitation should be implemented in the pocket calculator, not the seven segment functionality itself. For the underlying calculation use your function calc(). Read the input line by line (std::getline()) and interpret each line as a calculation (operand operator operand). Expected signature: void pocketcalculator(std::istream &, std::ostream&)
