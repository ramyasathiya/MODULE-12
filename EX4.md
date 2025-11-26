## Ex.No:4
## Ex.Name: Quick Sort – printArray Module
## Date: 10/11/25
## Aim:
To write a C++ program to implement Quick Sort and include a module to print the array before and after sorting.

## Algorithm:
Start the program.

Input the size n and elements of the array.

Define a function partition(arr, low, high) that:
Selects the pivot element.
Places all smaller elements to the left of the pivot and larger elements to the right.
Returns the pivot index.

Define a recursive function quickSort(arr, low, high) that:
Calls partition().
Recursively sorts the left and right subarrays.
Define a function printArray(arr, n) to print the array elements.

In main():
Print the array before sorting.
Call quickSort().
Print the array after sorting.

Stop the program.

## Program:
```
void printArray(int array[], int size){
    for(int i=0;i<size;i++){
        cout<<array[i]<<" ";
    }
    cout<<endl;
}
```
## Output:
<img width="868" height="467" alt="481643992-706050d0-dbbb-46b8-b2e9-781db13ca168" src="https://github.com/user-attachments/assets/b8056381-2888-4bd6-8b82-e123a4f6f6f7" />



## Result:
The Program Executed Successfully.
