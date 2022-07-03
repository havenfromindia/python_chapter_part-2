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
