# python_chapter_part-2
A continuation for the earlier repository python chapter

from numpy import *

# adding 5 to each values in an array
num = array([32, 45, 67, 89])
add = num + 5
print(array(add))
# [37 50 72 94]
# adding 2 arrays
values = array([100, 5, 22, 78])
print(num + values)
# [132  50  89 167]

# maths
print(sqrt(num))
# [5.65685425 6.70820393 8.18535277 9.43398113]
print(min(num))
print(max(num))
# 32 and 89

# ****************************************************************************************************
# COPING AN ARRAY

# 1. ALIASING
# array1 = array2
arr = num

print(num)
print(arr)
# [32 45 67 89] = [32 45 67 89]

print(id(num))
print(id(arr))
# num = arr
# 32564392 = 32564392
# Same address
# in the memory only one array exist and both point to the same memory.


# 2. SHALLOW COPY - different address
# to create different array use view
# array1 = array2.view()

arr2 = num.view()
print(arr2)
# [32 45 67 89]
print(id(arr2))
print(id(num))
# 92292264 != 36693160
# values equal with different address
# here both the arrays are dependent on each
# that is if the values of the 1st array is changed it will affect the copied array (its value also changes).

num[2] = 21
print(num)
print(arr2)
# [32 45 21 89] = [32 45 21 89]


# 3. DEEP COPY - different address and no connection
# array.copy()

# in deep copy both arrays aren't linked (except its values).
# Change in the 1st array will not affect the copied array.
# Both arrays have different address

arr3 = num.copy()
print(arr3)
print(num)
# [32 45 21 89] = [32 45 21 89]

print(id(arr3))
print(id(num))
# 92294552 != 43639976

num[0] = 12
print(num)
print(arr3)
# [12 45 21 89] != [32 45 21 89]

# *********************************************************************************************************
