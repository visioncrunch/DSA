1. # how to approach a problem

1. understand the objective
2. pay attention to the constraints
3. write a pseudocode of best case
4. inlcude corner cases
5. dry run it

2. # return minimum/maximum of three numbers

1. set ans = INT_MAX
2. iterate on all numbers and update ans as min(ans, number)
3. return ans

1. using ternary operators
    return a<b ? (a<c ? a : c) : (b<c ? b : c)  

1. sort array and report the smallest element as answer

1. use min function min(a,(min(b,c)))

3. # check prime or not

1. if any number from 2 to n-1 factors n then its not prime. else it is

1. if any number from 2 to sqrt(n) factors n then its not prime. else it is

1. sieve of eratosthenes

1. fermat's little theorem

1. miller rabin's primality test

1. AKS primality test

1. lucas-lehmer primality test

1. baillie-psw primality test

4. # statements a loop contains

1. initialization
2. condition
3. logic
4. updation

5. # loops

1. for
2. while
3. do-while
4. for-each

6. # check odd or even

1. if n%2==0 even
2. if n&1 odd
3. 1 and 2 can be written as:
    return n%2==0 ? even : odd
    return n&1==1 ? odd : even

7. # print counting from 1 to n / n to 1

1. for i in 1 to n print i

1. i = 1
2. while i<=n
        print i
        i++

1. use recursive fn 
    printnum(m, n)
        if m<=n
        print i
        printnum(m+1,n)

1. i = 1
2. do 
      print i
      i++ 
   while i<=n

8. # if else piecewise defined for each range

1. read n
2. if n in 91 to 100 print a 
3. else if n in 81 to 90 print b
4. else if n in 71 to 80 print c
5. else if n in 61 to 70 print d
6. else print e

9. # check +ve/-ve/0

1. if n<0 -ve
   else if n>0 +ve
   else 0

1. switch(n) (increases readability)(n must be int char long or any integer datatype)
        case(n<0): 
            -ve
            break; //break is important for termination of further execution
        case(n>0): 
            +ve
            break;
        default:
            0
            break;

1. return n>0 ? +ve : n<0 ? -ve : 0

10. # CheckTriangle(a, b, c) (output 1 or 0)

1. return (a + b > c) && (a + c > b) && (b + c > a);

11. # factorial of a number

1. fact = 1
2. for i in 2 to n 
        fact*=i
3. return fact

1. fact(n)
    if n ==1 or n==0
        return 0
    else
        return n*fact(n-1)

12. # print 1 to n odd numbers

1. change the updation from i++ to i = i + 2 and print the index

1. function print_odd_numbers(start, n):
2.   if start > n  : return   
3.   if start&1    : print start
4.   print_odd_numbers(start + 1, n)

13. # reverse a number

1.  while(n>0)
2.  rev = rev * 10 + num%10;
3.  num/=10;

14. # same after double reversal

1. return reverse(reverse(num))==num;

15. # movies for programmers

1. terminator
2. the matrix
3. the wolf of wallstreet


16. # LLM MLL HLL

1. C++, assembly language 
2. binary 
3. python, no code platforms

17. # working of compiler

