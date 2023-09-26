# first approach

1. for i = 1; i <= n; i=i+2
    cout<< i

# second approach

1. for i = 1; i <=n; i++
    if(i&1){
        cout<<i;
    }

# third recursive approach

1. function print_odd_numbers(start, n):
     if start > n: 
         return
     
     if start&1:
         print start
     
     print_odd_numbers(start + 1, n)

