# Class-and-Object
This is my first OOP code

#include <iostream>
#include <string.h>
using namespace std;

class Teacher {
private:
    string name;
    double salary;
public:
    string id;
    string dpt;
    string qualification;
    // Access for private class
    void info(string Name, double Salary){
        name = Name;
        salary = Salary;

    }
    //Print for private class
    void display(){
        cout << "Name of teacher is:" <<  name << endl;
        cout << "Salary is:" << salary << endl;
    }
    void access(string id, string dpt, string qualification){
        cout << "The id of teacher is: " << id << endl;
        cout << "The department of  teacher is: " << dpt << endl;
        cout << "The qualification of teacher is: " << qualification << endl;
    }
};


int main(){
    Teacher t1;
    cout << "\t\t\t Teacher Record system" << endl;
    t1.access("B23118006035", "Space science", "Software engineer");
    t1.info("Alyan", 25000);
    t1.display();

    Teacher t2;
    t2.access("B23118006036", "Health and Education", "Physisit");
    t2.info("Rameez",30000);
    t2.display();

    return 0;
}
