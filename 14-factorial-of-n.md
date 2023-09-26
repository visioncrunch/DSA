The factorial of a non-negative integer n is denoted by n! and is the product of all positive integers from 1 to n.

# Approach 1: Iterative Approach

Procedure FactorialIterative(n)
    result = 1
    for i from 1 to n
        result = result * i
    end for
    return result
End Procedure

# Approach 2: Recursive Approach

Function FactorialRecursive(n)
    if n equals 0 or n equals 1
        return 1
    else
        return n * FactorialRecursive(n - 1)
    end if
End Function



