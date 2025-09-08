# Ex.No4
## Ex.Name: Write a C++ program to overload a function to print Integer data in one and Floating-Point data in another
## Date:

## Aim:
To demonstrate constructor overloading by performing addition of two and three numbers.

## Algorithm:
1. Start the program.  
2. Create a class `Addition` with constructors overloaded.  
3. Constructor with 2 parameters adds two numbers and displays sum.  
4. Constructor with 3 parameters adds three numbers and displays sum.  
5. In `main()`, create objects with two and three values.  
6. End the program.  

## Program:
```cpp
#include <iostream>
using namespace std;
class stu
{
    public:
    int n1;
    float n2;
    void read(){
        cin >>n1>>n2;
    }
    void out(){
        cout<<"Integer="<<n1<<endl;
        cout<<"Floating Point="<<n2<<endl;
    }
};
int main()
{
    stu obj;
    obj.read();
    obj.out();
}
```

## Output:
<img width="669" height="452" alt="image" src="https://github.com/user-attachments/assets/2693018f-f821-4e18-a4f4-e8d0406d8cfd" />

## Result:
```
Input: 90 99.98
Output: Integer=90 Floating Point=99.98
```