1. Preprocessing:
   Includes expanding macros (#define AUTHOR "abcd").
   Inclusion of header files.
   Conditional compilation (#ifdef, #ifndef, #endif).

2. Remove Comments: Comments in the code are removed.

3. Source Code to Tokenization:
   Lexical analysis involves tokenizing the preprocessed code. Tokens are the smallest units in a programming language, such as keywords, identifiers, operators, and literals.

4. Syntax Analysis (Parsing):
   The token stream is used to build a parse tree or syntax tree, which represents the grammatical structure of the program.
   Handles the language syntax and verifies that the code adheres to the language grammar rules.

5. Semantic Analysis:
   This step involves analyzing the meaning of the code beyond its syntax.
   Checks for type compatibility (e.g., int a = "ABD";) and verifies that variables are declared before use.
   Resolves variable references and enforces scoping rules.

6. Intermediate Code Generation:
   Translates the syntax tree or the high-level representation of the code into an intermediate language (e.g., three-address code or an intermediate representation specific to the compiler).

7. Code Optimization:
   Performs various optimizations to improve the efficiency of the code, such as constant folding, common subexpression elimination, and dead code elimination.

8. Code Generation:
   Translates the optimized intermediate code into the target machine code (assembly code) for the specific processor architecture.

9. Linking:
   Combines multiple object files (resulting from compiling different source files) and resolves references between them.
   It resolves symbols (functions, variables) used across different files and libraries.

10. Object File Creation:
   The linked code is assembled into relocatable object files.

11. Executable Creation:
   The linker combines object files, libraries, and other necessary components to create the final executable file.

1. preprocessing -> compiling -> assembling -> linking 
2. #include<stdio.h> gets converted to prototype of printf scanf etc. and the functions are written at the end below the main function
3. compiling converts the source code to assembly code
4. assembler converts the assembly code to binary code. 
5. linking combines stdio.c cs50.c main.c into one large c file
./a.out - assembly output



18. # why need a programming language

Programming languages are essential tools that enable humans to communicate instructions to computers in a structured and understandable way. Here are several reasons why we need programming languages:

1. Communication with Computers:

Computers only understand machine language (binary code), which consists of 0s and 1s. Programming languages act as intermediaries, allowing humans to write code using a more intuitive and human-readable syntax.

2. Abstraction and Simplification:

Programming languages abstract complex operations and tasks, allowing developers to work at a higher level of understanding. They provide simplified constructs and functions to perform intricate operations without dealing with low-level hardware details.

3. Efficiency and Productivity:

Programming languages enable efficient coding by providing pre-defined functions, libraries, and frameworks that can be reused. This boosts productivity, as developers don't have to reinvent the wheel for common tasks.

4. Flexibility and Adaptability:

Different programming languages are designed for specific purposes and domains, offering flexibility to choose the most suitable language for a particular project. Some languages are best for web development, while others excel in data analysis, AI, or system programming.

5. Problem Solving and Logic:

Programming languages encourage structured thinking and problem-solving skills. Writing code requires breaking down complex problems into smaller, manageable steps, and then implementing logical solutions.

6. Automation and Repetitive Tasks:

Programming allows automation of repetitive tasks, saving time and effort. By writing scripts or programs, we can instruct computers to perform routine actions consistently and accurately.

7. Scalability and Maintainability:

Well-structured programming languages promote scalable code, making it easier to handle larger projects. They also facilitate code maintenance and updates, ensuring that software remains functional and relevant over time.

8. Innovation and Development:

New programming languages often introduce innovative features and capabilities that drive technological advancements. They enable the development of new software, applications, and technologies, pushing the boundaries of what's possible in the digital world.

9. Cross-Platform Compatibility:

Many programming languages are designed to work on multiple platforms and devices. This cross-platform compatibility allows developers to create applications that can run on various operating systems, enhancing accessibility and reach.


19. # header files 

1. Files that contain declarations of functions, variables, and other constructs. 
2. They often also include function prototypes, macros, constants, and type definitions. 
3. These files typically have a `.h` extension (e.g., `example.h`) and are used to organize and manage code in a modular and reusable way.

1. Declaration: It contains declarations, which tell the compiler about the existence and type of functions, variables, and other constructs defined in other parts of the program.
2. Inclusion: The `#include` directive is used to include a header file's content in a C or C++ source file. This is usually done at the beginning of the source file.
3. Preprocessing: Before the actual compilation, a preprocessor processes the `#include` directives and replaces them with the content of the specified header files.
4. Compile: The compiler then compiles the resulting source code, which now includes the content of the header files.
5. header files are included in the memory of the process that is happening.

20. # from transistors to softwares


1. Transistors and Logic Gates:
   Transistors are the fundamental building blocks of digital circuits.
   Logic gates (AND, OR, NOT) are created using transistors to perform basic operations (Boolean logic).

2. Combinational Logic:
   Combinational circuits use logic gates to process inputs and produce outputs based on the current input only.
   Important for understanding algorithms involving bitwise operations.

3. Sequential Logic and Flip-Flops:
   Flip-flops store binary information and are the basis of sequential circuits.
   Understanding flip-flops is crucial for algorithms involving state and memory management.

4. Registers and Memory:
   Registers store data that the CPU needs to process quickly.
   Memory (RAM) is crucial for storing and accessing variables and data structures efficiently, which is vital in DSA.

5. Assembly Language and Machine Code:
   Assembly language is a low-level human-readable representation of machine code.
   Understanding assembly is essential for algorithm optimization, especially for time-critical operations.

6. Operating Systems:
   Operating systems provide an interface between hardware and software.
   Understanding OS concepts (processes, threads, scheduling) is important for designing efficient algorithms and data structures.

7. Programming Languages:
   High-level languages (e.g., C++, Java, Python) abstract hardware details, allowing developers to focus on algorithm design and data structures.
   Knowledge of programming languages is crucial for implementing and optimizing algorithms.

8. Data Structures:
   DSA involves understanding and implementing various data structures (arrays, linked lists, trees, graphs, etc.) and algorithms (sorting, searching, etc.).
   Efficiency in data structure choices impacts algorithm performance.

9. Compilers and Interpreters:
   Compilers translate high-level code to machine code, optimizing and improving efficiency.
   Interpreters execute code directly but often with a performance trade-off.
   Knowledge of how compilers work is essential for writing efficient code.

10. Software Development Lifecycle:
    Understanding the software development process (requirements, design, implementation, testing, maintenance) is crucial for building robust and efficient software systems.

11. Algorithms:
    DSA includes the study of various algorithms for solving specific problems efficiently.
    Analyzing algorithm complexity (time and space) is essential for optimizing and choosing appropriate algorithms.

12. Optimization and Performance Tuning:
    Profiling and optimizing code for better performance are essential skills in DSA, especially for handling large datasets and complex operations.

Understanding the interplay between hardware and software at each level is vital for designing efficient algorithms and implementing them effectively, considering both time and space complexities.

21. # getch function()

1. #include <stdio.h>
2. #include <conio.h>  // for getch() function

3. int main() {
    printf("Press any key to exit...\n");
    getch();  // Wait for a keypress then exit from the program
    return 0; }

22. # how computer understands binary

Computers understand binary, which is a base-2 numerical system, because the fundamental building blocks of computers, such as transistors and electronic circuits, can easily represent and operate using two states: on and off, or 1 and 0. These states align perfectly with the binary system, where 1 represents "on" or true, and 0 represents "off" or false.

Here's how computers interpret binary:

1. Bit (Binary Digit):
   The basic unit of information in a computer is a bit, which can be either 0 or 1. It's the smallest piece of data in binary representation.

2. Bytes and Words:
   A group of 8 bits forms a byte. Bytes are commonly used as the basic unit for representing and manipulating data. Multiple bytes grouped together form words, which represent larger units of data.

3. Representation of Numbers:
   Binary is used to represent numbers, where each position in a binary number represents a power of 2. Starting from the rightmost digit, each position corresponds to 2^n, where n is the position's index.

      For example:
      \(1011_2\) in binary is \(1 \times 2^3 + 0 \times 2^2 + 1 \times 2^1 + 1 \times 2^0\), which is equal to \(11_{10}\) in decimal.

4. Representation of Characters:
   In computing, characters (letters, numbers, symbols) are also represented using binary. Common encoding schemes like ASCII and Unicode assign unique binary patterns to each character.

5. Instruction Execution:
   Machine language instructions are encoded in binary. The CPU interprets these binary instructions and performs the corresponding operations, such as arithmetic, logic, or data manipulation.

6. Storage and Memory:
   Data stored in computer memory (RAM, hard drives, etc.) is represented in binary. Each byte of data is stored as a series of 8 bits, with each bit having a value of 0 or 1.

7. Data Processing and Logic Operations:
   Logical operations (AND, OR, NOT) and arithmetic operations (addition, subtraction, etc.) are performed using binary arithmetic and logic gates, which are the basis of all computation in a computer.

Computers use electrical signals to represent these binary values (0 or 1), with voltages or states corresponding to these digits. Complex circuits and processors are designed to process and manipulate binary data efficiently, allowing computers to perform a wide array of tasks, from simple calculations to complex operations in software applications.


23. # optimization

1. a program can have multiple solutions but as a programmer our job is to find the most efficient one.

24. # fact about compiler

1. it was written by yet another compiler of previous version. hence automating the automation.

25. # where does a program starts

1. at the main function and it's the only function that is detected by compiler as the starting point

26. # function

1. a function takes input, applies the embedded logic in it, and then processes the output
2. return type name(argument type argname){return statement in line with return datatype at the end}

27. # working of cout

1. `cout << "Anubhav";`, is a C++ code snippet using the Standard Library for output.

2.  `cout`:
   `cout` is the standard output stream in C++. It is an object of the `iostream` class, which represents the standard output device, typically the console or terminal.

3.  `<<` (Insertion Operator):
   The `<<` operator in C++ is called the insertion operator. It is used to insert data into the output stream, in this case, the `cout` stream.

4.  `"Anubhav"`:
   `"Anubhav"` is a string literal, which is a sequence of characters enclosed within double quotes. In this case, it represents the text "Anubhav".

5. Output to the Console:
   The `cout` stream, combined with the `<<` operator, is used to send the string "Anubhav" to the standard output (usually the console). The `<<` operator inserts the string into the `cout` stream, and it gets displayed on the console.

6. Final Output:
   When this statement is executed, "Anubhav" is displayed on the console.

Putting it all together, `cout << "Anubhav";` instructs the program to output the string "Anubhav" to the standard output, typically the console, using the `cout` stream and the insertion operator (`<<`). This is a fundamental way to display information in C++ programs.

28. # why include iostream

1. because it has declaration of cout cin and other important functions

29. # identifiers--tokens-literals

1. Identifiers:
   Definition: An identifier is a name given to a program element, such as variables, functions, classes, etc., to uniquely identify them in a program.
   Rules for Naming Identifiers:
     Must start with a letter (a-z, A-Z) or an underscore (_).
     Can be followed by letters, digits (0-9), or underscores.
     Cannot be a keyword (reserved word).
     Cannot contain spaces or special characters (except underscores).
   Example Identifiers: `variableName`, `function_1`, `ClassA`.

2. Tokens:
   Definition: Tokens are the smallest units of a program that have meaning. In programming languages, tokens can be identifiers, literals, operators, keywords, and punctuation symbols.
   Example Tokens: `if` (a keyword), `123` (a numeric literal), `+` (an operator), `variableName` (an identifier).

3. Literals:
   Definition: Literals are constant values that are used in a program. They represent fixed values that do not change during the program's execution.
   Types of Literals:
     Numeric Literals: Represent numbers (e.g., integers, floating-point numbers).
       Example: `123`, `3.14`.
     String Literals: Represent sequences of characters enclosed in double or single quotes.
       Example: `"Hello, World!"`, `'A'`.
     Boolean Literals: Represent true or false values.
       Example: `true`, `false`.
     Null Literal: Represents a null or empty value.
       Example: `nullptr` (in C++).

4. Keywords:
   Definition: Keywords are reserved words in a programming language that have special meaning and cannot be used as identifiers or for any other purpose.
   Examples of C++ Keywords: `if`, `else`, `while`, `for`, `int`, `double`, `class`, `return`, `break`, `switch`, etc.
   Usage: Keywords are used to define the syntax and structure of a program. For example, `if` is used to start a conditional block, and `int` is used to declare an integer variable.

In summary, identifiers are names given to program elements, tokens are the smallest units with meaning, literals are constant values, and keywords are reserved words with specific meanings in a programming language. Understanding and using these concepts is fundamental in writing and comprehending code in any programming language.

30. # end of line or newline

1. Portability:
The "newline character" ("\n") is widely accepted and standardized across different programming languages, platforms, and operating systems. It ensures portability and consistency in representing the end of a line.

2. Consistency and Clarity:
Using "\n" as the newline character is a clear and consistent way to denote line endings in text. It's easily recognizable and understood by programmers, making code more readable and maintainable.

3. Compatibility:
Most programming languages and text processing tools interpret "\n" as the newline character. Using this convention ensures compatibility and interoperability with various tools and systems.

4. Efficiency:
The "newline character" ("\n") is efficient in terms of both memory usage and processing time. It requires just one character to represent the end of a line and is handled efficiently by modern programming environments and libraries.

31. # vscode shortcuts 

1. ctrl + g   go to a specific line no
2. ctrl + f2  select all the occurences of a word
3. ctrl + p quick open files
4. ctrl + shift + f search across files in the project
5. ctrl + fn + home - goes to starting of document
6. ctrl + fn + end - goes to ending of document
7. ctrl + f to find some words press enter to replace, esc to exit
8. f5 to debug
9. shift ctrl debug to restart debug
10. shift f5 to stop debug
11. step over f10 step into f11 continue f5

32. # why return statements at the end of functions

1. to indicate a successful termination of the function and perform its side effects

33. # graph of reality

1. starts from 100thousands
2. decreases exponetially
3. stops at around some hundreds

34. # flow of execution

The flow of execution of a program refers to the sequence in which the instructions and statements in a program are executed. This sequence follows a particular order, which can vary based on the programming language and the structure of the program. Here's a general overview of the typical flow of execution in a program:

1. Initialization:
   Variables and data structures are initialized with default values or values specified by the programmer.

2. Input:
   The program may prompt the user for input or read input from files or other sources.

3. Control Flow:
   Based on conditional statements (e.g., if, switch), the program determines which code block to execute next.

4. Loops:
   Iterative structures (e.g., for, while, do-while) execute a specific block of code repeatedly until a condition is met.

5. Function Calls:
   The program may call functions or methods to execute specific blocks of code, possibly passing arguments.

6. Execution of Statements:
   The program executes statements in a sequential manner unless controlled by loops, conditional statements, or function calls.

7. Modifying Data:
   Data may be modified or updated based on calculations, operations, or user input.

8. Error Handling:
   The program may check for errors or exceptions, and appropriate actions are taken to handle them.

9. Output:
   The program generates output, which can be displayed to the user, stored in files, or sent to other systems.

10. Termination:
    The program reaches its end or encounters an exit condition, and the execution is completed.

Understanding this flow of execution is crucial for programmers to create efficient and functional programs. Proper control flow, efficient use of functions, appropriate error handling, and effective output generation are essential aspects of writing robust and maintainable code.

35. # gcd(greatest common divisor)

1. gcd(m,n) = gcd(m-n,n) if m>n use this minus program over modulo
2. gcd(m,n) = gcd(m%n,n) if m>n
3. if n is zero return m
4. else return gcd(n,m%n)

it doesn't matter whoever is greater than another they would be swapped of the divisor is greater, anyways

36. # lcm(lowest common multiple)

1.  gcd * lcm = a * b  (so if i know gcd lcm can be found out) 

37. # story of int a = 5

1. an integer of 4bytes of size named a that's equal to the literal value 5 stored at an address(say 104)
2. char has 1 byte of memory
3. bool has also 1byte of memory
4. long in 64 bit cpu is of 8bytes and in 32 its 4bytes
5. int num; cout<< num; prints garbage value
6. variable naming - telMeter, area_of_circle, flight1, greatestDivisor

38. # how data and address of a variable is stored

1. data is stored as binary digits
2. address is stored as a hexadecimal value
3. char a = '97' means the letter a 
4. char is an integer datatype
5. smallest unit of memory that can be represented is a byte

39. # number system conversion

40. # storage of -ve numbers

1. 1s complement - negate all the bits
2. 2s complement - 1s complement and then add 1 to result
3. so -5 = ~5 + 1
4. range of signed int is 2^31-1 to -2^31
5. range of unsigned int is 2^32-1 to 0

41. # char ch = 239094094 output?

1. garbage value

42. # logical operators

1. && || !

43. # boilerplate code

1.  #include<iostream>
   using namespace std;
   int main(){

   return 0;
   }

44. # namespaces

1. 

45. # preprocessor directives

1. 

46. # range of different datatypes

1. char  -128,127
2. short -32K, 32K
3. int -2 billion, 2 billion
4. long -9 billion, 9 billion
5. decalaration int a;
6. initialization int a = 5;

47. # how fractions, powers, exponentials are represented?

1. 

48. # smallest representable unit in computer

1. byte and that's why boolean uses 8 bits instead of 1 bit.

49. # why counting starts from 0?

1. 

50. # typecasting

1. implicit - compiler promotes one type to larger type float a = 3/5.0 = 0.6
2. explicit - int a = (int)c where c is float
3. either one of them must be float in division for result to be float

51. # operators

1. 

52. # 32bit vs 64bit architecture

1. 32 bit CPU can process 32 bits of instructions per cycle
2. 64 bit CPU can process 64 bits of instructions per cycle
3. addressable memory 2^64-1 upperlimit as opposed to 2^32-1 in a 32 bit cpu
4. resource usage more rams can be installed as opposed to only 4gb ram in a 32bit cpu and a 4gb ram in 64 bit cpu will be used more efficiently than if it was in a 32bit processor
5. double work per cycle as compared to 32 bit cpu
6. compatibility with 32bit softwares as well
7. better graphics performance
8. more security and signed processors
9. stops kernel patching with software
10. data execution/deletion prevention
11. ram limitation is just a software not a physical limitation
12. program files has 64bit files
13. and program files(x86) have 32 bit files


53. # decimal to binary

1. division method

2. bitwise n&1 method

54. # last digit of a number

1. mod by 10

55. # number excluding the last digit

1. divide by 10

56. # binary to decimal conversion

1. multiply with place value method

57. # computer's dumb

1. can't understand things at high level

58. # what exactly header files do

1. taking input
2. displaying output
3. accessing keyboard's pressed keys,etc.

59. # compile code in terminal

1. 

60. # run object file in terminal

1. 

61. # how to run files in C++/JAVA/Python

1. 

62. # extensnion of executables in: 

1. windows  .exe
2. mac/unix  .out

63. # java's compiltation story

1. every os has its own JVM thaat can run the universal bytecode interpreted by javac

64. # principal of mathematical induction

1. 

65. # patterns learnt while drawing shapes

1. 

66. # printf vs cout

1. printf is backward compatible with cout

67. # what is terminal

1. it is a command line interface and a program of OS that gives computer the access to physical world

68. # which g++

1. a compiler program found in user/bin

69. # what is cin

1. character input

70. # does keyboard input goes directly to program?

1. terminal takes the keyboard input and passes it on to software

71. # does program output goes directly to screen?

1. terminal takes output from program and passes it on to screen

72. # when are blocks copulsory

1. when there are multiple statements involved

73. # infinite for loop

1. for(;;){}

74. # if (cin>>n) or if(cout<<n)

1. cin cout return true if they take or produce the output

75. # what does ./a.out does?

1. it takes the executable to ram from rom and os runs it if main is there

76. # P1 P2

1. P1 P2 if P2 returns 0 implies the function P2 runs perfectly, hence indicating perfect termination

77. # what g++ does?

1. g++ converts a text file to .exe program. g++ is defined uniquely for every os systems

78. # xor

1. same bits - zero; different bits - one

79. # << >>

1. "x >> n" this just divides number by 2^n
2. "x << n" this just mulitplies number by 2^n
3.  by default signed integer is formed and >> works fine in handling the sign (sign dhifting occurs here)
4. for unsigned, right shift can change the value to a drastically large value
5. n<<1 produces a garbage value and gives a warining not an error

80. #  i++ and ++i

1. i++ executes then increments
2. ++i increments then executes
3. cout << a++*++a can produce different outputs on different compilers

81. # -10 >> 1 = -5

1. 00001010 
2. apply 1s complement - 11110101
3. add 1 - 11110110
4. ">>" 11111011 (that should be the answer but)
5. apply 1s complement - 00000100
6. add 1 - 111110101  -5

82. # ~1 = -2

1. 00000001
2. 11111110
3. 10000001
4. 10000010

83. # for if continue;

1. skips to next iteration by not executing the current iteration's unexecuted code

84. # for if break;

2. breaks out of the whole loop it is nested in

85. # global variable - bad practice

1. because it can be modified during program execution

86. # goto

1. 

87. # operators precedence

1. use brackets always to avoid it

88. # call stack

1. 

89. # some pre-defined useful functions in c++ library

1. 

90. # 5^-5 = -2

1.   5 = 00000101
2.  -5 = 11111011
3. xor = 11111110 (not correctly stored)
4. ans = 00000010 (2s complement applied)

91. # fastest loop

1. all are of smae speed

92. # which one to use if elseif else or if if else

1. for possibility of multiple conditions to be correct use if if if else otherwise for one condition use if elseif else

93. # count no of digits in a number

1. while n>0
2. n/=10
3. count++

94. # for each loop

1. for(auto i:st){cout<<i}

95. # ASCII

1. 

96. # header files class example

1. 

97. # array

1. why? to make n variables efficiently without naming all of them
2. int br[10];
3. address of oth element in array (104) then increments by size of data for subsequent element (108,112,116 if it was an integer array) 
4. addressof(); returns first element address in array
5. sizeof(); returns size of array
6. &arr gives address of that array
7. a[0] is smae as 0[a]
8. int a[3]; all garbage values
9. int a[]={1,2,3};
10. int a[3] = {1,2,3};
11. int a[5] = {2,4} -> {2,4,0,0,0}
12. int b[2] = {1,2,3,4} -> error
13. int n; cin >> n; in arr[n];  bad practice - possible that memory demanded is unavailable (instead use dynamic arrays)
14. addressof(arr[i]) = base index address + i*data type size 
15. linear search if arr[i] == target -> cout<<"found" break;

98. # generics

1. 

99. # adding 2 hexadeicals

1. a1c + a2b = 1547

100. # time complexity (increasing order)

1. 1,log2n,rootn,n,nlogn,n2,n3,2^n,n!,n^n
2. m+n if seperated loops
3. m*n if nested loops

101. # symbol table

1. var   address
2.  a      104 (hexadecimal value)
3.  b      232

102. # array passed into function

1. solve(int arr[], int size){}   
2. solve(int arr[][]4, int row, int col){}
3. whether or not you are giving 1st dimension, the successive dimensions are needed to be given

103. # count 0s and 1s in an array, dnfp, sort 2,1,0 sorting, -ve +ve sorting

1. while l < r
2. if l == 0 l++
3. if r == 1 r--
4. else swap(arr[l++],arr[r--])

1. use sort function sor(arr,arr+n)

1. can count all the 0s and 1s linearly and print 0s and 1s their count times

104. # return more than one values

1. in form of list tuple dictionary vector array and access their elements

105. # reverse an array

1. swap[arr[left++],arr[right--]] for i <n/2 
2. reverse[arr,arr+n]
3. for i=n-1 i>=0 i-- print arr[i]

106. # extreme print an array

1. until left > right print arr[left++], arr[right--]

107. # swap function

1. arithmetic method (a,b)
2. a = a+b
3. b = a-b
4. a = a-b

1. xor
2. a = a xor b
3. b = a xor b
4. a = a xor a

1. temp variable
2. temp = a
3. a = b
4. b = temp

108. # pass by value vs pass by refernce

1. by value makes copy always, not alters the real data, is limited to its scope, has different address
2. by refernce is &a, it's like altering the real data

109. # int &b = a

1. same memory location two names(a and b)
2. so cout << a is same as cout << b 

110. # arrays always get passed by reference

1. int solve(arr[], int size) no need to write int&arr[]

111. # important subjects

1. LLD, HLD, DSA, Web Development, 2 tagde projects, OOPs concept, DBMS, OS

112. # find unique elements in an array

1. xor all of them

113. # 0 xor a

1. a 

114. # print all pairs of an array

1. for i < n for j=i j < n cout arr[i], arr[j]
2. for i < n for j=i j < n for k = j k < n cout arr[i], arr[j], arr[k]
3. why j = i k = j (to avoid duplicate element pairs)

115. # while(count--)

1. runs till count is not 0

116. # shift array by n

1. implement shift function(swap(arr[i], arr[0])) k times
2. implement circular  approach (i+k)%n is the new index where value at index i will go
   make a new array
   for i <n 
   newarr[(i+k)%n]=arr[i]
3. extraspace method reverse(0,n-1) -> reverse(0,k-1) -> rev(k,n-1)
   123456
   654321
   564321
   651234



117. # run .exe

1. cmd  main.exe
2. powershell  .\main.exe

118. # static memory allocation

1. 

119. # dynamic memory allocation

1. 
 
120. # count set bits

1. use n&1 in each iteration and count
2. while(n) {n = n& n-1 count ++} return count

121. # vector

1. #include <vector>
2. int arr[5] static array
3. int n;
4. cin>>n;
5. int arr[n] redundant and bad practice
6. int * arr = new int[n]; dunamic array(still can't push more elements, size is fixed)
7. vector<int>v; 0 size
8. vector< vector << int >> v;
9. {5,-1} of size 5 and all values -1
10. {5} of size 5 and all values 0
11. v.push_back(n)
12. v.clear() clears whole vector data
13. vector<int>crr{1,2,3,4,5}
14. vector<int>brr={1,2,3,4}
15. vector<int>x(v) to copy other vector's data
16. v[0] first element
17. v[v.size()-1] last element
18. v.front(); first element
19. v.end(); last element
20. print using  ector method for(auto it:v){cout<< it };
21. 2d vector row size - v.size(); col size - v[i].size()
22. vector<vector<int>>arr(5,vector<int>(10,-1));  2d vector of 5 rows of size 10 each with all values -1
23. 2d index in 1d form c*i + j
24. rowwise access i < row j < col print v[i][j]
25. colwise access i < col j < row print v[j][i]
26. diagonal sum for i < row cout arr[i][i] (first diagonal)
27. diagonal sum for i < row cout arr[i][row-i-1](second diagonal)
28. transpose of matrix for i < n for j = i j < n swaparr[i][j],arr[j][i] (analyze the index patterns for printing via other traiangles)
29. i = 2 j = 2,1,0
    i = 1 j = 1,0
    i = 0 j = 0
30. reverse vector reverse(v.begin(),v.end())
31. jagged array v.push_back(v1), v.push_back(v2) and so on

122. # missing element {1,2,3,4,5,6,7,8}

1. calculate sum and subtract it from wholesum to get missing element

1. xor with whole xor

1. initialize answer as 0
2. if arr[mid]-mid = 1 move right -> start = mid + 1 //coz pattern didn't break move on
3. else if arr[mid]-mid != 1 store mid as answer and end = mid - 1 //pattern broke answer could have been skipped so move left
4. update mid and repeat 1 and 2 until start > end 
5. if answer = 0 then return n + 1 //it means last element is missing
6. else return answer
7. midify this approach to include the corner case(not done till now)

123. # rearrange +ve -ve in consecutive order with preserved order +-+-

1. 

124. # return row with max 1s

1. count 1s in all rows and return row with maximum counts by storing the index of row which had the max 1s latestly

125. # rotate a matrix 90degree clockwise/anticlockwise

1. take transpose and reverse(matrix[i].begin(),matrix[i].end())

126. # binary search time complexity log2n

1. s=0 e=n-1 mid;
2. while s < e  // this depends on case whether to use <= or only <
3. mid = s+(e-s)/2
4. if arr[m]id==target return mid
5. else if arr[mid]>target e = mid -1 // this also depends on case could have been e = mid
6. else start = mid + 1 // this also could have been s = mid
7. why monotonic function: we are able to neglect half the problem hence reducing the size
8. why binary search time complexity is very less
9. why s + (e-s)/2 INT_MAX + INT_MAX > range of integer
10. when s = e what does it mean? it represents single array element of size 1

127. # find and element, first occurence, last occurence, total occurence

1. in all cases use binary search and total = last - first + 1 and keep storing possible answers
2. for first occurence if we find an answer store it and move left because we might have skipped the first occurence and treated further occurences as first
3. same for last occurence just move right in order to check possible last occurence if skipped
it's code
0. initialize answer as -1
1. give start and end index
2. calculate mid index as s + (e-s)/2
3. if middle == target: store that mid index as answer and end = mid - 1 (for first occurence) or start = mid + 1(for last occurence);
   else if middle > target ? end = mid -1 :: start = mid + 1
4. repeat 2 and 3 until start>end
5. return answer;

128. # key pair two sum

1. n =6 x = 16 arr{1,4,45,6,10,8} yes arr[3] + arr[4]
2. for i< n Y = X - arr[i] for j < n j!=i if arr[j] = Y return yes

129. # find pivot index before or after which sum is same

1. 

130. # peak element in a mountain array

1. declare those start end mid and ans = -1
2. if arr mid > arr mid + 1 : store mid in answer and move left - > end = mid //answer could have been skipped and end = mid so as to not skip peak
3. else start = mid + 1
4. update mid repeat 2 to 3 until start >=end 
5. return answer
6. why stop when start>=end
   if start equals end then at only one element currently we would be iterating infinitely
   suppose s = 5 e = 5 m = 5 then certainly we are in step 2 condition when it is true we are reupdating end = mid that is 5 so again s = e = m = 5 so infinite loop

131. # whixh swap is faster

1. xor is faster because it is more close to CPU

132. # custom comparator

0. bool mycomp(int&a,int&b){return a>b}
1. sort(v.begin(),v.end(), mycomp)
2. bool mycomp(vector<int>a,vector<int>b){return a[0]>b[0]; for 0based indexing return a[1]>b[1]; for 1based indexing}

1.
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

133. # advanced questions of binary are based on

1. if found target store answer and move to intended portion of array and proceed to find another possible better approximate solution


134. # general practice

1. make copy then make modifications on that copy. do not alter the original data.

135. # pivot in sorted rotated array

    4 5 6 7 1 2 3
1. declare those start end mid 
2. if s == e then return s
3. else if arr mid < arr mid - 1 and mid - 1 >= 0 return mid - 1; //this is the case when mid is at the lowest element  // range out of bound error can come in here
4. else if arr mid > arr mid + 1 and mid + 1 < n return mid; //this is the case when mid is at the highest index      // same range out of bound error can come here
5. else if arr start > arr mid end = mid - 1 //at the lower line of graph, move backward
6. else s = mid + 1 //at the upper line of graph, move forward
7. update mid repeat 2 to 6 until start > end;

136. # pseudocode of square root of a number correct to n decimal places

1. define search space(the changing dynamic reduced range of possible answers) from answer space(the range of numbers that can be possible answers)
2. define the predicate function which will be applied on mid
3. based on output of this function decide whether to go left or right (advanced concept of binary search)

for example if i have to find sqrt of 68
i know it must be in range [0,68) (my answer space)
and my predicate function is mid*mid < 68 it can either say true or false 
if it is equal then return mid
if greater then go left
else if mid*mid < 68 store the answer, go to right (predicate function is true here only)  
hence minimizing search space by halfing the range

wherever predicate function gives true then store those answers isntantly
for example mid*mid<68 is true for mid = 6,7,8,8.1,8.2,...

to configure it for giving sqrt upto n decimal precision
1. define a double precision variable that stores 0.1 if precision is 1 0.01 if precision is 2
2. now apply mid+= mid/10 if mid*mid < 68  (to be continued...)

137. # binary search on 2d array pseudocode

1. c*i + j = address of ith element of a 2d array in 1d format
2. declare start end mid as before
3. i = mid/c j = mid%c  are indices of a 1d array in 1d format
4. same binary search code of 1d array just replace arr[mid] with currindex=arr[i][j]

138. # divide 2 numbers using binary search

dividend = quotient * divisor + remainder

1. range 0 to dividend 
2. if arr[mid]*divisior == dividend -> return arr[mid]
3. else if arr[mid]*divisor > dividend -> end = mid - 1
4. else store answer and start = mid + 1
5. repeat 2 to 4 until start > end

139. # binary search in a nearly sorted array
in case of sorted array there is only one condition
in a nearly sorted array, arr at index can be at position mid-1 mid mid +1

1. if arr[mid]==target return mid; (in case of nearly sorted array ther are three cases)
1. if arr[mid]==target return mid;
2. if arr[mid-1]==target return mid -1;
3. if arr[mid+1]==target return mid+1;
4. if arr[mid]> target end = mid -2
5. if arr[mid]< target start = mid + 2 
6. why 4,5 steps (to be continued...)

140. # find odd occuring element via binary search
an array with all elements even no of times except one number that occurs odd times
all repeating numbers come in pairs
and all pairs do not repeat
one number can't come more that 2 times at a time

1. xor method
2. count method
3. binary search method

0. observation:
    a) starting element of pairs before odd element stand on even index
    b) starting element of pairs after odd element stand on odd index
    c) for single element cases, the single element is the only answer

