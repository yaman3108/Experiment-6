# Experiment 6



## Aim:
To study and implement C++ decision making statements Loops.


## Apparatus:
Vs Code, Github


## Theory:
Loops in C++ are programming constructs that allow for a certain block of code to be repeated as many times as needed. Depending on the type of loop the number of itterations of the loop can either be predetermined. Loops usually run until certain conditions are met. Different types of loops allow for different types of operations examples of such are:

### For loop:
A for loop statement allows for a block of code to be excecuted repeatedly based on the condition. It is commonly used over a range of values for example, finding out the number of elemtents in an array. 

### While loop:
The while loop runs the code repeatedly until the given condition is proven false.

### Do while loop:
The key difference between a while loop and a do while loop is that in a do while loop the code is run atleast once even if the condition is false. This is because the condition is checked after the code is run.

### Nested for loop: 
This is a for loop inside of a for loop, useful when working with multidimensional data such as matrices.

### Nested while loop:
A nested while loop similar to a nested for loop is a while loop inside of another while loop. 

### Nested do while loop:
This is useful for scenarios where you need to ensure that the inner loop executes at least once for each iteration of the outer loop.

## Explanation: 
This program covers the basic loop statements in C++ For loop, While loop, Do while loop, Nested for loop, Nested while loop, Nested do while loop.


## Code:
```
#include <iostream>
using namespace std;

//Name: Yaman Hasan Ansari PRN:23070123155
int main()
{
    // for loop
    int i=0;
    for(i=0;i<=10;i++){
        cout<<i<<endl;
    }
    cout<<endl;
    cout<<endl;

    // while loop
    int a = 10;
    while(a>0)
    {
        cout<<a<<endl;
        a--;
    }
    cout<<endl;
    cout<<endl;

    // do-while loop
    int b = 0; 
    do {
        cout<<b<<endl;
        b+=2;
    } 
    while (b <= 10);

    cout<<endl;
    cout<<endl;

    //nested for loop
    int set = 3;
    for(int b = 1;b<=set;b++){
        for(int c = 1;c<=set;c++){
            cout<<b*c<<"\t";
        }
        cout<<endl;
    }
    cout<<endl;
    cout<<endl;

    // nested while loop
    int ROWS = 5; 

    int d = 0;
    while (d < ROWS) {
        int e = 0;
        while (e <= d) {
            cout << "* ";
            e++;
        }
        cout << endl;
        d++;
    }
    cout<<endl;
    cout<<endl;

    // nested for-while loop
    int rows = 10; 
    for (int i = rows; i >= 1; i--) {
        int j = 1;
        while (j <= i) {
            cout << j << " " ;
            j++;
        }
        cout<<endl;
        
    }
    cout<<endl;

    //nested do-while
    int rowred = 1;
    do {
        int cols = 1;
        do {
            cout << "* ";
            cols++;
        } 
        while (cols <= 5); 
        
        cout <<endl; 
        rowred++;
    } while (rowred <= 3); 

    return 0;
}

```
### Output:
![Screenshot 2024-08-06 093952](https://github.com/user-attachments/assets/cc0b7b1f-99ca-4932-827d-6fea745c72d6)
![Screenshot 2024-08-06 094002](https://github.com/user-attachments/assets/653b971d-3beb-45cd-9d27-e3a3953bddfd)


## Conclusion:
In this program we learned the working and uses of different types of loops in C++. We also learnt how to work with multi dimensional data using nested loops.
