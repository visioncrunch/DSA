How does computer stores any information -: name, address, pass/fail, 01010010 in form of bytes
01010110 01011101 01011101 01011010

bit /transistor/ switch  / wire
0 1  on off     on off    connected disconnected
smallest unit of information that computers can understand: byte - set of 8 bits
how does computer stores anything: bytes




1. # how to approach a problem

 problem statement ->
 solution in head -> 
 rough solution(flowchart) ->
 high level language(C++) -> 
 machine language 0101010101110101

2. # return minimum/maximum of three numbers

 - set ans = INT_MAX
 - iterate on all numbers and update ans as min(ans, number)
 - return ans

 - using ternary operators
    return a < b ? (a < c ? a : c) : (b < c ? b : c)  

 - sort array and report the smallest element as answer

 - use min function min(a,(min(b,c)))

3. # check prime or not

 - if any number from 2 to n-1 factors n then its not prime. else it is

 - if any number from 2 to sqrt(n) factors n then its not prime. else it is

 - sieve of eratosthenes

 - fermat's little theorem

 - miller rabin's primality test

 - AKS primality test

 - lucas-lehmer primality test

 - baillie-psw primality test

4. # statements a loop contains

 - initialization
 - condition
 - logic
 - updation

5. # loops

 - for
 - while
 - do-while
 - for-each

6. # check odd or even

 - if n%2==0 even
 - if n&1 odd
 - 1 and 2 can be written as:
    return n%2==0 ? even : odd
    return n&1==1 ? odd : even

7. # print counting from 1 to n / n to 1

 - for i in 1 to n print i

 - i = 1
 - while i<=n
        print i
        i++

 - use recursive fn 
    printnum(m, n)
        if m<=n
        print i
        printnum(m+1,n)

 - i = 1
 - do 
      print i
      i++ 
   while i<=n

8. # if else piecewise defined for each range

 - read n
 - if n in 91 to 100 print a 
 - else if n in 81 to 90 print b
 - else if n in 71 to 80 print c
 - else if n in 61 to 70 print d
 - else print e

9. # check +ve/-ve/0

 - if n<0 -ve
   else if n>0 +ve
   else 0

 - switch(n) (increases readability)(n must be int char long or any integer datatype)
        case(n<0): 
            -ve
            break; //break is important for termination of further execution
        case(n>0): 
            +ve
            break;
        default:
            0
            break;

 - return n>0 ? +ve : n<0 ? -ve : 0

10. # CheckTriangle(a, b, c) (output 1 or 0)

 - return (a + b > c) && (a + c > b) && (b + c > a);

11. # factorial of a number

 - fact = 1
 - for i in 2 to n 
        fact*=i
 - return fact

 - fact(n)
    if n ==1 or n==0
        return 0
    else
        return n*fact(n-1)

12. # print 1 to n odd numbers

 - change the updation from i++ to i = i + 2 and print the index

 - function print_odd_numbers(start, n):
 -   if start > n  : return   
 -  if start&1    : print start
 -   print_odd_numbers(start + 1, n)

13. # reverse a number

 -  while(n>0)
 -  rev = rev * 10 + num%10;
 - num/=10;

14. # same after double reversal

 - return reverse(reverse(num))==num;

15. # movies for programmers

 - terminator
 - the matrix
 - the wolf of wallstreet


16. # LLM MLL HLL

 - C++, assembly language 
 - binary 
 - python, no code platforms

