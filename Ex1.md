# Ex.No1
## Ex.Name: Write a C++ program to overload the (+) operator to add two Box objects and calculate their volume.
## Date:

## Aim:
To overload the (+) operator to add two Box objects, calculate their individual volumes, and also calculate the volume of the resulting Box.

## Algorithm:
1. Start the program.  
2. Create a class `Box` with data members length, breadth, height.  
3. Create a parameterized constructor to initialize the Box.  
4. Write a function to calculate and return the volume.  
5. Overload the (+) operator to add corresponding dimensions of two objects and return a new object.  
6. In `main()`, create two Box objects with values, calculate their volumes, and then use the overloaded operator to get a third Box.  
7. Print all volumes.  
8. End the program.  

## Program:
```cpp
#include <iostream>
using namespace std;

class Box {
    float length, breadth, height;
public:
    Box(float l=0, float b=0, float h=0) {
        length = l; breadth = b; height = h;
    }
    float volume() {
        return length * breadth * height;
    }
    Box operator+(Box &b) {
        return Box(length + b.length, breadth + b.breadth, height + b.height);
    }
};

int main() {
    float l1,b1,h1,l2,b2,h2;
    cin >> l1 >> b1 >> h1;
    cin >> l2 >> b2 >> h2;

    Box b1Obj(l1,b1,h1);
    Box b2Obj(l2,b2,h2);
    Box b3Obj = b1Obj + b2Obj;

    cout << "Volume of Box1 : " << b1Obj.volume() << endl;
    cout << "Volume of Box2 : " << b2Obj.volume() << endl;
    cout << "Volume of Box3 : " << b3Obj.volume() << endl;

    return 0;
}
```

## Output:
<img width="1179" height="489" alt="image" src="https://github.com/user-attachments/assets/f2dddd22-57d3-48e9-a2b6-624d4f705ca2" />

## Result:
```
Volume of Box1 : 210
Volume of Box2 : 24
Volume of Box3 : 729
```
