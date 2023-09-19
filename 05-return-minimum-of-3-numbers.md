# first approach

1. read all inputs: a, b, c
2. initialize a variable called minimum with INT_MIN of header limits.h
3. if a < minimum set minimum = a
4. do step 3 for b and c too
5. return minimum

# second approach (using ternary operator)

function find_minimum(num1, num2, num3):
    min_number = (num1 <= num2 && num1 <= num3) ? num1 :
                  (num2 <= num1 && num2 <= num3) ? num2 :
                  num3
    return min_number

a more concise way:
int find_minimum(int num1, int num2, int num3) {
    return (num1 < num2) ? ((num1 < num3) ? num1 : num3) : ((num2 < num3) ? num2 : num3);
}

Steps:
1. Set min_number to num1 if num1 is less than or equal to both num2 and num3; otherwise:
2. If num2 is less than or equal to both num1 and num3, set min_number to num2; otherwise:
3. Set min_number to num3.
4. return min_number

# third approach (iterating through array)

Steps:
1. make array of the numbers.
2. for each number in array
        if array[i] < minimum:
            minimum = array[i]
3. return minimum

# fourth approach (sort in ascending order and return the number at index 0)

Steps:
1. create numbers array of length 3
2. use sort function: sort(numbers, numbers + 3)
3. return minimum number which is numbers[0]

# fifth approach (use min function)

Steps:
1. return min(num1, min(num2, num3))