1. if mid % 2 == 0 then //for even indices
      
      if arr mid == arr mid + 1 
          
          then standing at left -> to move right s = mid +2
          
      else right -> to move left e = mid coz it can also contain answer

2. if mid % 2 != 0 then //for odd indices
    
      if arr mid == arr mid - 1
        
         then standing at left -> to move right s = mid + 1 
        
      else right -> to move left e = mid -1 

141. # interview hack

1. don't show that you know everything, take moer time, do it so that he can see your curiosity
2. first tell all the approaches and then wait
3. if he asks to solve ONLY then solve otherwise DON'T

142. # why it is important to tell col size when using a 2d array in function

1. its column size coz c*i + j

143. # basic math for dsa

Prime Number
1. Naive Approach:
 In this naive approach, we start from 2 (the smallest prime number) and iterate up to n-1,
 checking if n is divisible by any number in this range. 
 If it is divisible by any number, it's not a prime number. Otherwise, it's a prime number.

2. Square Root Approach:
 In this square root approach, we only need to check divisors up to the square root of n
 because if n is not a prime number, it must have a divisor smaller than or equal to its square root.

3. Sieve of Eratosthenes
 Start with a list of numbers from 2 up to the desired limit.
 Start with the first number (2) and mark all of its multiples as non-prime.
 Move to the next unmarked number (3) and repeat the process.
 Continue this process until you reach the square root of the limit.

