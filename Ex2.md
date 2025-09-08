# Ex.No:2
# Ex.Name:Write A CPP Program to create class RectangleBox and calculate the volume of the rectangleBoxe use of static member variable in the class RectangleBox.
## Date: 08.09.2025
## Experiment No : 1 To write a C++ program to create a class RectangleBox and calculate the volume of the rectangle box using a static member variable to count the number of objects created.
## Aim:
To write a C++ program to create a class RectangleBox and calculate the volume of the rectangle box using a static member variable to count the number of objects created.

## Algorithm:
Start the program and define a class RectangleBox with private data members: length, breadth, and height.

Declare a static data member count to keep track of the number of objects created.

Define a constructor to initialize dimensions and increment the count variable.

Define a member function Volume() to calculate and return the volume (length * breadth * height).

In main(), read input values, create objects of RectangleBox, and display their volumes.

Finally, display the total number of objects created using the static variable, then stop the program.

## Program:
```
#include <iostream>
using namespace std;
class Sum
{
  public:
  int a,b,c;
  void two(int a,int b)
  {
      cout<<"Sum of two Numbers="<<a+b<<endl;
  }
  void three(int a,int b,int c)
  {
      cout<<"Sum of three Numbers="<<a+b+c<<endl;
  }
};
int main()
{
    Sum obj;
    int a,b,c;
    cin>>a>>b;
    obj.two(a,b);
    cin>>a>>b>>c;
    obj.three(a,b,c);
}
```
## Output:
<img width="1186" height="351" alt="image" src="https://github.com/user-attachments/assets/00604b2d-a478-4181-83a1-2b88278767d0" />


## Result:
The program was successfully executed. The volume of the rectangle box was calculated, and the total number of objects created was displayed using a static member variable.

## Experiment No: 2. Write a CPP Program to overload the Operator (++) i.e. on invoking it the incrementation should happen by some random value.
## Aim:
To write a C++ program that demonstrates operator overloading by overloading the increment operator (++) so that, when invoked, it performs a custom operation (in this case, summing two numbers and displaying the result).
## Algorithm:
Start the program and create a class sum with data members a, b, and res.

Overload the increment operator by defining operator++() inside the class.

Read two integer values and perform their addition.

Display the result inside the overloaded operator function.

In main(), create an object, read values, and invoke the overloaded operator using ++obj;.

Display the computed result and stop the program.
## Program:
```
#include <iostream>
using namespace std;
class sum
{
    public:
    int res,a,b;
    void operator ++()
    {
        cin>>a>>b;
        res=a+b;
        cout<<res;
    }
    
};
int main()
{
    sum obj;
    cin>>obj.a>>obj.b;
    ++obj;
    
}
```
## Output:
<img width="1178" height="400" alt="image" src="https://github.com/user-attachments/assets/671812ce-2cb5-49f4-81a9-f255efdd9bf6" />

## Result:
The program was successfully executed. The increment operator (++) was overloaded, and on invoking it, the addition of two numbers was performed and displayed.

## Experiment No: 3. Write A CPP Program to create class Rectangle and calculate the volume of the rectangle, make use of static member variable in the class Rectangle.

## Aim:
To write a C++ program to create a class Rectangle and calculate the volume of the rectangle using a member function.
Additionally, to demonstrate the use of a static data member to count the total number of objects created from the class.
## Algorithm:
Start the program and define a class Rectangle with private data members: length, breadth, and height.

Declare a static integer variable count inside the class to track the number of objects created.

Define a constructor to initialize dimensions and increment the count variable.

Define a member function Volume() to calculate and return length * breadth * height.

In main(), read input values, create Rectangle objects, and display their volumes.

Finally, display the total number of objects created using the static variable and stop the program.
## Program:
```
#include <iostream>
 
using namespace std;

class Rectangle {
    public:
    static int count;
   
      
      // Constructor definition
      Rectangle(double l,double b,double h) 
      {
          length=l;
          breadth=b;
          height=h;
          cout<<"Constructor called.\n";
          count++;
         
      }
      double Volume() 
      {
          return length*breadth*height;
        
      }
      
   private:
      double length;     // Length of a box
      double breadth;    // Breadth of a box
      double height;     // Height of a box
};
int Rectangle::count=0;

int main(void) 
{
    double l,b,h;
    cin>>l>>b>>h;
    Rectangle obj(l,b,h);
    cout<<"Volume :"<<obj.Volume()<<endl;
    cin>>l>>b>>h;
    Rectangle obj1(l,b,h);
    cout<<"Volume :"<<obj1.Volume()<<endl;
    cout<<"Total objects: "<<Rectangle::count;
    
  
   return 0;
}

```
## Output:
<img width="1173" height="489" alt="image" src="https://github.com/user-attachments/assets/f3e65513-b780-44ed-bd7f-09539ad82721" />

## Result:
The program was successfully executed.
It calculated the volume of each rectangle object and displayed the total number of objects created using a static member variable.

## Experiment No: 4. Write a C++ program to read the customer details using the constructor and display them using a member function.
## Aim:
To write a C++ program to read the customer details using a constructor and display them using a member function.
## Algorithm:
Start the program and define a class Details with data members: name, place, and no (pin code).

Define a constructor to initialize the data members with user-provided values.

Define a member function Display() to print the customer details.

In main(), read customer details (name, place, pin code) from the user.

Create an object of Details and pass the values to the constructor.

Call Display() to show the details, then stop the program.
## Program:
```
#include <iostream>
using namespace std;
class Details
{
  public:
  string name,place;
  int no;
  
  void Display()
  {
      cin>>name;
    cin>>place;
    
      cin>>no;
      cout<<"Customer name is "<<name<<endl<<"Customer city is "<<place<<endl<<"Pin code is "<<no;
      
  }
  
};
int main()
{   
    Details obj;
    obj.Display(); 
}

```
## Output:
<img width="1188" height="467" alt="image" src="https://github.com/user-attachments/assets/4e73082f-d437-41e7-93cf-01f8877dbf5c" />

## Result:
The program was successfully executed.
It accepted customer details using the constructor and displayed them using a member function.

## Experiment No: 5. Write A CPP Program to allocate memory dynamically for an long integer variable. (Note: p_var = new typename;)
## Aim:
To write a C++ program to allocate memory dynamically for a long integer variable using the new operator.
## Algorithm:
Start the program.

Declare a pointer variable of type long.

Use the new operator to dynamically allocate memory for the long integer (p_var = new long;).

Read a value from the user and store it in the allocated memory location.

Display the stored value using the pointer.

Release the memory using the delete operator (good practice).

End the program.
## Program:
```
#include <iostream>
using namespace std; 
class var_space
{
  public:
  double *p_var=new double;
     
     
  void allocateSpace()
  {
      cin>>*p_var;
      cout<<"Long Value is : "<<*p_var;
    
  }
};
int main()
{
    var_space obj;
    obj.allocateSpace();
  
    
}
```
## Output:
<img width="1168" height="292" alt="image" src="https://github.com/user-attachments/assets/2199cf85-7035-46d2-9b3f-cfcfc15a8055" />



## Result:
The program was successfully executed.
It demonstrated dynamic memory allocation for a long integer variable using the new operator and displayed the entered value.


