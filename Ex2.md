## Ex.No:2
## Ex.Name:Write A CPP Program to create class RectangleBox and calculate the volume of the rectangleBoxe use of static member variable in the class RectangleBox.
## Aim:
To write A CPP Program to create class RectangleBox and calculate the volume of the rectangleBoxe use of static member variable in the class RectangleBox.

## Algorithm:
1.Start the program.

2.Define a class RectangleBox with private members length, breadth, height and a static member objectCount.

3.Define a constructor to initialize dimensions and increment objectCount when each object is created.

4.Define a member function Volume() to calculate and return the volume of the rectangle box.

5.Define a static function getObjectCount() to return the total number of objects created.

6.In main(), input values for two rectangle boxes and display the initial object count.

7.Create objects, calculate their volumes, display them, and finally print the total object count, then end the program.

## Program:
```
#include <iostream>
 
using namespace std;

class RectangleBox {
   public:
      int static objectCount,stacount;
      // Constructor definition
      RectangleBox(double l, double b, double h) {
         
         length = l;
         breadth = b;
         height = h;
         cout <<"Constructor called." <<endl;
         // Increase every time object is created
         objectCount++;
         stacount++;
      }
      double Volume() {
         return length * breadth * height;
      }
      
   private:
      double length;     // Length of a box
      double breadth;    // Breadth of a box
      double height;     // Height of a box
};

// Initialize static member of class Box
int RectangleBox::objectCount = 0;
int RectangleBox::stacount = 0;

int main(void) 
{
      
   int l,b,h,l1,b1,h1;
   cin>>l>>b>>h>>l1>>b1>>h1;
   cout<<"Inital Stage Count: "<<RectangleBox::stacount << endl;
   RectangleBox s1(l,b,h);    // Declare box1
   cout << "Volume :" << s1.Volume()<<endl;
   
   RectangleBox s2(l1,b1,h1);    // Declare box2
   cout << "Volume :" << s2.Volume()<<endl;
   // Print total number of objects.
   cout << "Total objects: " << RectangleBox::objectCount << endl;
   cout << "Final Stage Count: " << RectangleBox::objectCount;
   return 0;
}
```
## Output:

<img width="1250" height="628" alt="image" src="https://github.com/user-attachments/assets/a9c39ce3-e17f-4290-8cef-517c116c0cfe" />


## Result:
Hence the program is executed successfully.