17. # working of compiler

 - Preprocessing:
   Includes expanding macros (#define AUTHOR "abcd").
   Inclusion of header files.
   Conditional compilation (#ifdef, #ifndef, #endif).

 - Remove Comments: Comments in the code are removed.

 - Source Code to Tokenization:
   Lexical analysis involves tokenizing the preprocessed code. Tokens are the smallest units in a programming language, such as keywords, identifiers, operators, and literals.

 - Syntax Analysis (Parsing):
   The token stream is used to build a parse tree or syntax tree, which represents the grammatical structure of the program.
   Handles the language syntax and verifies that the code adheres to the language grammar rules.

 - Semantic Analysis:
   This step involves analyzing the meaning of the code beyond its syntax.
   Checks for type compatibility (e.g., int a = "ABD";) and verifies that variables are declared before use.
   Resolves variable references and enforces scoping rules.

 - Intermediate Code Generation:
   Translates the syntax tree or the high-level representation of the code into an intermediate language (e.g., three-address code or an intermediate representation specific to the compiler).

 - Code Optimization:
   Performs various optimizations to improve the efficiency of the code, such as constant folding, common subexpression elimination, and dead code elimination.

 - Code Generation:
   Translates the optimized intermediate code into the target machine code (assembly code) for the specific processor architecture.

 - Linking:
   Combines multiple object files (resulting from compiling different source files) and resolves references between them.
   It resolves symbols (functions, variables) used across different files and libraries.

 - Object File Creation:
   The linked code is assembled into relocatable object files.

 - Executable Creation:
   The linker combines object files, libraries, and other necessary components to create the final executable file.

 - preprocessing -> compiling -> assembling -> linking 
 - #include<stdio.h> gets converted to prototype of printf scanf etc. and the functions are written at the end below the main function
 - compiling converts the source code to assembly code
 - assembler converts the assembly code to binary code. 
 - linking combines stdio.c cs5 -c main.c into one large c file
./a.out - assembly output



18. # why need a programming language

Programming languages are essential tools that enable humans to communicate instructions to computers in a structured and understandable way. Here are several reasons why we need programming languages:

 - Communication with Computers:

Computers only understand machine language (binary code), which consists of 0s and 1s. Programming languages act as intermediaries, allowing humans to write code using a more intuitive and human-readable syntax.

 - Abstraction and Simplification:

Programming languages abstract complex operations and tasks, allowing developers to work at a higher level of understanding. They provide simplified constructs and functions to perform intricate operations without dealing with low-level hardware details.

 - Efficiency and Productivity:

Programming languages enable efficient coding by providing pre-defined functions, libraries, and frameworks that can be reused. This boosts productivity, as developers don't have to reinvent the wheel for common tasks.

 - Flexibility and Adaptability:

Different programming languages are designed for specific purposes and domains, offering flexibility to choose the most suitable language for a particular project. Some languages are best for web development, while others excel in data analysis, AI, or system programming.

 - Problem Solving and Logic:

Programming languages encourage structured thinking and problem-solving skills. Writing code requires breaking down complex problems into smaller, manageable steps, and then implementing logical solutions.

 - Automation and Repetitive Tasks:

Programming allows automation of repetitive tasks, saving time and effort. By writing scripts or programs, we can instruct computers to perform routine actions consistently and accurately.

 - Scalability and Maintainability:

Well-structured programming languages promote scalable code, making it easier to handle larger projects. They also facilitate code maintenance and updates, ensuring that software remains functional and relevant over time.

 - Innovation and Development:

New programming languages often introduce innovative features and capabilities that drive technological advancements. They enable the development of new software, applications, and technologies, pushing the boundaries of what's possible in the digital world.

 - Cross-Platform Compatibility:

Many programming languages are designed to work on multiple platforms and devices. This cross-platform compatibility allows developers to create applications that can run on various operating systems, enhancing accessibility and reach.


19. # header files 

 - Files that contain declarations of functions, variables, and other constructs. 
 - They often also include function prototypes, macros, constants, and type definitions. 
 - These files typically have a `.h` extension (e.g., `example.h`) and are used to organize and manage code in a modular and reusable way.

 - Declaration: It contains declarations, which tell the compiler about the existence and type of functions, variables, and other constructs defined in other parts of the program.
 - Inclusion: The `#include` directive is used to include a header file's content in a C or C++ source file. This is usually done at the beginning of the source file.
 - Preprocessing: Before the actual compilation, a preprocessor processes the `#include` directives and replaces them with the content of the specified header files.
 - Compile: The compiler then compiles the resulting source code, which now includes the content of the header files.
 - header files are included in the memory of the process that is happening.

20. # from transistors to softwares


 - Transistors and Logic Gates:
   Transistors are the fundamental building blocks of digital circuits.
   Logic gates (AND, OR, NOT) are created using transistors to perform basic operations (Boolean logic).

 - Combinational Logic:
   Combinational circuits use logic gates to process inputs and produce outputs based on the current input only.
   Important for understanding algorithms involving bitwise operations.

 - Sequential Logic and Flip-Flops:
   Flip-flops store binary information and are the basis of sequential circuits.
   Understanding flip-flops is crucial for algorithms involving state and memory management.

 - Registers and Memory:
   Registers store data that the CPU needs to process quickly.
   Memory (RAM) is crucial for storing and accessing variables and data structures efficiently, which is vital in DSA.

 - Assembly Language and Machine Code:
   Assembly language is a low-level human-readable representation of machine code.
   Understanding assembly is essential for algorithm optimization, especially for time-critical operations.

 - Operating Systems:
   Operating systems provide an interface between hardware and software.
   Understanding OS concepts (processes, threads, scheduling) is important for designing efficient algorithms and data structures.

 - Programming Languages:
   High-level languages (e.g., C++, Java, Python) abstract hardware details, allowing developers to focus on algorithm design and data structures.
   Knowledge of programming languages is crucial for implementing and optimizing algorithms.

 - Data Structures:
   DSA involves understanding and implementing various data structures (arrays, linked lists, trees, graphs, etc.) and algorithms (sorting, searching, etc.).
   Efficiency in data structure choices impacts algorithm performance.

 - Compilers and Interpreters:
   Compilers translate high-level code to machine code, optimizing and improving efficiency.
   Interpreters execute code directly but often with a performance trade-off.
   Knowledge of how compilers work is essential for writing efficient code.

1 - Software Development Lifecycle:
    Understanding the software development process (requirements, design, implementation, testing, maintenance) is crucial for building robust and efficient software systems.

1 - Algorithms:
    DSA includes the study of various algorithms for solving specific problems efficiently.
    Analyzing algorithm complexity (time and space) is essential for optimizing and choosing appropriate algorithms.

1 - Optimization and Performance Tuning:
    Profiling and optimizing code for better performance are essential skills in DSA, especially for handling large datasets and complex operations.

Understanding the interplay between hardware and software at each level is vital for designing efficient algorithms and implementing them effectively, considering both time and space complexities.

21. # getch function()

 - #include <stdio.h>
 - #include <conio.h>  // for getch() function

 - int main() {
    printf("Press any key to exit...\n");
    getch();  // Wait for a keypress then exit from the program
    return 0; }

22. # how computer understands binary

Computers understand binary, which is a base-2 numerical system, because the fundamental building blocks of computers, such as transistors and electronic circuits, can easily represent and operate using two states: on and off, or 1 and  - These states align perfectly with the binary system, where 1 represents "on" or true, and 0 represents "off" or false.

Here's how computers interpret binary:

 - Bit (Binary Digit):
   The basic unit of information in a computer is a bit, which can be either 0 or  - It's the smallest piece of data in binary representation.

 - Bytes and Words:
   A group of 8 bits forms a byte. Bytes are commonly used as the basic unit for representing and manipulating data. Multiple bytes grouped together form words, which represent larger units of data.

 - Representation of Numbers:
   Binary is used to represent numbers, where each position in a binary number represents a power of  - Starting from the rightmost digit, each position corresponds to 2^n, where n is the position's index.

      For example:
      \(1011_2\) in binary is \(1 \times 2^3 + 0 \times 2^2 + 1 \times 2^1 + 1 \times 2^0\), which is equal to \(11_{10}\) in decimal.

 - Representation of Characters:
   In computing, characters (letters, numbers, symbols) are also represented using binary. Common encoding schemes like ASCII and Unicode assign unique binary patterns to each character.

 - Instruction Execution:
   Machine language instructions are encoded in binary. The CPU interprets these binary instructions and performs the corresponding operations, such as arithmetic, logic, or data manipulation.

 - Storage and Memory:
   Data stored in computer memory (RAM, hard drives, etc.) is represented in binary. Each byte of data is stored as a series of 8 bits, with each bit having a value of 0 or  -

 - Data Processing and Logic Operations:
   Logical operations (AND, OR, NOT) and arithmetic operations (addition, subtraction, etc.) are performed using binary arithmetic and logic gates, which are the basis of all computation in a computer.

Computers use electrical signals to represent these binary values (0 or 1), with voltages or states corresponding to these digits. Complex circuits and processors are designed to process and manipulate binary data efficiently, allowing computers to perform a wide array of tasks, from simple calculations to complex operations in software applications.


23. # optimization

 - a program can have multiple solutions but as a programmer our job is to find the most efficient one.

24. # fact about compiler

 - it was written by yet another compiler of previous version. hence automating the automation.

25. # where does a program starts

 - at the main function and it's the only function that is detected by compiler as the starting point

26. # function

 - a function takes input, applies the embedded logic in it, and then processes the output
 - return type name(argument type argname){return statement in line with return datatype at the end}

27. # working of cout

 - `cout << "Anubhav";`, is a C++ code snippet using the Standard Library for output.

 -  `cout`:
   `cout` is the standard output stream in C++. It is an object of the `iostream` class, which represents the standard output device, typically the console or terminal.

 -  `<<` (Insertion Operator):
   The `<<` operator in C++ is called the insertion operator. It is used to insert data into the output stream, in this case, the `cout` stream.

 -  `"Anubhav"`:
   `"Anubhav"` is a string literal, which is a sequence of characters enclosed within double quotes. In this case, it represents the text "Anubhav".

 - Output to the Console:
   The `cout` stream, combined with the `<<` operator, is used to send the string "Anubhav" to the standard output (usually the console). The `<<` operator inserts the string into the `cout` stream, and it gets displayed on the console.

 - Final Output:
   When this statement is executed, "Anubhav" is displayed on the console.

Putting it all together, `cout << "Anubhav";` instructs the program to output the string "Anubhav" to the standard output, typically the console, using the `cout` stream and the insertion operator (`<<`). This is a fundamental way to display information in C++ programs.

28. # why include iostream

 - because it has declaration of cout cin and other important functions

29. # identifiers--tokens-literals

 - Identifiers:
   Definition: An identifier is a name given to a program element, such as variables, functions, classes, etc., to uniquely identify them in a program.
   Rules for Naming Identifiers:
     Must start with a letter (a-z, A-Z) or an underscore (_).
     Can be followed by letters, digits (0-9), or underscores.
     Cannot be a keyword (reserved word).
     Cannot contain spaces or special characters (except underscores).
   Example Identifiers: `variableName`, `function_1`, `ClassA`.

 - Tokens:
   Definition: Tokens are the smallest units of a program that have meaning. In programming languages, tokens can be identifiers, literals, operators, keywords, and punctuation symbols.
   Example Tokens: `if` (a keyword), `123` (a numeric literal), `+` (an operator), `variableName` (an identifier).

 - Literals:
   Definition: Literals are constant values that are used in a program. They represent fixed values that do not change during the program's execution.
   Types of Literals:
     Numeric Literals: Represent numbers (e.g., integers, floating-point numbers).
       Example: `123`, ` -14`.
     String Literals: Represent sequences of characters enclosed in double or single quotes.
       Example: `"Hello, World!"`, `'A'`.
     Boolean Literals: Represent true or false values.
       Example: `true`, `false`.
     Null Literal: Represents a null or empty value.
       Example: `nullptr` (in C++).

 - Keywords:
   Definition: Keywords are reserved words in a programming language that have special meaning and cannot be used as identifiers or for any other purpose.
   Examples of C++ Keywords: `if`, `else`, `while`, `for`, `int`, `double`, `class`, `return`, `break`, `switch`, etc.
   Usage: Keywords are used to define the syntax and structure of a program. For example, `if` is used to start a conditional block, and `int` is used to declare an integer variable.

In summary, identifiers are names given to program elements, tokens are the smallest units with meaning, literals are constant values, and keywords are reserved words with specific meanings in a programming language. Understanding and using these concepts is fundamental in writing and comprehending code in any programming language.

30. # end of line or newline

 - Portability:
The "newline character" ("\n") is widely accepted and standardized across different programming languages, platforms, and operating systems. It ensures portability and consistency in representing the end of a line.

 - Consistency and Clarity:
Using "\n" as the newline character is a clear and consistent way to denote line endings in text. It's easily recognizable and understood by programmers, making code more readable and maintainable.

 - Compatibility:
Most programming languages and text processing tools interpret "\n" as the newline character. Using this convention ensures compatibility and interoperability with various tools and systems.

 - Efficiency:
The "newline character" ("\n") is efficient in terms of both memory usage and processing time. It requires just one character to represent the end of a line and is handled efficiently by modern programming environments and libraries.

3 - # vscode shortcuts 

 - ctrl + g   go to a specific line no
 - ctrl + f2  select all the occurences of a word
 - ctrl + p quick open files
 - ctrl + shift + f search across files in the project
 - ctrl + home - goes to starting of document
 - ctrl + end - goes to ending of document
 - ctrl + f to find some words press enter to replace, esc to exit
 - f5 to debug
 - shift ctrl f5 debug to restart debug
 - shift f5 to stop debug
 - step over f10 step into f11 continue f5

32. # why return statements at the end of functions

 - to indicate a successful termination of the function and perform its side effects

33. # graph of reality

 - starts from 100thousands
 - decreases exponetially
 - stops at around some hundreds

34. # flow of execution

The flow of execution of a program refers to the sequence in which the instructions and statements in a program are executed. This sequence follows a particular order, which can vary based on the programming language and the structure of the program. Here's a general overview of the typical flow of execution in a program:

 - Initialization:
   Variables and data structures are initialized with default values or values specified by the programmer.

 - Input:
   The program may prompt the user for input or read input from files or other sources.

 - Control Flow:
   Based on conditional statements (e.g., if, switch), the program determines which code block to execute next.

 - Loops:
   Iterative structures (e.g., for, while, do-while) execute a specific block of code repeatedly until a condition is met.

 - Function Calls:
   The program may call functions or methods to execute specific blocks of code, possibly passing arguments.

 - Execution of Statements:
   The program executes statements in a sequential manner unless controlled by loops, conditional statements, or function calls.

 - Modifying Data:
   Data may be modified or updated based on calculations, operations, or user input.

 - Error Handling:
   The program may check for errors or exceptions, and appropriate actions are taken to handle them.

 - Output:
   The program generates output, which can be displayed to the user, stored in files, or sent to other systems.

1 - Termination:
    The program reaches its end or encounters an exit condition, and the execution is completed.

Understanding this flow of execution is crucial for programmers to create efficient and functional programs. Proper control flow, efficient use of functions, appropriate error handling, and effective output generation are essential aspects of writing robust and maintainable code.

35. # gcd(greatest common divisor)

 - gcd(m,n) = gcd(m-n,n) if m>n use this minus program over modulo
 - gcd(m,n) = gcd(m%n,n) if m>n
 - if n is zero return m
 - else return gcd(n,m%n)

it doesn't matter whoever is greater than another they would be swapped of the divisor is greater, anyways

36. # lcm(lowest common multiple)

 -  gcd * lcm = a * b  (so if i know gcd lcm can be found out) 

37. # story of int a = 5

 - an integer of 4bytes of size named a that's equal to the literal value 5 stored at an address(say 104)
 - char has 1 byte of memory
 - bool has also 1byte of memory
 - long in 64 bit cpu is of 8bytes and in 32 its 4bytes
 - int num; cout<< num; prints garbage value
 - variable naming - telMeter, area_of_circle, flight1, greatestDivisor

38. # how data and address of a variable is stored

 - data is stored as binary digits
 - address is stored as a hexadecimal value
 - char a = '97' means the letter a 
 - char is an integer datatype
 - smallest unit of memory that can be represented is a byte

39. # number system conversion

40. # storage of -ve numbers

 - 1s complement - negate all the bits
 - 2s complement - 1s complement and then add 1 to result
 - so -5 = ~5 + 1
 - range of signed int is 2^31-1 to -2^31
 - range of unsigned int is 2^32-1 to 0

41. # char ch = 239094094 output?

 - garbage value

42. # logical operators

 - && || !

43. # boilerplate code

 -  #include<iostream>
   using namespace std;
   int main(){

   return 0;
   }

44. # namespaces

 - 

45. # preprocessor directives

 - 

46. # range of different datatypes

 - char  -128,127
 - short -32K, 32K
 - int -2 billion, 2 billion
 - long -9 billion, 9 billion
 - decalaration int a;
 - initialization int a = 5;

47. # how fractions, powers, exponentials are represented?

 - 

48. # smallest representable unit in computer

 - byte and that's why boolean uses 8 bits instead of 1 bit.

49. # why counting starts from 0?

 - 

50. # typecasting

 - implicit - compiler promotes one type to larger type float a = 3/ -0 =  -6
 - explicit - int a = (int)c where c is float
 - either one of them must be float in division for result to be float

51. # operators

 - 

52. # 32bit vs 64bit architecture

 - 32 bit CPU can process 32 bits of instructions per cycle
 - 64 bit CPU can process 64 bits of instructions per cycle
 - addressable memory 2^64-1 upperlimit as opposed to 2^32-1 in a 32 bit cpu
 - resource usage more rams can be installed as opposed to only 4gb ram in a 32bit cpu and a 4gb ram in 64 bit cpu will be used more efficiently than if it was in a 32bit processor
 - double work per cycle as compared to 32 bit cpu
 - compatibility with 32bit softwares as well
 - better graphics performance
 - more security and signed processors
 - stops kernel patching with software
 - data execution/deletion prevention
 - ram limitation is just a software not a physical limitation
 - program files has 64bit files
 - and program files(x86) have 32 bit files


53. # decimal to binary

 - division method

 - bitwise n&1 method

54. # last digit of a number

 - mod by 10

55. # number excluding the last digit

 - divide by 10

56. # binary to decimal conversion

 - multiply with place value method

57. # computer's dumb

 - can't understand things at high level

58. # what exactly header files do

 - taking input
 - displaying output
 - accessing keyboard's pressed keys,etc.

59. # compile code in terminal

 - 

60. # run object file in terminal

 - 

61. # how to run files in C++/JAVA/Python

 - 

62. # extensnion of executables in: 

 - windows  .exe
 - mac/unix  .out

63. # java's compiltation story

 - every os has its own JVM thaat can run the universal bytecode interpreted by javac

64. # principal of mathematical induction

 - 

65. # patterns learnt while drawing shapes

 - 

66. # printf vs cout

 - printf is backward compatible with cout

67. # what is terminal

 - it is a command line interface and a program of OS that gives computer the access to physical world

68. # which g++

 - a compiler program found in user/bin

69. # what is cin

 - character input

70. # does keyboard input goes directly to program?

 - terminal takes the keyboard input and passes it on to software

71. # does program output goes directly to screen?

 - terminal takes output from program and passes it on to screen

72. # when are blocks copulsory

 - when there are multiple statements involved

73. # infinite for loop

 - for(;;){}

74. # if (cin>>n) or if(cout<<n)

 - cin cout return true if they take or produce the output

75. # what does ./a.out does?

 - it takes the executable to ram from rom and os runs it if main is there

76. # P1 P2

 - P1 P2 if P2 returns 0 implies the function P2 runs perfectly, hence indicating perfect termination

77. # what g++ does?

 - g++ converts a text file to .exe program. g++ is defined uniquely for every os systems

78. # xor

 - same bits - zero; different bits - one

79. # << >>

 - "x >> n" this just divides number by 2^n
 - "x << n" this just mulitplies number by 2^n
 -  by default signed integer is formed and >> works fine in handling the sign (sign dhifting occurs here)
 - for unsigned, right shift can change the value to a drastically large value
 - n<<1 produces a garbage value and gives a warining not an error

80. #  i++ and ++i

 - i++ executes then increments
 - ++i increments then executes
 - cout << a++*++a can produce different outputs on different compilers

81. # -10 >> 1 = -5

 - 00001010 
 - apply 1s complement - 11110101
 - add 1 - 11110110
 - ">>" 11111011 (that should be the answer but)
 - apply 1s complement - 00000100
 - add 1 - 111110101  -5

82. # ~1 = -2

 - 00000001
 - 11111110
 - 10000001
 - 10000010

83. # for if continue;

 - skips to next iteration by not executing the current iteration's unexecuted code

84. # for if break;

 - breaks out of the whole loop it is nested in

85. # global variable - bad practice

 - because it can be modified during program execution

86. # goto

 - 

87. # operators precedence

 - use brackets always to avoid it

88. # call stack

 - 

89. # some pre-defined useful functions in c++ library

 - 

90. # 5^-5 = -2

 -   5 = 00000101
 -  -5 = 11111011
 - xor = 11111110 (not correctly stored)
 - ans = 00000010 (2s complement applied)

91. # fastest loop

 - all are of smae speed

92. # which one to use if elseif else or if if else

 - for possibility of multiple conditions to be correct use if if if else otherwise for one condition use if elseif else

93. # count no of digits in a number

 - while n>0
 - n/=10
 - count++

94. # for each loop

 - for(auto i:st){cout<<i}

95. # ASCII

 - 

96. # header files class example

 - 

97. # array

 - why? to make n variables efficiently without naming all of them
 - int br[10];
 - address of oth element in array (104) then increments by size of data for subsequent element (108,112,116 if it was an integer array) 
 - addressof(); returns first element address in array
 - sizeof(); returns size of array
 - &arr gives address of that array
 - a[0] is smae as 0[a]
 - int a[3]; all garbage values
 - int a[]={1,2,3};
 - int a[3] = {1,2,3};
 - int a[5] = {2,4} -> {2,4,0,0,0}
 - int b[2] = {1,2,3,4} -> error
 - int n; cin >> n; in arr[n];  bad practice - possible that memory demanded is unavailable (instead use dynamic arrays)
 if we want to still do that, use heap memory by int* arr = new int[5];
 - addressof(arr[i]) = base index address + i*data type size 
 - linear search if arr[i] == target -> cout<<"found" break;

98. # generics

 - 

99. # adding 2 hexadeicals

 - a1c + a2b = 1547

100. # time complexity (increasing order)

 - 1,log2n,rootn,n,nlogn,n2,n3,2^n,n!,n^n
 - m+n if seperated loops
 - m*n if nested loops

101. # symbol table

 - var   address
 -  a      104 (hexadecimal value)
 -  b      232

102. # array passed into function

 - solve(int arr[], int size){}   
 - solve(int arr[][]4, int row, int col){}
 - whether or not you are giving 1st dimension, the successive dimensions are needed to be given

103. # count 0s and 1s in an array, dnfp, sort 2,1,0 sorting, -ve +ve sorting



 - use sort function sor(arr,arr+n)

 - can count all the 0s and 1s linearly and print 0s and 1s their count times

104. # return more than one values

 - in form of list tuple dictionary vector array and access their elements

105. # reverse an array

 - swap[arr[left++],arr[right--]] for i <n/2 
 - reverse[arr,arr+n]
 - for i=n-1 i>=0 i-- print arr[i]

106. # extreme print an array

 - until left > right print arr[left++], arr[right--]

107. # swap function

 - arithmetic method (a,b)
 - a = a+b
 - b = a-b
 - a = a-b

 - xor
 - a = a xor b
 - b = a xor b
 - a = a xor a

 - temp variable
 - temp = a
 - a = b
 - b = temp

108. # pass by value vs pass by refernce

 - by value makes copy always, not alters the real data, is limited to its scope, has different address
 - by refernce is &a, it's like altering the real data

109. # int &b = a

 - same memory location two names(a and b)
 - so cout << a is same as cout << b 

110. # arrays always get passed by reference

 - int solve(arr[], int size) no need to write int&arr[]

111. # important subjects

 - LLD, HLD, DSA, Web Development, 2 tagde projects, OOPs concept, DBMS, OS

112. # find unique elements in an array

 - xor all of them

113. # 0 xor a

 - a 

114. # print all pairs of an array

 - for i < n for j=i j < n cout arr[i], arr[j]
 - for i < n for j=i j < n for k = j k < n cout arr[i], arr[j], arr[k]
 - why j = i k = j (to avoid duplicate element pairs)

115. # while(count--)

 - runs till count is not 0

116. # shift array by n

 - implement shift function(swap(arr[i], arr[0])) k times
 - implement circular  approach (i+k)%n is the new index where value at index i will go
   make a new array
   for i <n 
   newarr[(i+k)%n]=arr[i]
 - extraspace method reverse(0,n-1) -> reverse(0,k-1) -> rev(k,n-1)
   123456
   654321
   564321
   651234



117. # run .exe

 - cmd  main.exe
 - powershell  .\main.exe

118. # static memory allocation

 - 

119. # dynamic memory allocation

 - 
 
120. # count set bits

 - use n&1 in each iteration and count
 - while(n) {n = n& n-1 count ++} return count

121. # vector

 - #include <vector>
 - int arr[5] static array
 - int n;
 - cin>>n;
 - int arr[n] redundant and bad practice
 - int * arr = new int[n]; dunamic array(still can't push more elements, size is fixed)
 - vector<int>v; 0 size
 - vector< vector << int >> v;
 - {5,-1} of size 5 and all values -1
 - {5} of size 5 and all values 0
 - v.push_back(n)
 - v.clear() clears whole vector data
 - vector<int>crr{1,2,3,4,5}
 - vector<int>brr={1,2,3,4}
 - vector<int>x(v) to copy other vector's data
 - v[0] first element
 - v[v.size()-1] last element
 - v.front(); first element
 - v.end(); last element
 - print using  ector method for(auto it:v){cout<< it };
 - 2d vector row size - v.size(); col size - v[i].size()
 - vector<vector<int>>arr(5,vector<int>(10,-1));  2d vector of 5 rows of size 10 each with all values -1
 - 2d index in 1d form c*i + j
 - rowwise access i < row j < col print v[i][j]
 - colwise access i < col j < row print v[j][i]
 - diagonal sum for i < row cout arr[i][i] (first diagonal)
 - diagonal sum for i < row cout arr[i][row-i-1](second diagonal)
 - transpose of matrix for i < n for j = i j < n swaparr[i][j],arr[j][i] (analyze the index patterns for printing via other traiangles)
 - i = 2 j = 2,1,0
 - i = 1 j = 1,0
 - i = 0 j = 0
 - reverse vector reverse(v.begin(),v.end())
 - jagged array v.push_back(v1), v.push_back(v2) and so on

122. # missing element {1,2,3,4,5,6,7,8}

 - calculate sum and subtract it from wholesum to get missing element

 - xor with whole xor

 - initialize answer as 0
 - if arr[mid]-mid = 1 move right -> start = mid + 1 //coz pattern didn't break move on
 - else if arr[mid]-mid != 1 store mid as answer and end = mid - 1 //pattern broke answer could have been skipped so move left
 - update mid and repeat 1 and 2 until start > end 
 - if answer = 0 then return n + 1 //it means last element is missing
 - else return answer
 - midify this approach to include the corner case(not done till now)

123. # rearrange +ve -ve in consecutive order with preserved order +-+-

 - 

124. # return row with max 1s

 - count 1s in all rows and return row with maximum counts by storing the index of row which had the max 1s latestly

125. # rotate a matrix 90degree clockwise/anticlockwise

 - take transpose and reverse(matrix[i].begin(),matrix[i].end())

126. # binary search time complexity log2n

 - s=0 e=n-1 mid;
 - while s < e  // this depends on case whether to use <= or only <
 - mid = s+(e-s)/2
 - if arr[m]id==target return mid
 - else if arr[mid]>target e = mid -1 // this also depends on case could have been e = mid
 - else start = mid + 1 // this also could have been s = mid
 - why monotonic function: we are able to neglect half the problem hence reducing the size
 - why binary search time complexity is very less
 - why s + (e-s)/2 INT_MAX + INT_MAX > range of integer
 - when s = e what does it mean? it represents single array element of size 1

127. # find and element, first occurence, last occurence, total occurence

 - in all cases use binary search and total = last - first + 1 and keep storing possible answers
 - for first occurence if we find an answer store it and move left because we might have skipped the first occurence and treated further occurences as first
 - same for last occurence just move right in order to check possible last occurence if skipped
it's code
 - initialize answer as -1
 - give start and end index
 - calculate mid index as s + (e-s)/2
 - if middle == target: store that mid index as answer and end = mid - 1 (for first occurence) or start = mid + 1(for last occurence);
   else if middle > target ? end = mid -1 :: start = mid + 1
 - repeat 2 and 3 until start>end
 - return answer;

128. # key pair two sum

 - n =6 x = 16 arr{1,4,45,6,10,8} yes arr[3] + arr[4]
 - for i< n Y = X - arr[i] for j < n j!=i if arr[j] = Y return yes

129. # find pivot index before or after which sum is same

 - 

130. # peak element in a mountain array

 - declare those start end mid and ans = -1
 - if arr mid > arr mid + 1 : store mid in answer and move left - > end = mid //answer could have been skipped and end = mid so as to not skip peak
 - else start = mid + 1
 - update mid repeat 2 to 3 until start >=end 
 - return answer
 - why stop when start>=end
   if start equals end then at only one element currently we would be iterating infinitely
   suppose s = 5 e = 5 m = 5 then certainly we are in step 2 condition when it is true we are reupdating end = mid that is 5 so again s = e = m = 5 so infinite loop

131. # whixh swap is faster

 - xor is faster because it is more close to CPU

132. # custom comparator

 - bool mycomp(int&a,int&b){return a>b}
 - sort(v.begin(),v.end(), mycomp)
 - bool mycomp(vector<int>a,vector<int>b){return a[0]>b[0]; for 0based indexing return a[1]>b[1]; for 1based indexing}


 
To use a custom comparator in the C++ sort() function, you need to pass it as the third argument to the function. The comparator function should take two elements of the type you want to sort as arguments and return a boolean value indicating whether the first element is less than, equal to, or greater than the second element.

For example, the following code sorts a std::vector of std::string objects in alphabetical order, using a custom comparator:

C++
std::vector<std::string> strings = {"hello", "world", "!"};

bool compareStrings(const std::string& a, const std::string& b) {
  return a < b;
}

std::sort(strings.begin(), strings.end(), compareStrings);

for (const std::string& string : strings) {
  std::cout << string << " ";
}
Use code with caution. Learn more
Output:

! hello world
Custom comparators can also be used to sort more complex data types, such as objects with multiple attributes. For example, the following code sorts a std::vector of Person objects by age, using a custom comparator:

C++
struct Person {
  int age;
  std::string name;
};

bool comparePersons(const Person& a, const Person& b) {
  return a.age < b.age;
}

std::vector<Person> people = {{25, "Alice"}, {30, "Bob"}, {20, "Carol"}};

std::sort(people.begin(), people.end(), comparePersons);

for (const Person& person : people) {
  std::cout << person.name << ": " << person.age << std::endl;
}
Use code with caution. Learn more
Output:

Carol: 20
Alice: 25
Bob: 30
Custom comparators are a powerful tool for sorting and ordering data in C++. They can be used to sort data based on any criteria, regardless of the data type.

vector<int> numbers = {4, 2, 7, 1, 9};

// Sorting in descending order using lambda function
sort(numbers.begin(), numbers.end(), [](int a, int b) {return a > b;});


133. # advanced questions of binary are based on

 - if found target store answer and move to intended portion of array and proceed to find another possible better approximate solution


134. # general practice

 - make copy then make modifications on that copy. do not alter the original data.

135. # pivot in sorted rotated array

    4 5 6 7 1 2 3
 - declare those start end mid 
 - if s == e then return s
 - else if arr mid < arr mid - 1 and mid - 1 >= 0 return mid - 1; //this is the case when mid is at the lowest element  // range out of bound error can come in here
 - else if arr mid > arr mid + 1 and mid + 1 < n return mid; //this is the case when mid is at the highest index      // same range out of bound error can come here
 - else if arr start > arr mid end = mid - 1 //at the lower line of graph, move backward
 - else s = mid + 1 //at the upper line of graph, move forward
 - update mid repeat 2 to 6 until start > end;

136. # pseudocode of square root of a number correct to n decimal places

 - define search space(the changing dynamic reduced range of possible answers) from answer space(the range of numbers that can be possible answers)
 - define the predicate function which will be applied on mid
 - based on output of this function decide whether to go left or right (advanced concept of binary search)

for example if i have to find sqrt of 68
i know it must be in range [0,68) (my answer space)
and my predicate function is mid*mid < 68 it can either say true or false 
if it is equal then return mid
if greater then go left
else if mid*mid < 68 store the answer, go to right (predicate function is true here only)  
hence minimizing search space by halfing the range

wherever predicate function gives true then store those answers isntantly
for example mid*mid<68 is true for mid = 6,7,8, -1, -2,...

to configure it for giving sqrt upto n decimal precision
 - define a double precision variable that stores  -1 if precision is 1  -01 if precision is 2
 - now apply mid+= mid/10 if mid*mid < 68  (to be continued...)

137. # binary search on 2d array pseudocode

 - c*i + j = address of ith element of a 2d array in 1d format
 - declare start end mid as before
 - i = mid/c j = mid%c  are indices of a 1d array in 1d format
 - same binary search code of 1d array just replace arr[mid] with currindex=arr[i][j]

138. # divide 2 numbers using binary search

dividend = quotient * divisor + remainder

 - range 0 to dividend 
 - if arr[mid]*divisior == dividend -> return arr[mid]
 - else if arr[mid]*divisor > dividend -> end = mid - 1
 - else store answer and start = mid + 1
 - repeat 2 to 4 until start > end

139. # binary search in a nearly sorted array
in case of sorted array there is only one condition
in a nearly sorted array, arr at index can be at position mid-1 mid mid +1

 - if arr[mid]==target return mid; (in case of nearly sorted array ther are three cases)
 - if arr[mid]==target return mid;
 - if arr[mid-1]==target return mid -1;
 - if arr[mid+1]==target return mid+1;
 - if arr[mid]> target end = mid -2
 - if arr[mid]< target start = mid + 2 
 - why 4,5 steps (to be continued...)

140. # find odd occuring element via binary search
an array with all elements even no of times except one number that occurs odd times
all repeating numbers come in pairs
and all pairs do not repeat
one number can't come more that 2 times at a time

 - xor method
 - count method
 -binary search method

 - observation:
    a) starting element of pairs before odd element stand on even index
    b) starting element of pairs after odd element stand on odd index
    c) for single element cases, the single element is the only answer

 - if mid % 2 == 0 then //for even indices
      
      if arr mid == arr mid + 1 
          
          then standing at left -> to move right s = mid +2
          
      else right -> to move left e = mid coz it can also contain answer

 - if mid % 2 != 0 then //for odd indices
    
      if arr mid == arr mid - 1
        
         then standing at left -> to move right s = mid + 1 
        
      else right -> to move left e = mid -1 

