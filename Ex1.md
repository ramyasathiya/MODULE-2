## Ex.No:1
## Ex.Name:Write A CPP Program to allocate memory dynamically for a double array. (Note: p_array = new type [size]; )
## Aim:
To write A CPP Program to allocate memory dynamically for a double array.(Note: p_array = new type [size]; )
## Name : Ramya S
## Register Number : 212222040130
## Algorithm:
1.Start the program.

2.Input the size of the array from the user.

3.Dynamically allocate memory for a long array using long* p_array = new long[size];

4.Display confirmation that the array has been created.

5.Read array elements from the user and store them in the allocated memory.

6.Print all stored array elements in sequence.

7.Release the allocated memory using delete[] p_array; and display confirmation, then end the program.

## Program:
```
#include <iostream>
int main() {
    int size;
    std::cin >> size;
    int* p_array = new int[size]; 
    
    std::cout << "Array Created" << std::endl;
    
    for (int i = 0; i < size; ++i) {
        std::cin >> p_array[i];
    }
    
    std::cout << "Array Values :" << std::endl;
    
    for (int i = 0; i < size; ++i) {
        std::cout << p_array[i] << " ";
    }
    std::cout << std::endl;
    delete[] p_array;  
    std::cout << "Array Deleted" << std::endl;
    return 0;
}
```
## Output:

<img width="1248" height="557" alt="image" src="https://github.com/user-attachments/assets/570e09d2-3adf-48a9-8f9a-2ba53173ebf2" />


## Result:
Hence the program is executed successfully.
