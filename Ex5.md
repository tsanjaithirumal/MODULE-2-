# Ex.No5
## Ex.Name: Write a C++ program to overload a function to perform sum of two integers and sum of three integers.
## Date:

## Aim:
To demonstrate function overloading by calculating sum of two and three integers.

## Algorithm:
1. Start the program.  
2. Define two overloaded functions `sum()`, one with 2 parameters and another with 3 parameters.  
3. Each function returns the sum of its arguments.  
4. In `main()`, call both functions with appropriate arguments.  
5. Print the results.  
6. End the program.  

## Program:
```cpp
#include <iostream>
using namespace std;

int sum(int a, int b) {
    return a+b;
}
int sum(int a, int b, int c) {
    return a+b+c;
}

int main() {
    int a,b,c;
    cin >> a >> b;
    cout << "Sum of two Numbers=" << sum(a,b) << endl;
    cin >> a >> b >> c;
    cout << "Sum of three Numbers=" << sum(a,b,c) << endl;
    return 0;
}
```


## Output:
<img width="853" height="417" alt="image" src="https://github.com/user-attachments/assets/c0a0d761-ad34-4ea2-86bd-5cc4f1be1dcc" />

## Result:
```
10 20
Sum of two Numbers=30
10 20 30
Sum of three Numbers=60
```
