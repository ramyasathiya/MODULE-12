## Ex.No:3
## Ex.Name: Binary Search Module
## Date: 10/11/25
## Aim:
To write a C++ program to implement the Binary Search Algorithm to find whether an element is present in a sorted array and return its position.

## Algorithm:
Start the program.

Input the number of elements n and the array elements (sorted in ascending order).

Input the element key to be searched.

Initialize two variables:
low = 0 (first index)
high = n-1 (last index).

Repeat while low <= high:
Find mid = (low + high) / 2.
If arr[mid] == key, return the position.
If arr[mid] > key, set high = mid - 1.
If arr[mid] < key, set low = mid + 1.
If the element is not found, print "Element Not Found".

Stop the program.

## Program:
```
int BS(int a[], int n, int search)
{
    int beg=0, end=n, mid;
    
    while(beg <= end)
    {
        mid = (beg+end)/2;
        if(a[mid]==search)
        {
            cout<<"Element found at "<<mid+1<<" position";
            return 1;
            break;
        }
        else if(a[mid] > search)
            end = mid-1;
        else
            beg = mid+1;
    }
    return 0;
}
```
## Output:

<img width="863" height="533" alt="image" src="https://github.com/user-attachments/assets/5d0feebe-222d-4f9c-8e38-62df04fa3831" />


## Result:
The Program Executed Successfully.
