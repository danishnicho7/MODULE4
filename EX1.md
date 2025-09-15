# Ex.No:1
# Ex.Name: Write a CPP Program for Class conversion that can be achieved by conversion function which is done by the use of operator overloading (use character data)
## Aim:
To write a C++ program that demonstrates class conversion into a basic data type (character) using operator overloading.

## Algorithm:
1. Start the program.
2. Create a class ConvertChar with a private data member of type char.
3. Initialize the character using a constructor.
4. Overload the type-casting operator operator char() to return the stored character.
5. In main(), create an object of the class, convert it into a char using the overloaded operator, and display the result.
6. End the program.

## Program:
```cpp
#include <bits/stdc++.h>
#include <string.h>
using namespace std;
class Class_type_one 
{
   string a;
   public:
      Class_type_one()
      {
       cin>>a;
      }
      string get_string()
      {
       return (a);
      }
   void display()
   {
      cout<<a<<endl;
   }
};
class Class_type_two 
{
   string b;
   public:
   Class_type_two()
     {
        
     }
  
    Class_type_two (Class_type_one& a)
    {
       b=a.get_string();
    }
   void display()
   {
      cout<<b;
   }
};
int main()
{
  Class_type_one a1;
  Class_type_two a2;
  a2=a1;
  a1.display();
  a2.display();
   return 0;
}
```


## Output:
<img width="280" height="228" alt="image" src="https://github.com/user-attachments/assets/405410f4-fefa-45f7-ac2f-ed74b78f2617" />

## Result:
The program successfully demonstrates class-to-basic type conversion using operator overloading, where a class object is converted into a character type.