1. make a bool vector (prime) of all numbers from 0 to n with all elements marked as true
2. mark 0th 1st element as false and make an ans variable for recording count of primes
3. for i = 2 i < sqrt(n) 
        if(prime[i])
            ans++ 
            j=i*i //becoz all multiples smaller than this number will be marked in previous iterations
            All multiples of primes smaller than p have been marked in previous iterations, not their squares (which is why we start marking from p×p).
            
            for j < n
                prime[j]=false  //marking all of the multiples of prime numbers as false
                j+=i
    return ans

    Time complexity = O(n*log(log(n)))

4. Segmented Sieve
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

146. # bubblesort principle
swap the adjacents if needed, till we get the largest element to the right in every iteration

for i < n-1 // coz the remaining element is sorted anyways so omit the last iteration
for j < n - i - 1  //j is the number of swaps for each iteration of i 
if arr j > arr j+1 then swap both (for ascending sort)
if arr j < arr j+1 then swap both (for descending sort)

147. # insertion sort

run i from 1 to n-1
set key = v[i]
run j from i-1 to j>=0 


for i in 1 to n-1
    set j = i-1
    set key = v[i]
    while j>=0 and v[j] > v[key]
        set v[j+1]=v[j]  //shifting the greater value to right
        j--  //concept of using out of range loop for program logic
    v[j+1]=key //shifting the key to left

