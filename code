#include <iostream>
#include <vector>
using namespace std;

int fibonacci(int n, vector <int> &ref) {
    // Base case
    if(n == 0){
        return 0;
    }
    if(n == 1 || n == 2){
        return 1;
    }
    if(ref[n] != -1){
        return ref[n];  //simply return the value if available
    }

    // Recursive case
    ref[n]= fibonacci((n-1),ref)+ fibonacci((n-2),ref);
    return ref[n];
}

//function below prints a list of fibonacci in recursive manner using memoization
void printList(int n){
// Creating a vector named 'storage' which calls the constructor that creates n+1 cells and inserts the value -1 into each cell of the vector
    vector <int> storage(n+1, -1);
  
    for(int i = 0; i<=n; i++){
        cout<< fibonacci(i,storage)<< " ";
    }

}


int main() {
    int n;
    cout << "Enter a number: ";
    cin >> n;
    printList(n);
    return 0;
}