141. # interview hack

 - don't show that you know everything, take moer time, do it so that he can see your curiosity
 - first tell all the approaches and then wait
 -if he asks to solve ONLY then solve otherwise DON'T

142. # why it is important to tell col size when using a 2d array in function

 - its column size coz c*i + j

143. # basic math for dsa

Prime Number
 - Naive Approach:
 In this naive approach, we start from 2 (the smallest prime number) and iterate up to n-1,
 checking if n is divisible by any number in this range. 
 If it is divisible by any number, it's not a prime number. Otherwise, it's a prime number.

 - Square Root Approach:
 In this square root approach, we only need to check divisors up to the square root of n
 because if n is not a prime number, it must have a divisor smaller than or equal to its square root.

 -Sieve of Eratosthenes count number of primes upto n
 Start with a list of numbers from 2 up to the desired limit.
 Start with the first number (2) and mark all of its multiples as non-prime.
 Move to the next unmarked number (3) and repeat the process.
 Continue this process until you reach the square root of the limit.
 If prime[i] is true, then i is a prime number.

 - make a bool vector (prime) of all numbers from 0 to n with all elements marked as true
 - mark 0th 1st element as false and make an ans variable for recording count of primes
 -for i = 2 i < sqrt(n) 
        if(prime[i])
            ans++ //ans is count of primes upto n
            j=i*i //becoz all multiples smaller than this number will be marked in previous iterations
            All multiples of primes smaller than p have been marked in previous iterations, not their squares (which is why we start marking from p×p).
            
            for j < n
                prime[j]=false  //marking all of the multiples of prime numbers as false
                j+=i
    return ans

    Time complexity = O(n*log(log(n)))

 - Segmented Sieve
