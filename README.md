# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```
#Developed by: Gedipudi Darshani
#RegisterNumber: 23004619
def linearsearch(array,n,k):
    for i in range(0,n):
        if(array[i]==k):
            return i
    return -1
array=eval(input())
k=eval(input())
n=len(array)
array.sort()
result = linearsearch(array,n,k)
if(result==-1):
    print(array)
    print("Element not found")
else:
    print(array)
    print("Element found at index:",result)




```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
#Developed by: Gedipudi Darshani
#RegisterNumber: 23004619
def binarySearchIter(array,k,low,high):
    while(low<=high):
        m=(low+high)//2
        if k==array[m]:
            return m
        elif k>array[m]:
            low=m+1
        else:
            high=m-1
    else:
        return -1
array=eval(input())
array.sort()
print(array)
k=eval(input())
n=len(array)
t=binarySearchIter(array,k,0,n-1)
if t==-1:
    print("Element not found")
else:
    print("Element found at index:",t)


```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
#Developed by: Gedipudi Darshani
#RegisterNumber: 23004619
def BinarySearch(arr,k,low,high):
    if low<=high:
        m=(low+high)//2
        if k==arr[m]
            return m
        elif k>arr[m]:
            low=m+1
            return BinarySearch(arr,k,low,high)
        elif k<arr[m]:
            high=m-1
            return BinarySearch(arr,k,low,high)
    else:
        return -1
array=eval(input())
array.sort()
print(array)
k=eval(input())
n=len(array)
t=BinarySearch(array,k,0,n-1)
if t==-1:
    print("Element not found")
else:
    print("Element found at index:",t)



```
## Sample Input and Output
![solution](output1.png)
![solution](output2.png)
![solution](output9.png)

## Result
Thus the linear search and binary search algorithm is implemented using python programming.