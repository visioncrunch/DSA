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

1. gcd(m,n) = gcd(m-n,n) if m>n
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

1. 

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
2. xor with whole xor
3. if arr[mid]-mid==1 go right s = m + 1 else store answer and go left e = mid-1

123. # rearrange +ve -ve in consecutive order with preserved order +-+-

1.

124. # return row with max 1s

1. count 1s in all rows and return row with maximum counts by storing the index of row which had the max 1s latestly

125. # rotate a matrix 90degree clockwise/anticlockwise

1. take transpose and reverse(matrix[i].begin(),matrix[i].end())

126. # binary search time complexity log2n

1. s=0 e=n-1 mid;
2. while s < e  // this depends on case whether to use <= or only <
3. mid = s+(e-s)/2 (saves memeory overflow if s and e are both INT_MAX)
4. if arr[m]id==target return mid
5. else if arr[mid]>target e = mid -1 // this also depends on case could have been e = mid
6. else start = mid + 1 // this also could have been s = mid

127. # find and element, first occurence, last occurence, total occurence

1. in all cases use binary search and total = last - first + 1 and keep storing possible answers

128. # key pair two sum

1. n =6 x = 16 arr{1,4,45,6,10,8} yes arr[3] + arr[4]
2. for i< n Y = X - arr[i] for j < n j!=i if arr[j] = Y return yes

129. # find pivot index before or after which sum is same

1. 

130. # peak element in a mountain array

1. 

131. # whixh swap is faster

1. xor is faster because it is more close to CPU

132. # custom comparator

0. bool mycomp(int&a,int&b){return a>b}
1. sort(v.begin(),v.end(), mycomp)
2. bool mycomp(vector<int>a,vector<int>b){return a[0]>b[0]; for 0based indexing return a[1]>b[1]; for 1based indexing}

133. 