given L and R limit in which we have to find primes 
apply simple sieve till the upperlimit root R and retrieve the marked array
filter in primes from it in an array baseprimes 
find first multiple of basePrimes in LR array to start marking by L/baseprime *baseprime

if firstmultiple < L
int j = max of firstMultiple or baseprime*baseprime
    then add basePrime to it for retrieving multiple in range
make segmentedsieve vector of size R-L+1,true
mark v[0] and v[1] as false
for prime in baseprime
    int firstmultiple = L/prime *prime
    if firstmultiple < L add prime to it
    for j = max(firstmultiple, prime*prime) j<R
        sieve[j-L] = false
        j+=prime
return segmentedsieve
cout<< i+L


144. # modulo arithmetic

a+b % m = a%m + b%m
a%m - b%m = a-b % m
a % m % m % m = a % m
a % m * b % m = a*b % m

145. # fast exponentiation a^n
 normal O(n) 
 keep multiplying n times

 fast o(log n)
 fastexponentiation a,b
 int ans=1
 while b> 0
    if b&1  //if b is odd
        ans = a*ans //multiply a once more for inclusion of odd occurence
    a *= a
    b>>1
 return ans

146. # bubble sort - bubble up  the largest element by swapping
swap the adjacents if needed, till we get the largest element to the right in every iteration

for i = 0 i < n-1
for j = 0 j < n - i - 1  // shrinking the swapping space from both side as large and small elements are equally being sorted 
if arr j > arr j+1 then swap both (for ascending sort)
if arr j < arr j+1 then swap both (for descending sort)

O(n^2)
omega(N)

147. # insertion sort

void insertionsort(int arr[], int size)
{
   for (int i = 1; i < size; i++)
    {   int j = i - 1;
        int key = arr[i];
        while (arr[j] > arr[j+1] && j >=0)
        {
            swap(arr[j],arr[j+1]);
            j--;
        }
        arr[j+1]=key;
    }
}
148. # selection sort - select the smallest element in unsorted array and swap it with ending element of sorted array

from i 0 to n-1
find smallest number bw number[i+1] and numbers[n-1]
swap smallest number with numbers[i]
theta of n^2


149. # char arrays strings class 1
char ch[5]; declares an array of name ch of 5 blocks each of size 1 which can store characters (any type of symbol)
cin >> ch; (no need to use for loop for input or output)
null character \0
d o g '\0' sybolizes termination of string 
ascii value of null character 0
all the elements after the string in a chracter array are filled with null charaters
if char ch = \0
ascii = (int)ch will be 0
delimiters(character that can terminate processing of chars after it) - space" " tab\t enter\n
anubhav \t gupta will only take anubhav as input
to take a whole line as input cin.getline(ch, 100);
where ch is the character and 100 is the maximum size of input 
delimiter of getline function is enter or newline character, tabs and spaces will work
length of string in a chracter array
initialize length as 0
same run a for loop
if ch[i]=='\0' break;
else increment length
when out side of loop return length
it will count spaces too
alternative 
include string.h
strlen(ch) does the same

reversing a string
using two pointer rev(ch, lengthofstring)
dont pass size of ch array as null character on swap will terminate the program
utility function to reverse a character array of strings - reverse(str, str+len) that same array function can be used here
character array are also passed by reference

convert lowercase to uppercase (toupper and tolower are STL functions)
My name is Love Babbar
MY NAME IS LOVE BABBAR
97-97+65
low-low+up
lc - 'a' + 'A'
or
lc + char(32)
and for uppercase to lowercase
up - A + a
up - char(32)

code of lower to UPPER: 

void convertToUpperCase(char ch[], int n) {

  int index = 0;

  while(ch[index] != '\0') {
    
    //check if lowercase, then convert to upper case
    if(ch[index] >= 'a' && ch[index] <='z') {
      ch[index] = ch[index] - 'a' + 'A';
    }
    index++;
  }
}

code of UPPER to lower: 

void convertToUpperCase(char ch[], int n) {

  int index = 0;

  while(ch[index] != '\0') {
    
    //check if uppercase, then convert to lower case
    if(ch[index] >= 'A' && ch[index] <='Z') {
      ch[index] = ch[index] - 'A' + 'a';
    }
    index++;
  }
}


replace @ with space

My@name@is@Babbar
My name is Babbar

while ch[i] != '\0'
    if ch[i] == @
        ch[i]== ' ';
    index++

check palindrome

noon
babbab
racecar
tabat

2 pointer approach
bool checkPalindrome(char ch[], int n) {
  //n -> length of string
  int i=0; 
  int j = n-1;

  while( i<= j) { //we need to only traverse till half array
    if(ch[i] == ch[j]) {
      i++;
      j--;
    }
    else {
      //characters are not matching
      return false;
    }
  }
  //agar yaha pohjoch gye ho
  //iska matlab saare characters match kr gye h 
  ///iska matlab palindrome hai 
  //iska matlab return true krdo
  return true;
  
}

some stl function for character array

* `begin()` and `end()` - Return iterators to the beginning and end of the character array, respectively.
* `find()` and `find_if()` - Search for an element in the character array.
* `count()` - Count the number of occurrences of an element in the character array.
* `copy()` - Copies the contents of one character array to another.
* `fill()` - Fills the character array with a specific value.
* `reverse()` - Reverses the order of the elements in the character array.
* `sort()` - Sorts the elements in the character array in ascending order.
* `unique()` - Removes duplicate elements from the character array.
* `equal()` - Compares two character arrays to see if they are equal.
* `lexicographical_compare()` - Compares two character arrays to see which one is lexicographically greater.

These functions are all defined in the `<algorithm>` header file.


strings

string name;  string data type ka ek variable (string class ka ek object)
dynamic range
creation : string name;
input cin >> name;
output cout<< name;
access cout << name[2];
last element after string is also a \0 null character

i/p love babbar
stored love
same issue
solution
name = "love babbar";
getline(cin, name);

some utilities of strings
https://cplusplus.com/reference/string/string/


 string name;

  cin >> name;

  empty string
  string temp = "";

  cout << "Length of string: "  << name.length() << endl;     //gives length of a string

  cout << "String is empty or not: " << temp.empty() << endl; //checks if a string is empty or not

  cout <<"Character at position 0 is: " << name.at(n) << endl;  //gives the value at index n

  cout << "Front character of string is: "<< name.front() << endl; //gives the value at index front

  cout << "back character of string is: "<< name.back() << endl; //gives the value at index last

  string str1 = "Love"; 

  string str2 = "Babbar";

  cout << "before appending" << endl;

  cout << str1 << endl;   

  cout << str2 << endl;
  
  //append
  str -append(str2);

  cout << "After appending" << endl;
  cout << str1 << endl;        lovebabbar
  cout << str2 << endl;        babbar

  string desc = "This is a car";
  desc.erase(4, 3);  //4th index se 3 characters remove krdo
  desc.erase(desc.begin()+5,desc.end-9); remove characters in this range
  cout << desc << endl;  This a car 


  string name = "Love Babbar";
  string middle = "kumar ";

  name.insert(5, middle); //5th index pr middle waali string

  cout << "Printing name:  " << name << endl;


  string name = "love" ;

  cout << name << endl;

  name.push_back('R');   push R after the last string element
  cout << name << endl;

  name.pop_back();       removes the last element
  cout << name << endl;


  string str1 = "yaar tera super star desi kalakar";
  string str2  = "staryyyy";


  if(str -find(str2) == string::npos){
   //not found
   cout << "Not FOund" << endl;
  }
  else {
   cout << "Found" << endl;
  }

  string str1 = "babbar";
  string str2 = "Love";

  if(str -compare(str2) == 0) {     equals 0 when compared string is equal, >0 for longer and <0 for shorter
   cout << "Matching" << endl;
  }
  else {
   cout << "not matching " << endl;
  }


  string desc = "this is a car, big daddy of all suvs";

  cout << desc.substr(19, 5) << endl; //19th index se 5 lenght ki substring nikal lo


  hw check stl functions in string class and character array stl function

150. # char arrays strings class 2
  remove duplicates in a string

Input: s = "abbaca"
Output: "ca"
Explanation: 
For example, in "abbaca" we could remove "bb" since the letters are adjacent and equal, and this is the only possible move.  The result of this move is that the string is "aaca", of which only "aa" is possible, so the final string is "ca".
Example 2:

Input: s = "azxxzy"
Output: "ay"

    string removeDuplicates(string s) {
      string temp = "";

    for (char ch : s) {
        if (temp.empty() || ch != temp.back()) {
            temp.push_back(ch);
        } else {
            temp.pop_back();
        }
    }

    return temp;
    }


remove dulpicates part 2
Input: s = "deeedbbcccbdaa", k = 3
Output: "aa"
Explanation: 
First delete "eee" and "ccc", get "ddbbbdaa"
Then delete "bbb", get "dddaa"
Finally delete "ddd", get "aa"
Example 3:

Input: s = "pbbcggttciiippooaais", k = 2
Output: "ps"


remove all occurence of a substring
Input: s = "axxxxyyyyb", part = "xy"
Output: "ab"
Explanation: The following operations are done:
- s = "axxxxyyyyb", remove "xy" starting at index 4 so s = "axxxyyyb".
- s = "axxxyyyb", remove "xy" starting at index 3 so s = "axxyyb".
- s = "axxyyb", remove "xy" starting at index 2 so s = "axyb".
- s = "axyb", remove "xy" starting at index 1 so s = "ab".
Now s has no occurrences of "xy".


while(substring exits in badi wali string){
    keep removing
}
string removeOccurrences(string s, string part) {
        while(s.find(part)!=string::npos){
            s.erase(s.find(part),part.length());
        }return s;
    }



hw find all the name algorithms that exist in string class for pattern finding and time complexity and space complextiy
write erase function by self


valid palindrome 2
Given a string s, return true if the s can be palindrome after deleting at most one character from it.
Example 2:

Input: s = "abca"
Output: true
Explanation: You could delete the character 'c'

two pointer 
left++ right -- if both are equal

if not equal then if i remove left then remaining strong palindrome? yes/no
if not equal then if i remove right then remaining strong palindrome? yes/no
if both of the answers are true then both with individually form palindrome on removal
if one forms plaindrome and other doesn't then remove the one that forms the palindrome
if neither of them forms a palindrome then return false

how to struncture this into pseudocode

making palindrome checker by making second array then return bool of a[i]=b[i] uptil half

define the palindrome checker(n) function
that checks whether the remaining string is plaindrome or not after removal of element at index n
iterate the string

if(arr[l]==arr[r])
    then l++ r--

else if
    return palindrome checker1 || palindrome checker2


class Solution {
public:
    bool checkPalindrome(string s, int i, int j) {
        while( i<= j) {
            if(s[i] != s[j] ) {
                return false;
            }
            else {
                i++;
                j--;
            }
        }
        return true;
    }

    bool validPalindrome(string s) {
        int i = 0;
        int j = s.length() - 1;

        while( i <= j) {
            if(s[i] == s[j]) {
                i++;
                j--;
            }
            else{
                //s[i]!=s[j]
                //1 removal allowed
                //check plaindrome for remaining string after removal

                //ith character -> remove
                bool ans1 = checkPalindrome(s, i+1, j);
                //jth character -> remove
                bool ans2 = checkPalindrome(s, i, j-1);

                return ans1 || ans2;
            }
        }
        //agar yha tk pohoche ho
        //iska matlab valid palindrome hai
        //iska matlab -> 0 removal
        return true;
    }
};

minimum time difference



palindrome substring
Given a string s, return the number of palindromic substrings in it.

A string is a palindrome when it reads the same backward as forward.

A substring is a contiguous sequence of characters within the string.

 

Example 1:

Input: s = "abc"
Output: 3
Explanation: Three palindromic strings: "a", "b", "c".
Example 2:

Input: s = "aaa"
Output: 6
Explanation: Six palindromic strings: "a", "a", "a", "aa", "aa", "aaa".
 

Constraints:

1 <= s.length <= 1000
s consists of lowercase English letters.

approach
run palindrome check for odd and even and increase the count outwards for both pointers if possible

if odd 
put i j in middle element 
go in outward direction
if match increase count
if not match no need to compare further

if even
put i j in middle element
go in outward direction
increase count if match
if not match no need to count further


class Solution {
public:
    int expand(string s,int i, int j) {
        int count = 0;

        while(i >= 0 && j < s.length() && s[i] == s[j] ) {
            count++;
            i--;
            j++;
        }
        return count;
    }
    int countSubstrings(string s) {
        int totalCount = 0;
        for(int i = 0; i < s.length(); i++ ) {
            //ODD
            int j = i;
            int oddKaAns = expand(s, i, j);  
            //EVEN
            j = i+1;
            int evenKaAns = expand(s, i, j);
            totalCount = totalCount + oddKaAns + evenKaAns;
        }
        return totalCount;
    }
};

//time space complextiy of this code

151. # char arrays string class 3

152. # doubt calss week5
char array have by defalut zero filled in elements
strlen(ch) for length of character array
char ch[] = {0}; //goof practice in general for all types of arrays
inshort make array of length+1 so it reserves the space for the null character
why cout<< ch gives the whole array without looping 
but for an integer array, we have to traverse it whole why? - > bcoz it is inbuilt and understood by developers

why was my double precision truncated always -> bcoz i used the cout command
instead use printf with this syntax
printf("% -10f",doubleValue);
%n.mf means use n width and m decimal place of precision  
printf statement utilites
Exactly, you've got it right!

