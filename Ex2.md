# Ex.No:2
# Ex.Name:Write A CPP Program to create class RectangleBox and calculate the volume of the rectangleBoxe use of static member variable in the class RectangleBox.
## Date: 08.09.2025
## Aim:
To write a C++ program to create a class RectangleBox and calculate the volume of the rectangle box using a static member variable to count the number of objects created.


## Algorithm:

## Step 1:
Start the program.

## Step 2:
Create a class RectangleBox with:

Private data members: length, breadth, height.

A static member variable count to keep track of the number of objects created.

A parameterized constructor to initialize dimensions and increment count.

A member function Volume() to calculate and return the volume.

## Step 3:
Define the static member variable outside the class.

## Step 4:
In the main() function:

Read the dimensions from the user.

Create RectangleBox objects by passing values to the constructor.

Display the volume of each object.

Display the total number of objects created using the static member variable.

Step 5: Stop the program.

## Program:

1.Write a CPP Program to overload a function to perform sum of two integers and sum of three integers
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
2. Write a CPP Program to overload the Operator (++) i.e. on invoking it the incrementation should happen by some random value.
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
3. Write A CPP Program to create class Rectangle and calculate the volume of the rectangle, make use of static member variable in the class Rectangle.
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
4. Write a C++ program to read the customer details using the constructor and display them using a member function.
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
5. Write A CPP Program to allocate memory dynamically for an long integer variable. (Note: p_var = new typename;)
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

<img width="1186" height="351" alt="image" src="https://github.com/user-attachments/assets/00604b2d-a478-4181-83a1-2b88278767d0" />
<img width="1178" height="400" alt="image" src="https://github.com/user-attachments/assets/671812ce-2cb5-49f4-81a9-f255efdd9bf6" />
<img width="1173" height="489" alt="image" src="https://github.com/user-attachments/assets/f3e65513-b780-44ed-bd7f-09539ad82721" />
<img width="1188" height="467" alt="image" src="https://github.com/user-attachments/assets/4e73082f-d437-41e7-93cf-01f8877dbf5c" />
<img width="1168" height="292" alt="image" src="https://github.com/user-attachments/assets/2199cf85-7035-46d2-9b3f-cfcfc15a8055" />






## Result:
Thus, the C++ program to create a class RectangleBox and calculate the volume of rectangle boxes using a static member variable was successfully executed.

