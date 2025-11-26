## Ex.No:5
## Ex.Name: Merge Sort – merge Module
## Date: 10/11/25
## Aim:
To write a C++ program to implement Merge Sort and include a module to merge subarrays and print the array before and after sorting.

## Algorithm:
Start the program.

Input the size n and elements of the array.

Define a function merge(arr, l, m, r) that:
Creates two temporary subarrays.
Merges them back into the original array in sorted order.

Define a recursive function mergeSort(arr, l, r) that:
Divides the array into two halves.
Calls itself for each half.
Calls merge() to combine them.
Define a function printArray(arr, n) to print the elements.

In main():
Print the array before sorting.
Call mergeSort().
Print the array after sorting.

Stop the program.

## Program:
```
void merge(int arr[], int l, int m, int r)
{
    int i,j,k;
    int n1=m-l+1;
    int n2=r-m;
    
    int L[n1],R[n2];
    for(i=0; i<n1; i++)
        L[i]=arr[l+i];
    for(j=0; j<n2; j++)
        R[j]=arr[m+1+j];
    
    i=0;
    j=0;
    k=l;
    while(i<n1 && j<n2)
    {
        if(L[i]<=R[j])
        {
            arr[k]=L[i];
            i++;
        }
        else
        {
            arr[k]=R[j];
            j++;
        }
        k++;
    }
    while(i<n1)
    {
        arr[k]=L[i];
        i++;
        k++;
    }
    while(j<n2)
    {
        arr[k]=R[j];
        j++;
        k++;
    }
}
```
## Output:
<img width="873" height="454" alt="481644567-70fd1c12-b20b-46e3-8e73-b433f30666c3" src="https://github.com/user-attachments/assets/32da0faa-74bb-4642-abc9-d7734084f989" />


## Result:
The Program Executed Successfully.
