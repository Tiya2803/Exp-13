# Experiment 13
# Aim:
To study and implement constructor overloading.

# Theory:

Constructors are unique member functions of a class that are automatically called when an object of the class is created. When there are more than one constructor in a class with the same name is called as constructor overloading. The important point to keep in mind is that the list of arguments should be different for each of these constructors. The number of parameters acts as a differentiating factor between each of the constructors.

The use case for constructor overloading are:

→ It allows flexibility in object creation.

→ It provides different ways to set up an object based on the input data.

→ It simplifies the code readability and maintenance by managing object initialization centrally within the constructors.

→ It provides multiple ways to instantiate objects depending on the situation


# Code:

```
#include<iostream>
using namespace std;

class room
{
    private:
    double l,b;

    public:
    room()
    {
        l = 1.2;
        b = 2.3;
    }
    room(double len, double bre)
    {
        l = len;
        b = bre;
    }
    room(double len)
    {
        l = len;
        b = 4.5;
    }
    double area()
    {
        return l*b;
    }

};
int main()
{
    room r1,r2(6.7,7.8),r3(9.1);
    cout<<"No parameter passed: "<<endl;
    cout<<"Area: "<<r1.area()<<endl;
    cout<<"Two parameters passed: "<<endl;
    cout<<"Area: "<<r2.area()<<endl;
    cout<<"One parameter passed: "<<endl;
    cout<<"Area: "<<r3.area()<<endl;
}
```

# Output:

![image](https://github.com/user-attachments/assets/a2f4a3a1-2c4b-4b31-a16e-a25f1b98311b)


# Conclusion:

→ We learnt about constructor overloading in C++.

→ We learnt the use case of constructor overloading in C++.