In the `printf` statement `printf("%n.mf", aDoubleValue)`, if `n` is a specified minimum width and `m` is the specified precision for decimal places, here's what happens:

 - **Minimum Width (`n`)**: The `n` value ensures a minimum width for the output. If the actual output is less than `n` characters, it will be padded with spaces on the left to meet the minimum width requirement.

 - **Precision (`m`)**: The `m` value specifies the number of decimal places to display for the floating-point number. It controls how many digits will be displayed after the decimal point.

So, for example:
- `% -6f` will ensure a minimum width of 5 characters and display up to 6 decimal places of precision.
- `% -100f` will also ensure a minimum width of 5 characters but display up to 100 decimal places of precision.

The `printf` function uses these format specifiers to format and print the floating-point number (`aDoubleValue`) accordingly.

153. # pointers
pointerl1
 special variable that stores address of other variable
example -  an interger variable named num mapped with address 104 with value 5
by default - address is stored as hexadecimal value
assume it as a variable with special datatype of address 
int* ptr = &a;
where int* is pointer to integer data ptr is pointer name
bool* = pointer to boolean data
short* pointer to short data
overall ptr is a pointe to integer data that contains some address

creation int*p;
access the value at address in ptr with derefernce operator joined with pointer cout<< *ptr 
why pointer?


int a = 5;
int*ptr = &a;
cout<< &a gives address of a
cout<< ptr gives address of a
cout<< &ptr gives address of pointer ptr
cout<< *ptr gives 5
cout<< a also gives 5
so a = *ptr
int &pr is only refernce name for the same memory location

int*ptr; will be illegal access of memory and runtime error will be thrown
to avoid this create a null pointer by int* ptr = 0; int*ptr =nullptr;

why arr = arr+ 1 not possbile bcoz arr is const pointer 
instead make a pointer variable pointing to arr and then modify that pointer bcoz its variable

why pointer size is 8?
most common in modern platforms
64 bit memory address are used hence 8 byte sized pointer
this size is determined by size of memory address in architecture
if memory address size is 8bytes then to store a value this large pointers should also be the same size of memory address




a = a + 1 (5 to 6)
ptr = ptr +1  (104 to 108 next memory location)
*ptr = *ptr + 1 (5 to 6)

a can be called *ptr also

int a = 100;  location 104
int*ptr = &a;
a - 100
&a - 104
*a - error
ptr - 104
*ptr - 100
&ptr - 208
(*ptr)++ - 101
++(*ptr) - 102
*ptr = *ptr/2 - half the value of a - 51
*ptr = *ptr -2 decrement in value of a by 2 - 49


int a = 5  1008
int *p = &a  216
int *q = p 318
a - 5
&a - 1008
*a - error
p - 1008
&p - 216
*p - 5
q - 1008
&q - 318
*q - 5


int*q = *p - error


int a = 50 104
int*p = &a 420
int*q = p 516
int*r = q 712
p q r are refernce pointers to the same variable

50 - a
104 - &a
error - *a
104 - p
420 - &p
50 - *p
104 - q
516 - &q
50 - *q
104 - r
712 - &r
50 - *r

pointer with arrays

arr, &arr, &arr[0] is base address 


int arr[5] = {10,20,30,40,50}; 104

arr 104
&arr 104
arr[0] 10
&arr[0] 104
*arr 10
*arr+1 11
*(arr)+1 11
*(arr+1) 20
*(arr+2) 30
*(arr+3) 40

*(arr+i) is same as arr[i] and i[arr]

int arr[5] = {1,2,3,4,5}
arr = arr+1 why not possible in this case
int p =5
p = p+1 possible and *p now stores some garbage values points at one address greater than original

arr - 104
&arr - 104
arr[0] - 10
&arr[0] - 104
p - 104
&p - 512
*p - 10
q - 108
&q - 420
*q - 20
*p+1 - 11
*(p)+2 13
*(q)+2 22
*(q+4) error

int arr[4] = {10,20,30,40}
sizeof(arr) = 16
int *p = arr
sizeof(p) = 8

char ch[50]= "love"
char* cptr = ch
cout<<cptr - love
cout<<ptr in case of integer array it will print the base address
cout<< *cptr ch[0]

char ch[50]="love" 104 cptr 208
char * cptr = ch;  char*cptr = &ch doesn't work but &ch[0] will work. Why? because &ch represents address of 10 characters (type-mismatch)
ch = love
&ch = 104
ch[0] l
&cptr 208
*cptr ch[0]
cptr love


char ch[50] = "Statement"
char*cptr= &ch[0]


ch = Statement
&ch = 104
*(ch+3) = t
cptr Statement
&cptr 216
*(cptr+3) t
cptr +2 atement
*cptr ch[0] S
cptr+8 t


char ch= 'a'
char*cptr = &ch

cptr - pointer to a character data
&ch gives address of a whole string that' why they both conflict



char*cptr = "babbar" bad practice 
bcoz the text is stored in temporary location without being named

wild pointer ?
uninitialized or deleted pointer
it doesn't points to a valid memory location so dereferencing it can cause undefined behaviour
int*ptr;
cout<<*ptr; - undefined behaviour

int*ptr = new int;
delete ptr;
cout<< *ptr; - again undefined behaviour

int*ptr = &x;
x is not declared so it doesn't count as a valid pointer much like the previous two cases

always initialize pointers to null ptrs or a valid memory location


void pointers can point to any data type
also called generic pointers
void * ptr;
it can not be derefernced directly bcoz compiler doesn't know which datatype is it pointing at

void*ptr;
int x = 10;
ptr = &x;
int * ptrptr = static_cast<int*>(ptr);
cout<<*ptrptr; gives 10 (value of x)(value of *ptr)(value of *ptrptr)

dereferencing means to retrieve the value at the memory location that is contained in the pointer

these are used for dynamic memory allocation using new keyword to determine the type of pointer at runtime
int*ptr = new int;
void*voidptr = ptr;
int*intptr=static_cast<int*>(voidptr);
*intptr=10;
cout << *ptr; //prints 10

static_cast<int*>(ptr);
casting ptr to int* datatype

static_cast<a>(b);
casting datatype a to b



dangling pointer

int*p = new int;
*p = 42;
delete p;
cout<<*p;
dangling refernce to 42 (undefined behaviour)

