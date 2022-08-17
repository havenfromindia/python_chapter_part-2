# python_chapter_part-2
A continuation for the earlier repository python chapter

from numpy import *

# in the array from numpy we don't have to mention the type code
# and an array can have values from multiple type code
arr = array([23, 45, 67, 3.4, 'let'])
print(arr)
# ['23' '45' '67' '3.4' 'let']

# while using flout
floats = array([23, 45, 67, 3.4])
print(floats)
# [23.  45.  67.   3.4]

# changing array to integer(int 32)
integer = array([2, 34, 6, 7], int)
print(integer)
# [ 2 34  6  7]

# changing array to flout
flows = array([2, 34, 6, 7], float)
print(flows)
# [ 2. 34.  6.  7.]

# converting int to str
string = array([2, 34, 6, 7], str)
print(string)
# ['2' '34' '6' '7']
# *************************************************************************************************************

# using linspace - 3 parameters - start, stop and step

lin = linspace(0, 15, 16)
# here it start from 0, go till 15 and is divided into 16 parts.
print(lin)
# [ 0.  1.  2.  3.  4.  5.  6.  7.  8.  9. 10. 11. 12. 13. 14. 15.]

no_step = linspace(0, 15)
# the step is generally taken as 15 itself.

# *************************************************************************************************************

# in arrange start and stop is mentioned + skip numbers based on the steps given

table = arange(5, 55, 5)
print(table)
# [ 5 10 15 20 25 30 35 40 45 50]

# similarly range also works the same
ray = range(5, 55, 5)
for i in ray:
    print(i, end=' ')
print()
# 5 10 15 20 25 30 35 40 45 50

# *************************************************************************************************************

strange = logspace(0, 15, 16)
print(strange)
# [1.e+00 1.e+01 1.e+02 1.e+03 1.e+04 1.e+05 1.e+06 1.e+07 1.e+08 1.e+09
#  1.e+10 1.e+11 1.e+12 1.e+13 1.e+14 1.e+15]
print('%.2f'% strange[4])
# 10000.00
# *************************************************************************************************************

# zeroes and ones
bit_0 = zeros(5)
print(bit_0)
# [0. 0. 0. 0. 0.]

bit_1 = ones(5)
print(bit_1)
# [1. 1. 1. 1. 1.]
