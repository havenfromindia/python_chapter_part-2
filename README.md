# python_chapter_part-2
A continuation for the earlier repository python chapter

# array
# in  array all the values are same unlike list containing any value(int, str, flout)

# An array is a special variable, which can hold more than one value at a time.

# If you have a list of items (a list of car names, for example),
# storing the cars in single variables could look like this:

car1 = "Ford"
car2 = "Volvo"
car3 = "BMW"
# However, what if you want to loop through the cars and find a specific one? And what if you had not 3 cars,
# but 300?
# The solution is an array!
# An array can hold many values under a single name, and you can access the values by referring to an index number.

cars = ["Ford", "Volvo", "BMW"]
print(type(cars))

# A user can treat lists as arrays. However, user cannot constraint the type of elements stored in a list.
# If you create arrays using the array module, all elements of the array must be of the same type.

# how can you specify that a variable containing some value is an array ?
# for a list we use square brackets but for array we import it.
