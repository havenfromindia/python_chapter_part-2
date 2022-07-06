# python_chapter_part-2
A continuation for the earlier repository python chapter

# how can you specify that a variable containing some value is an array ?
# for a list we use square brackets but for array we import it.
# 2 ways to import

import array as arr
a = arr.array('i', [1, 2, 3])
print(a)

from array import array
# here you only need to specify array & not "arr.array"

b = array('i', [34, 56])
print(b)

# how can you specify that a variable containing some value is an array ?
# for a list we use square brackets but for array we import it.

# 'i' : signed integer     2     (int)
# 'u' : Unicode character  2     (string)
# uni means 1. unicode take only 1 character

# 'I' : unsigned integer   2
# 'f' : floating point     4
# 'd' : floating point     8

from array import array
# here you only need to specify array & not "arr.array"

# using integers in an array:
b = array('i', [34, 56])
print(b)
# -------------------------------------("integer")----------------------------------------------------------------------
# converting array to list
a = array('i', [2, 3, 4])
print(a)

a_list = []

for i in a:
    a_list.append(i)
print(a_list)

# -----------------------------------("string")------------------------------------------------------------------------

# using string in an array:
# 'u' : Unicode character  2     (string)
# uni means 1. unicode take only 1 character

vowels = array('u', ['a', 'e', 'i', 'o', 'u'])
print(vowels)
# array('u', 'aeiou')
# after printing it join all the charters into one.
# --------------------------------' f vs d '---------------------("FLOAT")------------------------------

# 'f' : floating point     4
# 'd' : floating point     8
decimals = array('f', [4.5, 6.7, 3.4])
print(decimals)
# array('f', [4.5, 6.699999809265137, 3.4000000953674316])

decimals = array('d', [4.5, 6.7, 3.4])
print(decimals)
# array('d', [4.5, 6.7, 3.4])
# -----------------------------------------------------------------------------------------------------------
