# Approach 1: Using a Loop (e.g., for loop)

Procedure PrintCounting(m, n)
    for i from m to n i > n i --
        Print i
    
# Approach 2: Using a While Loop

Procedure PrintCounting(m, n)
    i = m
    while i >= n
        Print i
        i = i - 1
    
# Approach 3: Using Recursion

Procedure PrintCounting(m, n)
    if m >= n
        Print m
        PrintCounting(m - 1, n)

# Approach 4: Using Do-While Loop

Procedure PrintCounting(m, n)
    i = m
    do
        Print i
        i = i - 1
    while i >=n n