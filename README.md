# python_chapter_part-2
A continuation for the earlier repository python chapter

from array import array

# create an array with 5 values and delete the values at index number 2

# array = arr
# length = long
# deleted index number = non

arr = array('i', [])
long = int(input('enter the length of the array : '))

# creating an array
for i in range(long):
    values = int(input('enter the values : '))
    arr.append(values)
print(arr)

# deleting values
non = int(input('enter the index no of the value to delete : '))
arr.pop(non)
print(arr)

# write a code to reverse an array without using an in build function

# creating the array
count = array('i', [])
spare = array('i', [])

length = int(input('enter the length of the array : '))
for i in range(length):
    materials = int(input('enter the values : '))
    count.append(materials)
print(count)

# reversing the array
j = length
j = j - 1
for i in count:
    spare.append(count[j])
    j = j - 1
print(spare)


# ********************************************************NEW PROJECT******************************************************************************

from numpy import array

num = array([22, 45, 78, 12, 5])
values = array([67, 34, 89, 10, 3])

print(num + values)
# [ 89  79 167  22   8]

# write a code to add 2 arrays using for loop
j = 0
sum = []
for i in num:
    e = i + values[j]
    sum.append(e)
    j = j + 1

print(sum)

# write a code to find the maximum value from an array without an in build function

maxn = num[0]
# num = array([22, 45, 78, 12, 5])
for i in num:
    if i > maxn:
        maxn = i

print('max = ', maxn)

