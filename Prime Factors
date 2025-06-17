#include <iostream>
using namespace std;
 
int main() {
    int N;
    cin >> N;
    
    if (N <= 1) {
        cout << "Invalid input." << endl;
        return 0;
    }
    
    int originalN = N;  
    
    bool firstFactor = true;  
    for (int i = 2; i * i <= N; i++) {
        if (N % i == 0) {
            int count = 0;
            while (N % i == 0) {
                count++;
                N = N/ i;
            }
            if (!firstFactor) {
                cout << "*";
            }
            cout << "(" << i << "^" << count << ")";
            firstFactor = false;
        }
    }
    
    if (N > 1) {
        if (!firstFactor) {
            cout << "*";
        }
        cout << "(" << N << "^" << 1 << ")";
    }
    
    return 0;
}