why make key when we can directly use i
    the value at ith index will change with iterations that's why assigning its value to a key is important

148. # selection sort

principle
find the smallest element and swap it with ith element
for ith iteration in [0,n-1)
 declare minindex = i on every iteration
  and pick smallest element from j = i+1 to n-1
   and then compare j with minindex
   store minimum of both in minindex
    out from the j loop run the swap operation on minindex and i

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
  str1.append(str2);

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


  if(str1.find(str2) == string::npos){
   //not found
   cout << "Not FOund" << endl;
  }
  else {
   cout << "Found" << endl;
  }

  string str1 = "babbar";
  string str2 = "Love";

  if(str1.compare(str2) == 0) {     equals 0 when compared string is equal, >0 for longer and <0 for shorter
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
printf("%0.10f",doubleValue);
%n.mf means use n width and m decimal place of precision  
printf statement utilites
Exactly, you've got it right!

In the `printf` statement `printf("%n.mf", aDoubleValue)`, if `n` is a specified minimum width and `m` is the specified precision for decimal places, here's what happens:

1. **Minimum Width (`n`)**: The `n` value ensures a minimum width for the output. If the actual output is less than `n` characters, it will be padded with spaces on the left to meet the minimum width requirement.

2. **Precision (`m`)**: The `m` value specifies the number of decimal places to display for the floating-point number. It controls how many digits will be displayed after the decimal point.

So, for example:
- `%5.6f` will ensure a minimum width of 5 characters and display up to 6 decimal places of precision.
- `%5.100f` will also ensure a minimum width of 5 characters but display up to 100 decimal places of precision.

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

int a = 5
int*p = &a
solve(p) (*p = *p +5)
cout p &p *p in main = &a, &p, 5 in solve &a, &p(of the new p formed in solve), 10

pass by value int*p
pass by refernce int*&p (same things for pointers, no discrimination)
