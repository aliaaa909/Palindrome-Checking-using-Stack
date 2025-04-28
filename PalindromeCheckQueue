#include <iostream>
using namespace std;

bool isPalindrome(string str) {
    char queue[20];
    int front = 0, rear = -1;
    int n = str.length();

    // Input all character to queue
    for (int i = 0; i < n; i++) {
        queue[++rear] = str[i];
    }

    // check queue from front and back
    for (int i = 0; i < n / 2; i++) {
        if (queue[front++] != str[n - 1 - i]) {
            return false;
        }
    }

    return true;
}

int main() {
    string input;
    char choice;


    do {
    system("cls");
    cout << "=============================================" << endl;
    cout << "              Palindrome Checking            " << endl;


        do {

            cout << "=============================================" << endl;
            cout << "= Please enter a string: " << endl;
            cout << "= ";
            cin >> input;

            if (input.length() == 1) {
                cout << "= Error: Input must be more than 1 character!" << endl;
            } else if (input.length() > 20) {
                cout << "= Error: Input exceeds 20 characters limit!" << endl;
            }
        } while (input.length() == 1 || input.length() > 20);

        if (isPalindrome(input)) {
            cout << "= String is a Palindrome!" << endl;
        } else {
            cout << "= String is not a Palindrome!" << endl;
        }

        cout << "= Want to check another string? (y/n): ";
        cin >> choice;


    } while (choice == 'y' || choice == 'Y');

    cout << "Thank you for using the program!" << endl;
    cout << "=============================================" << endl;

    return 0;
}
