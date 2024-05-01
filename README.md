# cAlgorithm

### 알고리즘 문제 해결을 위한 C++

1. Fast I/O
   ```c++
   cout << "hello" << '\n';
   ```
2. STL
   ```c++
   // Container vector
   #include <vector>
   vector<type> name;

   // Container stack
   #include <stack>
   stack<type> name;

   // Container queue
   #include <queue>
   queue<type> name;

   // Container pair
   #include <utility name>
   pair<type, type> name;

   // Container map
   #include <map>
   map<type, type> name;

   // Container set
   #include <set>
   set<type> name;
   ```
3. Iterator
   ```c++
   // Iterator ex
   #include "pch.h"
   #include <iostream>
   #include <vector>

   using namespace std;
   int main(void)
   {
   vector<int> v;
   for (int i = 0; i < 7; i++) {
   v.push_back(10 * i);
   }

   vector<int>::iterator iter;
   iter = v.begin();

   cout << &iter << endl;
   cout << *iter << endl;
   cout << iter[1] << endl;

   iter += 2; // += 연산 사용
   cout << &iter << endl;
   cout << *iter << endl;

   for (iter = v.begin(); iter != v.end(); iter++) {
   cout << *iter << endl;
   }

   return 0;
   }
   ```
4. Algorithm
   ```c++
   # include <stdio.h>
   # define MAX_SIZE 5
    
   // Bubble sort
   void bubble_sort(int list[], int n){
     int i, j, temp;
   
     for(i=n-1; i>0; i--){
       for(j=0; j<i; j++){
         if(list[j]<list[j+1]){
           temp = list[j];
           list[j] = list[j+1];
           list[j+1] = temp;
         }
       }
     }
   }
   
   void main() {
     int i;
     int n = MAX_SIZE;
     int list[n] = {7, 4, 5, 1, 3};
   
     bubble_sort(list, n);
   
     for(i=0; i<n; i++){
       printf("%d\n", list[i]);
     }
   }
   ```
