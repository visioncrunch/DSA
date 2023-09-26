# problem 
check if a number is same after double reversal

# pseudocode
a function to reverse a number
pass the reversed number again to this function
then apply a bool that checks if initial = final

return num == reverse(reverse(num));

bool double_reverse(int num){
    int rev = 0;
    while(n>0){
        rev = rev * 10 + num%10;
        num/=10;
    }
    return num == reverse(reverse(num));
}
