# Ex.No2
## Ex.Name: Write a C++ program to allocate memory dynamically for a long integer variable.
## Date:

## Aim:
To demonstrate dynamic memory allocation for a long integer using `new`.

## Algorithm:
1. Start the program.  
2. Declare a pointer to a long integer.  
3. Allocate memory dynamically using `new long`.  
4. Read value from user and store in allocated memory.  
5. Display the stored value.  
6. Delete the allocated memory.  
7. End the program.  

## Program:
```cpp
#include <iostream>
using namespace std;

int main() {
    long *p_var = new long;
    long val;
    while (cin >> val) {
        *p_var = val;
        cout << "Long Value is : " << *p_var << endl;
    }
    delete p_var;
    return 0;
}
```

## Output:
<img width="1191" height="321" alt="image" src="https://github.com/user-attachments/assets/a6870834-a333-40aa-bb9a-a04f0e717da7" />

## Result:
```
10
Long Value is : 10
20
Long Value is : 20
```
