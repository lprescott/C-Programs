# I CSI 333 (= I CEN 333) Programming at the Hardware Software Interface (4)
Instruction set architecture of contemporary computers; Boolean logic, memory, registers, instructions and interrupts. Assembly language programming; assembler passes, symbols, macros, function linkage and separate compilations. C language programming; syntax, control, types, abstractions, pointers and strings. Dynamic memory, standard and user written libraries. ANSI and C++ standards. Instruction set simulation. 

## p1:
This C program converts the decimal integer d into its equivalent number in radix r.  
The first decimal integer, d, is assumed to be nonnegative and the second integer, r, is assumed 
to be an integer such that: 2 <= r <= 16.  The decimal integer, d, is inputted by the user via 
the function scanf(), as is the integer r. The program outputs the equivalent number in base 
r via the function printf(). 

## p2:
This C program carries out a left-to-right evaluation of an arithmetic expression. 
The arithmetic expression consists of non-negative integer constants and the operators: +, -, *,
and /. The operator / denotes integer division. There is no notion of precedence; the expression 
is evaluated strictly from left to right. The inputted expression is assumed to be valid (ie): It 
satisfies all of the previous conditions; It wont contain parentheses; Each integer constant in 
the expression consists of only one decimal digit; The expression begins with an integer constant 
without any preceding sign and in the expression: integer constants and operators alternate. The 
function evaluateExpression() inputs from stdin via fgets() and outputs to stdout via printf().

## p3:
This C program prompts the user for commands, accepts commands from the keyboard (stdin) 
and executes those commands. When a command requires output, it is written to stdout. The program continues 
to accept and process commands until the user types the end command. 

The program deals with linked lists. Each node of such a list contains a string of length at most 10, a 
positive integer (i.e., an integer value ≥ 1) and a pointer to the next node of the list. For any node, the 
string and the integer stored in that node will be referred to as the symbol and count for that node 
respectively. At all times, the list must satisfy the following two important properties:
	
1.	The symbols appearing in the list are all distinct; that is, no two nodes have the same symbol.
2.	When the list is scanned from left to right, the counts must be in non-increasing order. An example of such a linked list is shown below.

## p4:
This C program inputs a MIPS Assembly Language program and outputs a listing of the MAL program with line numbers
and/or a cross-reference table. The program will be executed via the command line by passing arguments to main method in the form
?.out flag inputfile outputfile. The arguments inputfile and outputfile specify the names of the input file and the output file respectively. The flag argument is one of the following: -l, -c or -b. If the flag is -l, the program only produces a program listing of the MAL source programin the specified output file. If the flag is -c, the program produces only the cross-reference table for the MAL source program in the specified output fule. If the flag is -b, the program produces both listing and table in the specified output file.

Assumptions: 

1. Every line of a MAL program is terminated by the newline ('\n') character and has at most 80 characters (including the newline character). 
2. The maximum number of labels that can appear in any MAL program is 100.
3. The identifiers are case sensitive and the maximum length of an identifier is 10. 
4. All input files  satisfy the following conditions:
    1. The MAL program in the input file won't contain any errors. 
    2. Every identifier will be defined somewhere in the MAL program. 
    3. There will be no multiply defined identifiers. 

# p5:
p5a.mal prompts the user for a positive decimal integer, reads a positive decimal integer typed by the user and outputs the following: 
	
1. The total number of 1's in the right half of the binary representation of the integer.
2. The total number of 0's in the left half of the binary representation of the integer.
3. The highest power of 2 that evenly divides the integer.
4. The value of the largest digit in the decimal representation of the integer.

p5b.mal prompts the user for a line of text and reads the line inputted by the user. If the line contains just white space characters the program outputs the message "Line contains only white space characters."

If the input is not empty, the program computes and outputs the following:

1. The number of non-whitespace characters in the line. 
2. The number of words in the line.
3. The maximum length of a word in the line.
4. The minimum length of a word in the line.
5. The word of maximum length in the line. If there are two or more words of maximum length in the line, then the program prints the word of maximum length that appears first in the line.
6. The word of minimum length in the line. If there are two or more words of minimum length in the line, then the program prints the word of minimum length that appears first in the line.