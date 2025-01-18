# Assignment-DSA
Binary Search Implementation: 
 
#include <iostream> #include <vector> using namespace std; 
 
int binarySearch(vector<int> arr, int target) {     int left = 0, right = arr.size() - 1;    
while (left <= right) {         int mid = left + (right - left) / 2;        
 if (arr[mid] == target)             return mid; // Target found         else if (arr[mid] < target)             left = mid + 1;         else             right = mid - 1; 
    }     return -1; // Target not found 
} 
 
int main() {     vector<int> arr = {2, 3, 4, 10, 40};     int target = 10; 
 
    int result = binarySearch(arr, target);     if (result != -1)         cout << "Binary Search: Target found at index " << result << endl; 
    else 
        cout << "Binary Search: Target not found." << endl; 
 
    return 0; 
} 

 
 Linear Search Implementation: 
 
 
#include <iostream> #include <vector> using namespace std; 
 
int linearSearch(vector<int> arr, int target) {     for (int i = 0; i < arr.size(); i++) {         if (arr[i] == target)             return i; // Target found 
    }     return -1; // Target not found 
} 
 
int main() {     vector<int> arr = {2, 3, 4, 10, 40};     int target = 10; 
 
    int result = linearSearch(arr, target);     if (result != -1) 
        cout << "Linear Search: Target found at index " << result << endl; 
    else         cout << "Linear Search: Target not found." << endl; 
 
    return 0; 
} 
 
 
