initiallization, condition, process, updation

# for-loop
for(int i = 0; i < n; i++)
{
    cout << i+1;
}

# while-loop
int i = 0;
while(i < n)
{
    cout << i;
    i++;
}

# do-while-loop
int i = 0;
do
{
    cout<<i;
    i++;
}
while(i<n);

# range-based-loop

int main() {
    std::vector<int> numbers = {1, 2, 3, 4, 5};

    std::cout << "Numbers in the vector:" << std::endl;

    for (int num : numbers) {
        std::cout << num << " ";
    }

    return 0;
}