#include<iostream>
using namespace std;


int main() {
    int a[100], n = 0, ch, pos, val, i, f;
    cout << "1.CREATE ,2.DISPLAY ,3.INSERT ,4.DELETE\n5.LINEAR SEARCH\n6.EXIT\n";
    cout << "Enter choice ->";
    cin >> ch;
    
    switch (ch) {
    case 1:
    cout << "Enter number of elements: ";
    cin >> n;
    cout << "Enter elements: ";
    for (i = 0; i < n; i++) cin >> a[i];
    break;
    
    case 2:
    cout << "Array elements: ";
    for (i = 0; i < n; i++) cout << a[i] << " ";
    cout << endl;
    break;
    
    case 3:
    cout << "Enter position and value to insert: ";
    cin >> pos >> val;
    for (i = n; i > pos; i--)
    a[i] = a[i - 1];
    a[pos] = val;
    n++;
    break;
    
    case 4:
    cout << "Enter position to delete: ";
    cin >> pos;
    for (i = pos; i < n - 1; i++) 
    a[i] = a[i + 1];
    n--;
    break;
    
    case 5:
    cout << "Enter value to search: ";
    cin >> val;
    for (i = 0; i < n; i++) {
    if (a[i] == val) 
    cout<<"Found";
    }
    
    case 6:
    return 0;
    
    default:
    cout << "Invalid ";
    }
    }
    
    //output - 
    /*chetanyabhargav@MacBook-Air-13 DSA LAB Assignnment 1 % cd "/Users/chetanyabhargav/Desktop/chetan
ya_coding/DSA LAB Assignnment 1/" && g++ question1.cpp -o question1 && "/Users/chetanyabhargav/D
esktop/chetanya_coding/DSA LAB Assignnment 1/"question1
1.CREATE ,2.DISPLAY ,3.INSERT ,4.DELETE
5.LINEAR SEARCH
6.EXIT
Enter choice ->1
Enter number of elements: 4
Enter elements: 1
2
3
4
chetanyabhargav@MacBook-Air-13 DSA LAB Assignnment 1 % */
