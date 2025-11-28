# C++ Program: Class Staff With Menu-Driven Operations

```cpp
#include <iostream>
using namespace std;

class Staff {
private:
    int staff_id;
    string name;
    float salary;

public:
    // Function to accept staff details
    void accept() {
        cout << "\nEnter Staff ID: ";
        cin >> staff_id;

        cout << "Enter Name: ";
        cin >> name;

        cout << "Enter Salary: ";
        cin >> salary;

        cout << "Data stored successfully!\n";
    }

    // Function to display staff details
    void display() {
        cout << "\n--- Staff Details ---\n";
        cout << "Staff ID : " << staff_id << endl;
        cout << "Name     : " << name << endl;
        cout << "Salary   : " << salary << endl;
    }
};

int main() {
    Staff s;
    int choice;

    while (true) {
        cout << "\n====== MENU ======\n";
        cout << "1. Accept Staff Data\n";
        cout << "2. Display Staff Data\n";
        cout << "3. Exit\n";
        cout << "Enter your choice: ";
        cin >> choice;

        switch (choice) {
            case 1:
                s.accept();
                break;

            case 2:
                s.display();
                break;

            case 3:
                cout << "Exiting program...\n";
                return 0;

            default:
                cout << "Invalid choice! Please try again.\n";
        }
    }

    return 0;
}
```
====== MENU ======
1. Accept Staff Data
2. Display Staff Data
3. Exit
Enter your choice: 1

Enter Staff ID: 101
Enter Name: Harshal
Enter Salary: 35000
Data stored successfully!

====== MENU ======
1. Accept Staff Data
2. Display Staff Data
3. Exit
Enter your choice: 2

--- Staff Details ---
Staff ID : 101
Name     : Harshal
Salary   : 35000


