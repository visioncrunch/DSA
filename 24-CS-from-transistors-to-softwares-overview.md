**Header Files in C/C++:**

Header files in C and C++ are files that contain declarations of functions, variables, and other constructs. They often also include function prototypes, macros, constants, and type definitions. These files typically have a `.h` extension (e.g., `example.h`) and are used to organize and manage code in a modular and reusable way.

**How They Work:**

- **Declaration**: A header file contains declarations, which tell the compiler about the existence and type of functions, variables, and other constructs defined in other parts of the program.
  
- **Inclusion**: The `#include` directive is used to include a header file's content in a C or C++ source file. This is usually done at the beginning of the source file.

- **Preprocessing**: Before the actual compilation, a preprocessor processes the `#include` directives and replaces them with the content of the specified header files.

- **Compile**: The compiler then compiles the resulting source code, which now includes the content of the header files.