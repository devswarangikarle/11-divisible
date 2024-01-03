# 11-divisible
#include <iostream>
using namespace std;

int main() {
    string inputNumber;
    
   
    
    cin >> inputNumber;

 
    int remainder = 0;
    for (char digit : inputNumber) {
        int currentDigit = digit - '0';
        remainder = (remainder * 10 + currentDigit) % 11;
    }

    cout  << remainder << endl;

    return 0;
}
