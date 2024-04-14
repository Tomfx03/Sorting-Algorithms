# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs & Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```
lst=eval(input(""))
n=int(input(""))
lst.sort()
b=len(lst)
print(lst)
for i in range(0,b):
    if (lst[i]==n):
     c=i
     print("Element found at index: ",c)
     break
else:
    print("Element not found")
#name:tom francies xaviour.L
#reg no:212223110600
```
ii)	#Insertion Sort
```
#name:tom francies xaviour.L
#reg no:212223110600
lst=eval(input(""))
n=int(input(""))
lst.sort()
b=len(lst)
print(lst)
low=lst[0]
high=lst[-1]
def binary(lst,n,low,high):
    while(low<=high):
        mid=(low+high)//2
        if n==mid:
            for i in range(0,b):
                if (lst[i]==n):
                    global c
                    c=i
                    return 1
                    break
        elif n>mid:
            low=mid+1
        else:
            high=mid-1
    return -1
find=binary(lst,n,low,high)
if(find==1):
    print("Element found at index: ",c)
elif(find==-1):
    print("Element not found")

```
iii)	#Insertion Sort(recursive Method).
```
#name:tom francies xaviour.L
#reg no:212223110600
lst=eval(input(""))
n=int(input(""))
lst.sort()
b=len(lst)
print(lst)
low=lst[0]
high=lst[-1]
def binary(lst,n,low,high):
    if low<=high:
        mid=(low+high)//2
        if n==mid:
            for i in range(0,b):
                if (lst[i]==n):
                    global c
                    c=i
                    return 1
        elif n>mid:
            low=mid+1
            return binary(lst,n,low,high)
        elif n<mid:
            high=mid-1
            return binary(lst,n,low,high)
    else:
             return -1
         
find=binary(lst,n,low,high)
if(find==1):
    print("Element found at index: ",c)
elif(find==-1):
    print("Element not found")
```
## Output:
i)	#Selection Sort:

![Screenshot 2024-04-14 132258](https://github.com/Tomfx03/Sorting-Algorithms/assets/101335832/88550395-3328-46df-821a-f2e7b3fc46aa)

ii)	#Insertion Sort:

![Screenshot 2024-04-14 132308](https://github.com/Tomfx03/Sorting-Algorithms/assets/101335832/4d19b877-7977-4e9e-8307-9b77ceac1ef5)

iii)	#Insertion Sort(recursive Method):

![Screenshot 2024-04-14 132331](https://github.com/Tomfx03/Sorting-Algorithms/assets/101335832/baf4565e-bbd2-440b-8e0a-7696ed0c1558)
## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
