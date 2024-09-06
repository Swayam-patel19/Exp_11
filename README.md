# Exp_11
# Aim
To study and implement Classes and Objects.

# Theory 
Class -> A class is a usser-defined data type, which holds its own data members and member functions, which can be accessed and used by creating an instance of that class.

Object-> When a class is defined, only the specification for the object is defined, no memory or storage is allocated. To use the data and access functions defined in the clss, we need to create objects.

In C++, there are three access specifiers that are:
(1) Public: Members declared as public can be accessed from outside the class.
(2) Private: Members declared as private can only be accessed within the class itself.

(3) Protected: Members declared as protected cn be accessed within the class and by derived classes.

# Code

(A)
```
# include<iostream>
using namespace std;
class cuboid
{
    public:
    double h = 2.0;
    double b = 3.0;
    double l = 4.0;
};
int main()
{
  cuboid c1;
  double vol = c1.h * c1.b * c1.l;
  cout<<"Volume "<<vol<<endl;
}
```
(B)
```
# include<iostream>
using namespace std;
class cuboid
{
    public:
    double h = 2.0,b = 3.0,l = 4.0;
    double volume()
    {
        double vol = h * b * l;
        cout<<"Volume "<<vol<<endl;
    }

};
int main()
{
    cuboid c1;
    c1.volume();
  
}
```
(C)
```
# include<iostream>
using namespace std;
class cuboid
{
    private:
    double h = 3.0,b = 2.0,l = 4.0;
    public:
    double volume()
    {
        double vol;
        vol = h * b * l;
        cout<<"Volume "<<vol<<endl;
    }

};
int main()
{
    cuboid c1;
    c1.volume();
  
}
```
(D)
```
# include<iostream>
using namespace std;
class cuboid
{
    private:
    double h = 2.0,b = 3.0,l = 4.0;
    public:
    double volume()
    {
        double vol;
        vol = h * b * l;
        return vol;
    }

    void disp(double vol)
    {
        cout<<"Volume "<<vol<<endl;

    }

};
int main()
{
    cuboid c1;
    double v = c1.volume();
    c1.disp(v);
  
}
```
(E)
```
# include<iostream>
using namespace std;
class cuboid
{
    public:
    double h,b,l;
    void input()
    {
        cout<<"Enter the length: ";
        cin>>l;
        cout<<"Enter the breadth: ";
        cin>>b;
        cout<<"Enter the height: ";
        cin>>h;
    }
    double volume()
    {
        double vol;
        vol = h * b * l;
        return vol;
    }

    void disp(double vol)
    {
        cout<<"Volume "<<vol<<endl;

    }

};
int main()
{
    cuboid c1;
    c1.input();
    double v = c1.volume();
    c1.disp(v);
  
}
```

# Output 

(A)

<img width="916" alt="Screenshot 2024-09-06 at 11 57 42" src="https://github.com/user-attachments/assets/da2b1e87-22b3-4be7-b336-f3e27d127d8b">

(B)

<img width="936" alt="Screenshot 2024-09-06 at 11 58 41" src="https://github.com/user-attachments/assets/9ca06c74-8485-4dab-b74a-dd59b13e759e">

(C)

<img width="712" alt="Screenshot 2024-09-06 at 11 59 05" src="https://github.com/user-attachments/assets/6f73cb5b-4bbd-4e23-b8a4-93754b894680">

(D)

<img width="943" alt="Screenshot 2024-09-06 at 11 59 30" src="https://github.com/user-attachments/assets/6eb260b4-7b28-4c6f-a99d-72164b1bb98c">

(E)

<img width="672" alt="Screenshot 2024-09-06 at 11 59 48" src="https://github.com/user-attachments/assets/ac0c8fc8-fa60-4f31-a757-7e38f0e064cc">

# Conclusion 

In this experiment, i learnt about classes and objects in C++ and performed programs using them and also learnt about local variables and global variables.


