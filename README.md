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
