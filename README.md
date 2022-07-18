# python_chapter_part-2
A continuation for the earlier repository python chapter

# taking the values from user to create an array and searching values in it.

from array import array
arr = array('i', [])

long = int(input('enter the length of array : '))
for i in range(long):
    user = int(input('enter the values : '))
    arr.append(user)
print(arr)

l = []
for i in arr:
    l.append(i)
print('in list :', l)

# *********************************************************************************************************

# search for the value
x = 0
search = int(input('enter the value to search : '))
for i in arr:
    if i == search:
        print('found at', x)
    x = x + 1
# 2
print('found at', arr.index(search))
