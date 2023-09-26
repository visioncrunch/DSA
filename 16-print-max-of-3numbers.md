# first approach

1. read all inputs: a, b, c
2. initialize a variable called maximum with INT_MAX of header limits.h
3. if a > maximum set maximum = a
4. do step 3 for b and c too
5. return maximum

# second approach (using ternary operator)

function find_maximum(num1, num2, num3):
    max_number = (num1 >= num2 && num1 >= num3) ? num1 :
                  (num2 >= num1 && num2 >= num3) ? num2 :
                  num3
    return max_number

a more concise way:
int find_maximum(int num1, int num2, int num3) {
    return (num1 > num2) ? ((num1 > num3) ? num1 : num3) : ((num2 > num3) ? num2 : num3);
}
if num1 > num2 then if num1 > num3 answer is num1 else num3
if num1 < num2 then if num2 > num2 answer is num2 else num3

Steps:
1. Set max_number to num1 if num1 is more than or equal to both num2 and num3; otherwise:
2. If num2 is more than or equal to both num1 and num3, set max_number to num2; otherwise:
3. Set max_number to num3.
4. return max_number

# third approach (iterating through array)

Steps:
1. make array of the numbers.
2. for each number in array
        if array[i] > maximum:
            maximum = array[i]
3. return maximum

# fourth approach (sort in ascending order and return the number at index 3-1)

Steps:
1. create numbers array of length 3
2. use sort function: sort(numbers, numbers + 3)
3. return maximum number which is numbers[2]

# fifth approach (use max function)

Steps:
1. return max(num1, max(num2, num3))
