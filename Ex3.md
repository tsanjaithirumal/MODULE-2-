
# Ex.No3
## Ex.Name: Write a C++ program to calculate the volume of a Box using static member variable.
## Date:

## Aim:
To calculate the volume of multiple Box objects and count the number of objects using a static member variable.

## Algorithm:
1. Start the program.  
2. Define a class `Box` with members length, breadth, height, and a static counter.  
3. Initialize counter as 0.  
4. In the constructor, increment counter and display a message.  
5. Define a function to calculate and print volume.  
6. Display total objects created using the static variable.  
7. End the program.  

## Program:
```cpp
#include <iostream>
using namespace std;

class Box {
    int l,b,h;
    static int count;
public:
    Box(int x,int y,int z) {
        l=x; b=y; h=z;
        count++;
        cout << "Constructor called." << endl;
    }
    void volume() {
        cout << "Volume :" << l*b*h << endl;
    }
    static void displayCount() {
        cout << "Total objects: " << count << endl;
    }
};
int Box::count=0;

int main() {
    int l1,b1,h1,l2,b2,h2;
    cin >> l1 >> b1 >> h1;
    cin >> l2 >> b2 >> h2;
    Box b1Obj(l1,b1,h1);
    b1Obj.volume();
    Box b2Obj(l2,b2,h2);
    b2Obj.volume();
    Box::displayCount();
    return 0;
}
```

## Output:
<img width="860" height="511" alt="image" src="https://github.com/user-attachments/assets/b8f55323-3254-4ebe-9aea-135ab91a58ab" />

## Result:
```
Constructor called.
Volume :24
Constructor called.
Volume :210
Total objects: 2
```
