# Python-task-
1. It belongs to second if statement(if False)

2. foo

reason: when the foo() function is called in the if statement it prints foo and return false 

once it returns false due to the and operator in the if statement, if the first condition foo 

() evaluates to False, the second condition bar () is not evaluated and as if condition 

evaluates to false the print(hello) statement is not executed

3. When we modify the loop variable i inside a for loop that iterates over a range () in 

Python, the change to i within the loop body does not affect the subsequent iterations of 

the loop.

4. tuples_list = [(1, "a"), (2, "b"), (3, "c"), (1, "d")]

target_set = {1, 3}

result_tuples = []

for i in tuples_list:

 if i[0] in target_set:

 result_tuples.append(i)

 print(result_tuples)

# Output: [(1, 'a'), (3, 'c'), (1, 'd')]

5. No, a set cannot directly contain tuples that contain mutable elements like lists. This is 

because elements in a set must be hashable, and mutable objects are not hashable in 

Python. If a tuple contains a mutable object, the tuple itself becomes unhashable, 

preventing it from being stored in a set.

To make it hashable we can convert the list into tuple

If we try to create a set with a tuple containing a mutable element python will return 

“TypeError”

6. The given loop runs infinitely due to the nature of floating-point arithmetic and how 0. 1 

is represented in binary. Therefore, the loop continues to execute because x never 

perfectly reaches the value 1.5 to terminate the loop.

7. List comprehension: squares = [i**2 for i in range(10) if i % 2 == 0]

8. Code:

l = [1, [2, [3, 4], 5], 6]

print(l[1][1][1])

9. def prime_no(List):

 prime_list=[]

 for i in List:

 if i > 1: 

 c=True

 for j in range(2,int(i**0.5)+1):

 if i % j == 0:

 c=False

 break

 if c==True:

 prime_list.append(i)

 return prime_list
 List=[2,45,6,7,11,45,9,91,47,83]

print(prime_no(List))

 10. def remove(list1):

 length = len(list1)

 if length % 2 == 1: # Odd length

 middle_index = length // 2

 del lst[middle_index]

 else: # Even length

 middle_index1 = length // 2 - 1

 middle_index2 = length // 2

 del lst[middle_index1:middle_index2+1] # Remove both middle

 return list1

 list1 = [10, 20, 30, 40, 50]

 print(remove(list1))

 list2 = [10, 20, 30, 40]

 print(remove(list2))

11.List = [5,6,7,8,9]

revList = []

 for i in range(len(List),0,-1):

 revList.append(List[i-1])

 print(revList)

12. def pallindrome(str):
13. emstr = ""

 for i in range(len(str),0,-1):

 emstr+=str[i-1]

 return emstr

str = input("enter a string:")

revstr=pallindrome(str)

if str==revstr:

 print("it is a pallindrome")

else:

 print("it is not pallindrome")

 

13. import numpy as np

 arr = np.random.randint(1, 101, size=(5, 5))

 print(arr)

 arr[arr % 2 == 0] = 0

 print("Array after replacing even numbers with 0:", arr)

14. import numpy as np

 array1 = np.random.randint(0, 10, size=(3, 3)) 

 array2 = np.random.randint(0, 10, size=(3, 3))

 print("Array 1:")

 print(array1)

 print("\nArray 2:")

 print(array2)

 equal_array = (array1 == array2)
 print("\nElement-wise equality array:")

 print(equal_array)

15. import numpy as np

 a = np.array([[45, 60], [30, 80]])

 a[a > 50] = 100

 print(“array after replacing:”)

 print(a)

 colmean = np.mean(a, axis=0)

 print("Mean of each column:")

 print(colmean)
