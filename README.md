# Floating_Point_ALU in MIPS

The purpose of this program is to create an ALU for floating-point numbers, in MIPS. It contains five methods, 
described below.

1) Float_Print, prints out the given float
Prints the sign, exponent, and mantissa in the argument $a0
Returns nothing, but syscalls to print out info about float
Side effects: The float's relevant information is printed out

2) Float_Compare, compares two given floats passed in $a0 and $a1
Returns: 1 if 1st float > 2nd float, -1 if 2nd float > 1st float, 0 iff 1st = 2nd 

3) Float_Addition, adds the two floats passed in in $a0 and $a1
returns: $v0, containing the normalized sum of the two floats added

4) Float_Multiply, multiplies the two floats passed in $a0 and $a1
returns: $v0, containing the normalized product of the two floats multiplied 

5) Float_Normalize, normalizes the inputted float in $a0, $a1, $a2, $a3
returns: $v0, containing the normalized float

Each function is detailed more specifically in the FloatingPointALU.asm file, as well as pseudocode explaining the 
process, comments, and the registers each function uses. A tester file, FloatingPointTester.asm, has been 
included as well to verify that the program works.