these arise bcoz of not managing the memory for the lifetime of that memory. 
while freeing memory and pointer still points to it.
 
 how to avoid dangling pointers
 returning a pointer to a local variable which in future can go out of scope.
 using a deleted or free up pointer
 RAII Resource Acquisition Is Initialization smart pointers
 unique_ptr, shared_ptr, weak_ptr
 use refernces instead of pointers (in case if i don't need to update the value at that memory)
 avoid returning pointers to local variables
 nullify pointers after deleting or freeing memory
 
 array of pointers - all elements are pointers to some locations int *ptr[5]
 pointer of array - pointer to the first element of an array int (*ptr)[5] 

 int (*ptr)[10]= &nums; a pointer to first element of an array of size 10
cout<<(*ptr)[3];
*(ptr+1) = 2
this is how it goes
 (*ptr)[3]

pointerl2
these both give errors as we are trying to create a pointer that points to array which is not allowed
pointers are supposed to point at a single value of datatype
char * cptr = &ch
int * ptr = &arr 

whereas this will run
int *ptr = arr
int (*ptr)[5] = &arr;
cout<< *ptr[5];
pointer in function
int arr[] is same as int *arr in function arguments that is a pointer named arr that stores the adress 416 of that array

&arr in function will return the address of the pointer newly created 
&arr in main function will return the address of arr[0] basically

pointer to pointer
int a int * ptr1 int ** ptr2 int *** ptr3 int **** ptr4
 "* ptr1" ** ptr2 *** ptr3 can get me value of a 

int a =5 304
int*p = &a 204
int **q = &p 104
a = 5
&a = 304
p = 304
&p = 204
*p = 5
q = 204
&q = 104
*q = 304
**q = 5


int a = 10
int *p = &a
int **q = &a  error assinging integer address to a pointer to pointer


int a = 10
int*p = &a
int**q = &p
int**r=&p
int***s=&q

a is integer with 5 at which p points at which q and r point and at q s points

*s = adress of p
**r = 10
***s = 10
**q = 10
**s = address of a
*q = &a
*p = 10
p = address of a
&s = address of s
&r = address of r
&q = address of q 
**s+1 = address of a+1 unit

int a = 5
int*p = &a
solve(p) (*p = *p +5)
cout p &p *p in main = &a, &p, 5 in solve &a, &p(of the new p formed in solve), 10

pass by value int*p
pass by reference int*&p (same things for pointers, no discrimination)

154. # cs50
debug50 ./buggy
rubber duck debugging
write always magic numbers as const int N = 4; (capitalize it for visual context)
constants can be globally declared
every string ends with nul character \0 whose ascii is 0
int main(void){}
int main(int arc, string argv[])
argv[0] has the name of the program ./program
argv[1] has the value that we pass
./greet a b c d (null)
argv[0] 1 2 3 4
argc will be 2 if i types ./greet a
echo $? - shows what the recently executed program exited with
cryptography
plaintext cipher ciphertext


155. # recursion

when a function calls it directly or indirectly

when solution of a bigger problem depends on a small problem of same type

1 case tum solve karo, baaki recursion sambhaal lega

to understand recursion, you need to first understand recursion

step(n) = K processing + step(n-1)
step(1) = base condition processing K1

recursion has
 base case (mandatory)  for n=0 or 1 return 1
 recursive call (mandatory) recursionans = fact(n-1)
 processing (optional) a +=b

some programs of recursion

print from n to 1
if n =1 (base condition)
print 1 and return;
cout << n  (processing)
print(n-1)  (tail recursion) (recursive call)

print from 1 to n
if n =1 (base condition)
print 1 and return;
print(n-1) (head recursion) (recursive call)
cout << n  (processing)

recursive tree

first the stack of recursive calls forms then the stack unwinds as a result of each call returning a value to its preceding recursive call

all the recursive calls are differnt instances of same function

time complexity make the recursive tree and add the processing times at each level

space complexity analyze the stack depth via function calls

climbing stair problem
virahanka numbers problem
fibonacci series problem
if n ==1 or n==0 return 1;
else f(n) = f(n-1) + f(n-2);

recursion in arrays

print(arr,size ,index)
if i == size return (simply exit if all elements are printed)
processing cout<< arr[i]; //for printing elements of array
print(arr, 5, i++)

following four can come at processing part of recursion, it can be storing the element in another structure, modifying the array element, or modifying another element based on this array

if arr[i] == target  return true or return i or cout << i //for searching an element in an array 

if arr[i] < minAns minAns = arr[i] //for finding min element in array

if arr[i]%2==0 v.push_back(arr[i]); //for pushing vector in array

arr[i]*=2 //for modifying the index to its double

recursive call 
print(arr, 5, i++, target, int &minAns)

store digits of a number in a vector

fun(int number, vector<int> &v)
if n==0 return;
fun(number/10,v);
v.push_back(number%10);

return a number made by using digits provided in a vector
int num = 0;
fun(vector<int> &v, num)
if i == size return number;
number= number*10 + v[i];
fun(v, num);

if a[i] == target cout < i //processing code for printing index of occurences of target in the provided string a

why int &minAns bcoz it avoids pass by copy (FOR THESE TYPE OF VARIABLES THAT STORE ANSWER, ALWAYS PASS THEM BY REFERNCE)

store all indices where occurence of target exists in a vector and return this vector
vector<int> dusso(int arr[], int size, int index, int target)
{
    vector<int> v;
    // Base case
    if (index == size)
    {
        return v;
    }
    
    // Processing
    if (arr[index] == target)
    {
        v.push_back(index);
    }
    
    vector<int> vectorans = dusso(arr, size, index + 1, target);
    
    // Combine the vectors
    v.insert(v.end(), vectorans.begin(), vectorans.end());
    
    return v;
}

// for specifically this code we can pass the vector by refernce in a void recursive function instead
dry run of this on
arr = {2, 1, 5, 2, 3, 4, 2};
size = 7;
target = 2;

main gets called
  
  it then calls dusso0
    
    it makes its own vector v0
    it pushes the index at which the occurence of target occured(if any)
    it then calls dusso1
  
      it makes its own vector v1
      it pushes the index at which the occurence of target occured(if any)
      it then calls dusso2
      
        it makes its own vector v2
        it pushes the index at which the occurence of target occured(if any)
        it then calls dusso3
      
          it makes its own vector v3
          it pushes the index at which the occurence of target occured(if any)
          it then calls dusso4
      
            it makes its own vector v4
            it pushes the index at which the occurence of target occured(if any)
            it then calls dusso5

              it makes its own vector v5
              it pushes the index at which the occurence of target occured(if any)
              it then calls dusso6

                it makes its own vector v6
                it pushes the index at which the occurence of target occured(if any)
                it then calls dusso7

                  it makes its own vector v7
                  it returns its empty vector v7 to dusso6

                dusso6 stores this and returns v7+v6 to dusso5
              
              dusso5 stores this and returns v7+v6+v5 to dusso4

            dusso4 stores this and returns v7+v6+v5+v4 to dusso3 

          dusso3 stores this and returns v7+v6+v5+v4+v3 to dusso2 

        dusso2 stores this and returns v7+v6+v5+v4+v3+v2 to dusso1

      dusso1 stores this and returns v7+v6+v5+v4+v3+v2+v1 to dusso0
       
    dusso0 stores this and returns v7+v6+v5+v4+v3+v2+v1+v0 to main

binary search
include exclude substr question pattern abc 
this can also be done using bit masking for more efficient solution

house roober coin change maximize the cuts pattern
in recursion i++ doesn't work, ++i works

in base case it is mandatory to return whatever the case, whatever the problem


big O - worst case time complexity for example binary search has O(log2n)

omega - best case time complexity for example binary search has O(1)

theta - if best and worst case have same complexity

typedef struct{
   string name;
   string phone;

}person;

person people[3];

people[1].name="fadfsd"
people[1].phone="1231233";

156. # doubt class week 6

majority number problem - return a number that has occured more than n/2 times in an array

brute force approach
just search and count linearly O(n^2)
binary search approach


moore's voting algorithm approach

157. # Week 1 - Assignment
    
Flowcharts Q1

- multiply two numbers 
- read a and b
- return a*b

Flowcharts Q2

- perimeter of a triangle with sides a,b,c
- read a,b,c
- return a+b+c 

Flowcharts Q3

- find simple interest
- read p,r,t
- return (p*r*t)/100

Flowcharts Q4

- print counting from 1 to n
- read n
- for i = 0 i < n
- print i + 1

Flowcharts Q5

- find factorial of a number
- read n
- initialize fact = 1
- fact*=n and n-- until n!=0
- return fact

Flowcharts Q6

- check prime or not
- from i = 2 to n-1
-   if i%n == 0 return false
- return true    

Flowcharts Q7

- check given triangle is valid or not
- read a,b,c
- if a>b+c && b>c+a && c>a+b
-   return true;
- return false

Flowcharts Q8

- print only even number from 1 to n
- read n
- for i = 2 to n i+=2
-   print i

Flowcharts Q9

- print maximum of three numbers
- read a,b,c
- return max(a,(max(a,b)))

- print maximum of three numbers
- if a>b 
    if a>c
      return a
    else
      return c
  else
    if b>c
      return b
    else
      return c

Patterns Q1

- solid square pattern
- for i < n
    for j < n
        cout<<"*"
    cout<< endl

Patterns Q2

- hollow square pattern
- for i < n
    for j < n
      if i == 0 or n-1 or j == 0 or n-1
      cout<<"*"
    cout<< endl;  

Patterns Q3
- hollow inverted half pyramid 0-+

Patterns Q4
- hollow full pyramid 0-+

158. # Week 2 - Assignments
    
Numeric Hollow Half Pyramid 0-+
    
Numeric Hollow Inverted Half Pyramid 0-+
    
Numeric Palindrome Equilateral Pyramid 0-+
    
Solid Half Diamond 0-+
    
Fancy Pattern #1 0-+
    
Fancy Pattern #2 0-+
    
Fancy Pattern #3 0-+
    
Floyd's Triangle Pattern 0-+
    
Pascal's Triangle Pattern 0-+
    
Butterfly Pattern 0-+
    
Display Area Of Circle print 2 * PI * r
    
Given Number Is Even or Odd 
Normal Method %2 = 0 is even  
Bitwise Method n&1 is odd
    
Find The Factorial
read n
initialize fact = 1
fact*=n and n-- until n!=0
return fact
    
Check Given Number Prime or Not factor from 2 to n-1 if any confirms not primes

Print All Prime From 1 to N: for every number from 2 to n check prime and print
    
Reverse Integer rev = rev*10 + num%10 num/=10 stop when num==0
    
Set the Kth Bit (1 << k) OR n
    
Convert the Temperature f = 9/5c + 32 k = c + 273.15
    
Count All Set Bits 
increase count if n%2 == 1 count++ and n/=2 until n==0 then return count
OR
if n&1 == 1 count++ and n>>1

Create Number using Digits numer = number*10 + arr[i]
    
Print all Digits of an Integer reverse first then acess the reversed number by num%10 and num/=10 until num==0
    
KM to Miles 
1km = 0.621371
store in float the answer or the value mile*km

159. # Week 3 - Assignments
    
Key Pair / two sum
find all pairs and check if there sum = X for i = 0 to n for j = i+1 to n if arr[i]+arr[j] == X store the indices and return the array if not found return empyty array
sort the array then use two pointer approach if csum == X return the indices in form of array else if csum > X h-- else l++

#include <iostream>
using namespace std;
#include<algorithm>
void twoSumPointerApproach(int arr[], int n, int x) {
    sort(arr,arr+n);
	    int l = 0;
        int h = n - 1;
         while (l < h)
         {
             int csum = arr[l] + arr[h];
             if (x ==csum)
             {      cout<<arr[l]<<" "<<arr[h]<<" ";
                 return;
             }
             else if (x < csum) h--;
             else if (x > csum) l++;
         }
         cout<<"Combination not found";
         return;
	}

int main(){
    
    int arr[] = {1,2,3,4,45};
    int x = 49;
    int n = 5;
    twoSumPointerApproach(arr,n,x);
    return 0;
}

Find Pivot Index
index where sum of left side elements is equal to the sum of right side elements

- brute force: calculate lsum rsum for each array element and return the index for which lsum rsum are equal

    #include <iostream>
using namespace std;
#include<algorithm>
void twoSumPointerApproach(int arr[], int n, int x) {
    sort(arr,arr+n);
	    int l = 0;
        int h = n - 1;
         while (l < h)
         {
             int csum = arr[l] + arr[h];
             if (x ==csum)
             {      cout<<arr[l]<<" "<<arr[h]<<" ";
                 return;
             }
             else if (x < csum) h--;
             else if (x > csum) l++;
         }
         cout<<"Combination not found";
         return;
	}

int main(){
    
    int arr[] = {1,2,3,4,45};
    int x = 49;
    int n = 5;
    twoSumPointerApproach(arr,n,x);
    return 0;
}

- optimized solution by creating arrays lsum and rsum to reduce caluclations(virahanka)

int pivotIndex(vector<int> &nums)
{
    
    int lsum[nums.size()];
    lsum[0] = 0;
    int rsum[nums.size()];
    rsum[nums.size() - 1] = 0;
    for (int i = 1; i < nums.size(); i++)
    {
        lsum[i] = lsum[i - 1] + nums[i - 1]; // filling the lsum array
    }
    for (int i = nums.size() - 2; i >=0; i--)
    {
        rsum[i] = rsum[i + 1] + nums[i + 1]; // filling the rsum array
    }
    for (int i = 0; i < nums.size(); i++)
    {
        if (lsum[i] == rsum[i])
        {
            return i;
        }
    }

    return -1;
}
int main()
{
    vector<int> arr{2, -1, 1};
    cout << pivotIndex(arr);
    return 0;
}

Sort Colors, dnfp, sort 0s and 1s
- 3pointer approach
while m<=h
int l = m = 0 h = size - 1
if arr[m] ==0 swap arr[l],arr[m]
l++ m++
if arr[m]==1 m++
else swap arr[m],arr[h] h--
    
Missing Number in an array of whole numbers

- sort the array
then while traversing it if i is not equal to arr[i] return index else if the whole array is traversed then just return n
- return xor of all values possible in rangle with xor of all values in array

    
Move All Negative Number To The Left Side Of An Array order not important
- use sort function
- while l < h
  if l is -ve l++
  if h is +ve h--
  else swap a[l++],a[h--]


  
Find Duplicate Number in an array of size n+1 where all numbers upto n were possible but one of them is duplicating (leetcode 287)

- sort the array and for i = 0 i < n-1  if arr[i] l== arr[i+1] return the element
- mark arr[arr[i]] = -1 and return 
      int findDuplicate(vector<int>&nums) {
     while (nums[0] != nums[nums[0]])
    {
        swap(nums[0], nums[nums[0]]);
    }
    return nums[0]; //everytime 0th element will have the duplicate
- negatice marking approach
  if nums[abs(nums[i])] == -1 return num[i]
    else apply nums[nums[i]]==-1

// n = sizeof(a)/sizeof(int) to get size of an array

Missing Elements From An Array With Duplicates

- sort and report the index where the pattern between index and value at index breaks

- for i 0 to n num[abs(num[i])-1] = -ve (this will mark all the unique elements as negative) and then for i 0 to n whereever num[i] is positive return it as i+1
  why num[i]-1 bcoz index start at 0 so nums[num[0]] would mean 0 which is out of range {1,2,3,4,...,n} so we subtract 1 from range to make it zero to n-1

- if arr[arr[i]-1]!=arr[i] 
    swap(arr[i],arr[arr[i]]) 
  else
    i++ 
  until i< n
  then for i 0 to n
    if arr[i]!= i+1
     then return that element



Find First Repeating Element create hash

- for i 0 to n for j i+1 to n if a[i] == a[j] then return i+1 after all the iterations return -1
- 1 5 3 4 3 5 6     1->1   5->2   3->2   4->1   6->1 (hashing)
  hash[arr[i]]++ then for i 0 to n if hash[arr[i]] > 1 return i+1
  unordered_map<int,int>hash;
  create your own hash of length equal to maximum of array element int* hash[6];   

Common Elements In 3 Sorted Array
while i< len1 j< len2 k< len3
- if all three are equal then return that element to set and increment them
- else if arr[i] < arr[j] then i++
- else if arr[j] < arr[k] then j++
- else k++
now iterate the set and print its element
to access the sets
set<int>st
for auto x=1; x < n x++
for auto i:st
another way remove the duplicates from each sorted array then use this program wo set


Wave Print A Matrix

access each column
if column no is even go from indexing 0 to n-1 for row
if column no is odd go from indexing n-1 to 0 for row

same logic for row
    
Spiral Print A Matrix

print outer box
decrease size
print next small box
    
Factorial Of A Large Number gfg
add two numbers represented by two arrays gfg

Remove Duplicates From ascending Sorted Array

Maximum Average Subarray (Sliding Window Problem)

160. # Week 4 - Assignments
    
K-Diff Pairs In An Array
    
Find K-Closest Element
    
Exponential Search & Unbounded Binary Search
    
Book Allocation Problem
    
Painters Partition Problem
    
Aggresive Cows
    
EKO SPOJ
    
PRATA SPOJ
    
Find SQRT of Integer N using Binary Search with K point decimal precision.
    
Divide using Binary Search with K point decimal precision

161. # Week 5 - Assignments
    
Valid Anagram
    
Reverse Only Letters
    
Longest Common Prefix
    
Reverse Vowels Of A String
    
Isomorphic Strings
    
Group Anagrams
    
Longest Palindromic Substring
    
String To Integer (atoi)
    
String Compression
    
Integer To Romans
    
Zig-Zag Conversion
    
Largest Number
    
Reorganise String
    
Find The Index Of First Occurence in a String

162. # Week 6 - Assignments
    
Let's Practice Pointers

163. # Expert session 1

non-verbal: articulate thinking before speaking and writing

listening

friendliness and being empathetic with juniors , office staff co-workers

open mindedness

feedback

being confident and influential

keep good contact with even sweepers  wiht everyone 

Can i work with random People? I can only survive through communicating via them

cross culture - take help of team leads project manager to "understand their culture" eg what japanese people consider work as, or what europeans do at work,
first impression is last impression
example i would need to talk to:
security guard (how do i talk to this person)
IT assistant (this guy can help me how do i talk with this person)
manager 
Lab Head
prepare statements of expected questions
maintain honesty

simplicity

dealing with clients

being concise yet story telling

sell your skills

treat everyone with equal respect because everyone has a unique story to tell 

merge technical skills with project management
learn the propagation flow cycle just like software development cycle

never assume anything always double check who you are working with their background
know a person before knowing them if not be clear

dealing with project managers

over communicate vs under communicate

give updates regularly to maintain integrity and loyalty with your work clients managers
poeple who do the work they are given will be recognized by managers
never tell how much you are working
if you are working it will be told indirectly becoz they recognize your work

learn the ecosystem of company put your ego down

never put yourself down without manager
you need the work to be done regardless of circumstances

personal touch and character building

dealing with aggresive managers, managing tough conversations

personality: look in the eyes when talking look straight be confident, be a brand

tean collaboration

conflict management

how communication change the narratives
build you own brand - 
building trust
raising hand/speaking when necessary
non verbal communication
personality, posture and perception
learn to say no, give up often

if i am doing my work clearly, work on my brand clearly, i can convey my message and i am damn sure it will be resonated

always treat the swiggy delivery boy greatly
these small things are noticeable

work on finances family mental health physcial health 

when i think i need to raise my voice i must

be specific

think from the perspective of the other put myself in his shoes

learn to say no politely with justified reasons

maintain work/life or work/brand balance

nevery say yes to anything to not burnout

never say a aa aaa while speaking english

writing effectively

concept 1 - who what when how
concept 2 - crisp clear no jargons/shortforms/acronyms write u as you only 

when you are sure that you have done the thing, natural confidence will come by itself

managers can be respect greedy and when they get it they will support you

honestly tell your problems you have to work on and your interest to learn it



never speak too much, only say what's necessary
accept mistakes/ be honest

nevery say you are in problem everyone has problem it only tells that you don't have fighting spirit

if someone asks what's your hobby. Only tell hobby nothing else, it can be disrespectful

frame yourself as you don't know it still learning its a big field and you will try to, this will convey that you can learn and showcase that you have tried and did it ++


what are you currently doing?
what are you currently studying?
I mean prepare these answer, cram them to make life easier
if someone speaks in hindi speak in hindi same for english
how are you -> i am fine
aap kese ho -> mei theek hu
i am open to feedback

overcome my fear of speaking regardless of shame guilt or something else

keep my tone overall the same - eg -  I met this person, he is great, never repeats anything, always comes up with new things.(speak all of these in the same tone)

never do office politics/talk about personal stuff at workplace
dealing with tough times, being underappreciated
why being relaxed, having financial and mental well being makes you a winner and an effective communicator

keep in mind once a perception is formed it is formed, and if it was formed badly, cure it smoothly

first year tips - read books, watch movies hollywood, think, make structures of every communication statement, think in the language you want to learn ENGLISH, HINDI

learn to talk in different scenarios - small chat statement,

think of a problems' solution, pseudocode, implement practically via code

toxic culture - pov they want us to frustruate so don't be frustruated to coutner them

how to neogciate for salary - learn to say no, i will think through it, and i will come back to you, research actual benchmarks backed by trustable data

164. # Dnc

mergesort
    s   m     e   //break into left and right half
    2 1 9 7 4 6 

Left          Right
2 1 9         7 4 6   //sort the two split arrays using recursion
s   m         m+1 e

    1 2 4 6 7 9    //merge the two sorted arrays

questions that most engineers fail to answer?
quick sort  merge sort  heap sort

    apply two pointer sorting on these two arrays

    inversion count question
    
    inplace mergesort

    why a = log2n

    space compexity?
    

void merge(int arr[], int s, int e){
    // declaring and filling the two heap arrays

    int m = (s+e)/2;
    //initialize sizes l,r of the two heap arrays
    int l = m - s + 1;
    int r = e - m;
    //declare the two heap arrays left,right
    int* left = new int[l];
    int* right = new int[r];
    //fill the two heap arrays left,right // these are already sorted
    int k = s;
    for (int i = 0; i < l; i++)
    {
        left[i]=arr[k];
        k++;
    }
    k = m + 1;
    for (int i = 0; i < r; i++)
    {
        right[i]=arr[k];
        k++;
    }
    _________________________________________________________________________
    //now replace the original array with the two arrays comparision for sort
    int i = 0, j= 0;
    int n = s; //s is the zeroth index of a divided array, so it may not be 0 else it would always start at starting array that was passed in the merge sort 
    	while(i < l &&  j < r) {
		
		if(left[i] < right[j] ) {
			arr[n] =  left[i];
			n++;
			i++;
		}
		else {
			arr[n] =  right[j];
			n++;
			j++;
		}
	}
  _____________________________________________________________________________
    //handle the corner cases if one of the array gets exhausted
    while (j<r)
    {
        arr[n]=right[j];
        j++;
        n++;
    }
    while (i<l)
    {
        arr[n]=left[i];
        i++;
        n++;
    }
   ___________________________________________________________________________ 
    //deallocate the heap memory
    delete[] left;
    delete[] right;
    
    
    
    
}
void mergesort(int arr[], int s, int e){
    if (s>=e) return;
    int m = (s + e)/2;
    mergesort(arr,s,m);
    mergesort(arr,m+1,e);
    merge(arr,s,e);
}

stack memory is far less than heap memory

how to allocate heap memory to data structures use the "new" keyword

variable sized array made on heap memory is fine
int* arr = new int[5];
new int[5] returns a address 
arr would be in stack memory 
and the address of array would be of heap memory
dynamic memory allocation can be done with this concept
to not waste the memory 
delete[] arr; at the end to deallocate the memory


165. # doubt class week 7

text data heap(after text and data near bottom) stack(on top)

OS by default gives a memory to stack (8mb/8kb)

segmentation fault aka stack overflow

whenever all possiblities are asked recursion is used generally

bit manipluation / bit masking in substr finding 

make recursive trees for fear of recursion

make recursive trees of hw questions of recursion

number of subsequence another apporach

calcualte n as size of string
calculate 2^n 
for i 0 to 2^n
declarea string out
decalre num = i
int j = 0
while(num)
int b = num &1
if b out.pushback(s[i])
++i
num >> 1

pirnt out


166. # local vs global variables

global variable is written outside a function

local variable is written inside a function

most local variable gets priority

to access global variable ::num 

::x=4
int x =20
 cout << x 20 will be printed
 cout << ::x 4 will be printed



167. # Memory Layout of a Program

hello.cpp
compile
assembly code
executable(program)(a.out)
this program is loaded in RAM by exec kernel, a program of OS

heap memory is dynamic memory


168. # OOPs Concept

revise c++ syntax
memory allocation
functional programming f1 calls f2 f2 calls f3 f3 returns f2 returns f1 returns
not easy to implement, extend ,maintain

structure/class is bundle of properties and methods

class Student
{
  int id;
  int age;
  string name;
  float marks;
  void study()
  {

  }
  void sleeping()
  {

  }
  void bunking()
  {

  }
  
};

int main()
{
  Student s1;
  Student s1[];
  s1 is an object that is instance of a custom datatype Student


}

cpu has register of size 4byte if it is 32bit cpu that has a pipe called memory bus that connnects to memory and reads ONCE and carries data from memory to registers
the thing is reading once is faster than reading twice or thrice

if class is empty, what would be its size -> 1 (smallest addressable memory)
now if a class is not empty, then it will remove the 1 byte of the empty class and will have the size of 4 bytes if integer property is set
if a behaviour is set then its size wont be counted until used

and if a variable of a class has size smaller than register for example a bool variable, the nalso it will be counted as 4bytes for a 32 bit cpu with 4bytes in a register
the cpu does it to not do extra work of extraction by adding a padding of size 3 byte to make it 1+3=4 bytes

and actually its not about register its about the largest datatype
so int double double will give 4+4(padding)+ 8+8 = 24 as answer

but its about smallest multiple of largest datatype that can store all the data
so int double int will be returning 16 not 24 
so bool will return 1 size(mulitples of 1 are sufficient to store datatype of size 1)

- brahmgyan: sbse bade datatype ke nearest multiple pr chale jao
minimum weight picker machine that can carry the largest datatype that exist at the time of operation

string is a class that has 24 size for a string object

abstraction - operating a mouse without caring about its internal working, using things in abstract way

by default class is private - methods and properties written without access modifiers are private


public private protected information of a class

private information can only be accessed by private methods

or change its access modifier to public
private:
  int name;
public:
  void funny(){}

constructor has no return type ####

ctor is shorthand for constructor

default constructor
Student(){}

when Student s1; is created it calls the default constructor that will initialize garbage or null value to the objects properties

this default constructor is set to public
when we set it to private then it will not let us make a Student variable as the constructor that helps initializes it properties is made private

the default constructor vanishes when another constructor is declared so if we need a default constructor to work we have to declare it again


Student(int _ogarg, bool _ewofe2, char _o1, int _re3){
  ogarg = _ogarg
  ewofe2 = _ewofe2
  o1 = _o1
  re3 = _re3
}
Student s1(3,1,'r',22);

with constructors "student without id" or "student without age" can be created
it will depend on the number of arguments that are passed that will decide which constructor is called - polymorphism
how to identify a constructor - it has the name of class in prototype


this.name = name
is same as
student.name = name
this is a private pointer that points at current object added inbuilt by compiler
this->id = id

student will be allocated in stack

can we change this variable?? 

heap int*a = new int(5);
heap Student*s = new Student(werw,22r,wr2,3r,13r); it creates a pointer s that will point to an object in heap
cout s->name;
cout *s.name;

just make sure to deallcate the object

object in stack is accessed by .name
object in heap is accessed by ->name

getter setter

const
 - makes object/method immutable const int x = 10 / compiler stores it in ROM(an optimisation)
lvalue that has memory location int a = 5
rvalue that doesnt have memory location int&a = b a is alias to b (refernce variable)
const int *a = new int(2);
int const *a = new int(2); (both are same)
cout<< *a << endl;
*a = 10 wont work
int b = 10;
a = &b;
cout << *a;
now 2 will be printed 
we changed the pointer to the const value but we didn't changed the constant value so this will work, 2 is not changed

for constant pointer 
int *const a = pnew int(2);

for both constant
const int* const a = new int(2);

constant method of a class can't change a class member variable, its content will be constant

int getx() const{} cant' change other member variables - the x can't be modified inside the value

setters shouldn't be made constant

default argument

void printfd(const abc &a){}
a is a constant object of class abc that implies that it can only use constant methods 
so a method like a.getZ() will only work if getZ is constant otherwise the compiler will throw an error saying that
you have used a non-constant method with "a" so it might be possible to change the object properties from getZ coz it's not constant

if we still want to change a property using a const method we can declare that property as mutable
mutable int x; instead of int x; bypassing const keyword promise

abc(int x, int y, int z)
{
  this->x=x;
  this->y=y;
  this->z=z;
}

initialization list to write a constructor

abc(int _x, int _y, int _z):x(_x),y(_y),z(_z) {}

if there is a const property and we need to initialize it for the first time we can use initialization list and it wont give any error


macros 
#define PI 3.142857
#define MAXX(x,y) (x > y ? X ; y)
shorthands for constants and commonly used expressions

Copy constructor(by default added by compiler)(called when making a copy of object into another)(public by default)(no return type)

Student s1 = s2;
s2 is source and s1 is destination where we need to copy
Student(const Student&srcobj)
{
  this->name = srcobj.name;
  this->age = srcobj.age;
}

data members are only things that are copied methods are not
it only gets called in this statement, because it is initialized in this statement
Student s2 = s1 (good practice)
s2 = s1 (bad practice to copy)
why we need copy constructor - > for deep copying 

student s1;
s1 = s2; will not call copy constructor

Student(const Student &srcobj){} (good practice)(this removes the possibility of data change in the srcobj)
Student(Student &srcobj){} (bad practice- in this srcobj's data can be changed)
Student(student srcobj){} - illegal as rhis statement prompts computer to call the copy constructor which is not declared yet

why pass by reference? because copy constructors work is to copy and by writing Student srcobj we are demanding a copy even before actaully making a copy this is like say you are drinving a car but without having one

variable life cycle
init/copy then destroyed

life cycle of an object
init/copy then destroyed

for destruction destructor is used (by default, inbuilt by compiler, public, no return type)
constructor, destructor, copy constructor is not safe and takes whole arguments
if we don't write destructor then compiler will make it's default dumb destructor

~Student(){
  cout<<"dtor"<< endl;
  delete v; to avoid memory leak
}

getter setter method to access data without changning it explicitely

string getgfname(){
  return gf;
  return this->gf;(same)
}

void setGfName(string gf)
{
  this->gf = gf;
}

oops ka mtlb jeevan

getters setters are made to access private data in public method

1 pillar of oops - abstraction loosely coupled things

encapsulation bundling of data and methods (wrapping things)

car that has hidden engine, accessible gear changer, key holder is encapsulation as it is the way to do abstraction

how it implements abstraction - i only see what student details are not the functioning of how all the data of student is stored or decided

why encapsulation
easy to handle
protect integrity, reliable, secure, control of how class data is modified and who can modify it's properties 
maintainability
friend keyword? -> to share info of a hidden class
friend class B;
friend void print(const A &);





authentications steps can be added
like only allow gf name if its female
perfect encapsulation - if all data members are private
access is gvien thorugh getter setter

encapsualtion is often a mean to acheive abstraction by hiding internal details and only exposing what is necesssary

inheritance 
class dog extends animal
(sub class child class derived class) extends (super class parent class base class)

syntax
class childname: public/protected/private(mode of inheritance) parentclass{};
class Sparrow : public Bird
{

};
increases extensibility by code reusability

protected members are accessible within class itself and to derived classes

if we try to borrow protected things as public they will be borrowed as protected to ensure security

private is never accessible or derived or it can't be inherited

private > protected > public
experiment the table - make base class and sub class with all these public private protected access modifiers

types of inheritance
- single inheritance
    animal to dog
- multiple inheritance(not possible in java)
    derived class that inherits from more than one class
    techer to professor
    reseracher to professor
    father to professor
    employee to professor
    class professor : public teacher, public reasearcher{}; 
- multl-level inheritance
    animal to human to girl
- hierarchical 
    animal to dog
    dog to desi
    desi to owned
    owned to died

dimaond problem

      person
      /    \
     /      \
    /        \  
teacher   reseracher
    \        /
     \      /
      \    /
       \  /
    professor

nonstatic member 'walk' found in multiple base-class subobjects of type 'person' 

member found by ambiguos name lookup
professor is comfused whose walk() to choose teacher or reseracher

by principle of abstraction professor deosnt know person

solution:

scope resolution: clearify whose walk() to use
p.teacher::walk();
p.reaserarcher::walk();

virtual
class teacher : virtual public Person
by inheriting virtually is saying dont make copy of the methods. when someone uses the walk() function now the user would be able to use person.walk() at the runtime from both the classes

compile time pr chizein less logical hoti hain
runtime pr chizein more logical hoti hain
the base class must be inherited virtually if needed in the diamond

polymorphism is used
so by using virtual we are using the walk() function at runtime by ihneriting the functions implementaiton when it is used
with virtual i can bring same copy to the class

polymorphism

compile time (faster) - static polymorphism
runtime (slower)

compile time polymorphism
function overloading - write parameterized constructors, normal functions
int add(int a, int b){
  return a+b;
}
double add(double a, double b)
{
  return a+b;
}
both will run regardless of their same name because of different parameters

operator overloading
hw find all c++ operators which can be overloaded
Sure, Anubhav. In C++, you can overload the following operators:

1. Arithmetic operators: `+`, `-`, `*`, `/`, `%`
2. Relational operators: `==`, `!=`, `<`, `>`, `<=`, `>=`
3. Logical operators: `&&`, `||`, `!`
4. Bitwise operators: `&`, `|`, `^`, `~`, `<<`, `>>`
5. Assignment operators: `=`, `+=`, `-=`, `*=`, `/=`, `%=`, `&=`, `|=`, `^=`, `<<=`, `>>=`
6. Increment/decrement operators: `++`, `--`
7. Subscript operator: `[]`
8. Function call operator: `()`
9. Member access operators: `->`, `->*`, `.`, `.*`
10. Comma operator: `,`

These operators can be overloaded to provide custom behavior for user-defined types. If you have any specific questions about operator overloading or need examples, feel free to ask.

v1+v2; should be stored in v1
void operator+(const Vector &src){
    this->x = this->x + src.y
    this->y = this->y + src.y 
}
no need to write v1 = v1 + v2

hw deep vs shallow copy
Student s1 = s2; (default dumb copy constructor is called)(shallow copy)
deep copy when all the propoerties of any objects are independent of ther objects of the same class
for example when shallow copy is done, pointer of the new object will point to pointer to the input object,
this in turn would make both the object's pointer same, so changing one of them would simultaneusly change the other

can a constructor be made private? 
yes and no error at compile time if not used
use: to not make object of a class directly instead make a friend class and declare constructor there
also we can initialize a count variable with the constructor that would monitor how many ojbects of the priv class has been made

another use singleton class where constructor is made private too

resource learn microsoft constructors C++


y = new int(*obj.y); would be the solution to deep copy

runtime polymorphism(dynamic)

function overriding
static binding(by compiler): Problem: Animal*animal = new dog();//this line should run in runtime but animal sound was played at compile time
same animal sound will be played
animal.sound();


dynamice polymorphism
solution for making runtime decision over compile time for sound
- make animals sound as virtual that will allow compiler for late binding - overriding of animal sound by dog sound (lately)
animal: virtual sound() override
dog: void sound() override    this has to do with increasing readability

virtual keyword - method to leave decisions at runtime
it does so by making static arrays/tables function poitner table at compile tile

late binding 
runtime pr decision
compiler ko btnae ka ki take things less seriously at compile time instead wait for runtime

same things applies to destructor so animal destructor will be called if not made virtual and if made virtual then dog destructor will be called

downcasting - beta papa ko utha 
dog* a = new animal();
Upcast
animal*a=new dog(); and why using pointer so as to set up the late binding

compile time 
- static binding 
- early binding

without virtual keyword in parent class
left mei jo likha hai uska function call hoga

agr lga hai toh right side wali chizein

virtual void sound(){}
void sound override(){} - this override is not 

static keyword in class

static data member - variables that relate to instances of all the objects, to access such a variable
int student::x; int student::y; (outside the class)
static int x,y;(that's how you declare them in the class)
this one is differnt from the object variable that could be access by a.x or a.y is it universal for that class
so obj1.x=10; and obj2.x=20; are essentially using the same x variable


static member function static void print(){} 
abc::print(); that's how you call it
common to all objects and can't include non static instances of class
__FUNCTION__ it prints the name of the function
this pointers are not accessible

abstraction - delivering only essential information to the outer world while masking the background details
accessing private data members only through public methods of that class
g++ -std=c++11 file.cpp to compile it from the standard of c++11



abstract class
classes that contain atleast one pure virtual function and these classes can not be instantiated, they are used as inteface
and the classes that inherit this one would have to make virtual functions mandatorily


bird.h
#if !defines(BIRD_H)
#define  BIRD_H
#include <iostream>
class Bird{ //abstract class
  public:
    virtual void eat() = 0;
    virtual void fly() = 0;

}
class sparrow: public Bird{
  public:
    void eat(){
      cout << "sparrow is eating\n";
    }
}

#endif

Bird *bird = new sparrow();
birddoessth(bird);
that's called abstraction we are changing the sparrow to eagle or pigeon and it will call the methods of that subbird/subclass
and we can only call the method of a specific sub class through an object of the parent class 
here interface is the parent bird class that provides the blueprint of how a bird would act
then we have the implementation in which we inherit the abstract interface class

inline function - idea is to cut the space exhausted by stack filling to override the function calling
inline void print(int a)
{
  cout << a << endl;
}
used in small sized function
169. # interview

take it serious -cgpa bcoz its highly populated india

offcampus requires projects skills

now coding test - analytical, coding, technical writing 
DSA OS DBMS OOPs Computer Networks LLD HLD
(coding > aptitude > techincal writing)

now interview - 
interviewer - will skill behaviour articulation 
they think of the itnerviewee as working with them and check their willingness to complete the project

only tell what is asked

stop when prompted to

when he is speaking, listen intently

he will test your panic by saying rude things,
 saying right things as wrong
  and you have to back your arguments with proofs subtly without getting angered

uh o uhm is sred flag
either speak in hindi or english select one and stick to it
always answer from very basic not on high level
answer in a flow
don't assume he knows everything
be fearless he is an idiot

for experienced candidates they will ask your experience
alognwith doing your work
always ask your colleagues about their work to know about it 
and mention it in interview that you have worked and contributed in it too
this shows activeness, eagerness to learn

treat every coding question as new one
increase complexity step by step
use full time by medium length easy explanation without letting them know it articulate it in a medium length to consume thier time
always tell brute force approach if you know the hard one
interview is always personal not on comparision

always ask for hints repetition, sample i/o
if still don't know - tell honestly didn't study it
in theory questions be brutally honest and tell idk if not studied.
don't ask non-tech questions

don't cheat

do you have any questions for me?
don't ask 
salary
working hours
job work?

ask 
his experience 
his job role
work culture
expectations from a candidate in an interview at my level
questions in which interviewer will be comfotable to answer
current product he is working on

writing good code
use good identifiers
indentation
only required comments -add comments where the code is hard to understand
no magic numbers
#define STUDENTID 100

virtual interview
don't be oversmart
no cheating

project discussions
prepare for but obvious questions
- motivation to build this?
- why this?
- why not that?
- why only this stack?
- which tech stack is used?

hr round 
on campus
off campus
know salary expectations
know the situation in the market
connect with people already working that org
ask relevant question about the org
culture
work location
remote

170. # linked list

difference in struct and class
struct mei default public and class mei default private
struct is used for bundling of data
bundling + methods = class
only a conventional difference
<!-- do this with all types of ll -->
<!-- creation of ll -->
<!-- printing a ll  -->
<!-- finding length of ll  -->
pass by refernce when we need to modify the ll
<!-- insert at head  -->
<!-- insert at tail  -->
<!-- insert at position n  -->

creation of all types of ll
singly node has next pointer and one data holder
doubly has prev and next pointers and one data holder
circular singly ll has next pointer and one data holder and tail's next pointer to head
circular doubly ll has prev and next pointers and one data holder and tail's next pointer to head head's prev pointed to tail

insertion or deletion of a node can be on the following nodes in linked list

if head is null
at head
at tail
in between

Node a; creation of static object
accessing via a.data
Node *head = new Node(); creation of dynamic object
accessing via *head.data or head->data

where is linnked list used in real life?
can we use recursion to move backwards in a linked list.

in OS in storage management where linked list is used? ram free space management

linked liked can work on non-contnous memory

it only needs memory

less wastage than array

collection of nodes

where a node is two boxes one of which contains the data and other is a pointer that contains the address of the next node
node *ptr

class node{
  int data;
  node* nextnode;
}
// structure can be made too
struct Node {
    int data;
    Node* next;

    Node(int value) : data(value), next(nullptr) {}
};


last node points at null 

LL is hindi

insert/shift operations happens in O(1) complexity (location must be known)

can be grown/shrink in size at runtime/dynamically 

address ka concept not indices
pointers ka concept

there will always be an error due to a missed corner case in ll so don't panic

types depends on number of pointers 
singly
doubly
circular
circular doubly


while temp !=null print temp->data  temp = temp->next

always consider code reusability - save the work you did once with someone's help

insertion in ll
-make new node called temp
point it to head
make temp the new head
make sure to pass by refernce in this case to add at head
node* &head 
and make a copy then use acccording to the use case
after solivng the problem in ll
check for corner cases - empty linked list - one sized ll etc

insertion at tail
create new node
access tail node by doing temp!=null and updating temp by its next value
change tail pointer from null to temp
make temp as tail

insert at position n
create a new node
point it to 4th postion
point 3rd node to new node 
pass by refernce
if this is used at head or tail then call the insertathead and insertattail codes

delete in ll using position number

delete from head
create node temp pointing to head
head = head->next
temp -> next = NULL
delete temp

delete from tail
create node temp pointing to tail
traverse to second last node and point temp to it
point temp to null
delete tail 
tail -> temp

delete nth position
iterate to n-1 node 
call it temp1
call temp1->next = temp2
point temp1 to temp2->next
delete temp2
delete in ll using value

always solve question with engineering wali approach

 


reverse an ll leetcode
reverse an ll using recursion
by reversing the next pointers 


middle element of a linked list 
by traversing once to find length and then traversing again till half the length and reporting the answer
tortoise algorithm to find midddle of a ll
slow wala pointer 1 step aage bdhta hai
fast wala pointer 2 step aage bdhta hai
firstly fast wala pointer will move two steps if he can then slow wala pointer will move else no one does and where slow pointer stands that's the answer


palindrome in ll 234 leetcode
make new ll that is reverse of original
compare both
not a good practice to alter the data structure or modfiy the original data
divide the ll at mid using tortoise algo
reverse the last ll
store the last half in stack and compare it with the first half

check cycle in a ll
computer can detect a loop if it falls on the same address twice.
while traversing if address repeats then it is a loop confirmation
by creating a map of addresses we can check if an address marked true is visited again for loop presence
map<ListNode*, bool> table; //that creates a map 
using tortoise algo if fast and slow pointers overlap before fast meething the null pointer then it is a loop

detect and delete loop in a ll
find one node less than starting point of loop using tortoise algo then
point its next to null, loop removed!

add 1 to a linked list
reverse the ll
try adding 1 to the head node after reversing
if carry 0 break
if carry !=0 go to head->next and try adding 1 there 
if carry !=0 and ll ended then create a new node at tail with data as carry
reverse again

in ll questions tail won't be given  only head


add 2 numbers given by ll
reverse both the ll
create a new ll
try adding both head nodes after reversing to ll
if carry 0 break
if carry !=0 go to head->next in both the ll and try adding there 
if carry !=0 and if ll ended then create a new node at tail of new ll with carry

if first ll ends then proceed to add carry and the second ll until second ll ends too
if second ll ends and carry !=0 then we can add a node at tail and store carry there

if second ll ends then proceed to add carry and the first ll until first ll ends too
if first ll ends and carry !=0 then we can add a node at tail and store carry there

reverse again

reverse ll in k group
rev the first k group then let recurision solve the next
mistake can happen when we have to join the ll of recursion with the base ll that we solved


sort 0s 1s and 2s (dummy node)

remove duplicated froma sorted ll leetcode
compare temp to temp ka next and increment temp when unique

sort a ll

quicksort is better for ll/array?
mergesort is better for ll/array?

171. # Stack

LIFO

underflow - deleting from already empty stack

overflow - adding element in already full stack

ctrl z use caes abc pqr xyz in ms word

#include <stack>

stack<int>st;
stack<char>sre;
stack<node>st;

st.push(13);
st.pop();
st.empty();
st.size();
st.top();

implementation of stack be done with array, vector
get a dynamic array
int size
int top at -1

push -> top++ arr[top]=data
pop -> top--
empty -> if top = -1
getTop -> return arr[top]
getsize -> return top + 1

if I need reverse ordering of something then I can apply stack in between
insert and pop to get reverse

recursional things happen in stack so stack can also happen in recursive way
while (!st.empty())
middle element of a stack using recursion
keep a temp 
keep a pos acc to if stack elements are even or odd in number

insert at bottom of stack
use same recursive approach as in finding middle element 

reverse a stack 
store it in another stack 
OR 
if sth can be reversed with a stack it can be reversed with a recursion

insert in a sorted stack
same as recursive approach but instead of keeping a position varaible we are doing comparision with the element

whenever top element of a stack is accessed check whether it is empty or not before doing any operation

sort a stack
do insertsorted for every element after popping

implement two stacks in a single array
giving half memory to stack1 and stack2 will waste memory
just that top1 top2 two indices each at -1 and size so top 1 will increment and top2 will decrement
when space is not available this is the condition top2 - top1 = 1

top1 top2 push1 push2 pop1 pop2 

valid parenthesis algorithm

remove redundant brackets/ return true false if redundtant brackets found
if there is no operator between two brackets then return true bcoz that's redundant
if present then return false

implement a min stack where all operations take O(1) complexity
push pop top min all in O(1) time
155 leetcode

pair<int,int> a pair where two integers will be kept together in a block
pair<int,char> p = make_pair(4,5);
p.first
p.second
top - first pair value
min - second pair value
.back() last in stack
this stack structure is: vector<pair<int,int>>
storing the minimum value upto right in second element of pair
altering stack structure to decrease time complexity

next smaller element returning if not found return -1
brute force n2 
8 4 6  2  3 
2 2 2 -1 -1
rightmost element always has -1

previous smaller element

1475 final prices with a special discount in a shop
longest valid parenthesis

largest area in a histogram = w * h(from an index)
w = next smaller element index - prev smaller index - 1 

use an extra stack if recursion not allowed in a programming lang

practice.cpp:6:15: warning: overflow in conversion from 'long long int' to 'char' changes value from '134134131551' to '95' [-Woverflow]
    6 |     char ch = 134134131551;

pascals triangle ->
C = 1
C = C * (i - j) / j 



