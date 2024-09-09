# Data-structures
lst = ["apple","guava","mango","banana","kiwi"]

print("length of list:", len(lst))
print("first element:",lst[0])
print("last element:", lst[-1])

lst.append("papaya")
print("updated list:", lst)

lst.remove("guava")
print("updated list:",lst)

lst.sort()
print("sorted list:", lst)

lst.pop(1)
print("updated list:", lst)

lst.reverse()
print("reversed list:", lst)

print("multiplication on list:", lst*2)

lst = lst[:4]
print("sliced list:", lst)

lst.clear()
print("updated list:", lst)

def test(lst):
	result = {}
	for item in lst:
		result[item[0]] = item[1:]
	return result

students = [[1, 'Jean Castro', 'V'], [2, 'Lula Powell', 'V'], [3, 'Brian Howell', 'VI'], [4, 'Lynne Foster', 'VI'], [5, 'Zachary Simon', 'VII']]

print("\nOriginal list of lists:")
print(students)
print("\nConverted  lists to a dictionary:")
print(test(students))

# empty dictionary
my_dict = {}

# dictionary with integer keys
my_dict = {1: 'apple', 2: 'ball'}

# dictionary with mixed keys
my_dict = {'name': 'John', 1: [2, 4, 3]}

my_dict = {'name': 'Jack', 'age': 26}

# Output: Jack
print(my_dict['name'])
print(my_dict.get('age'))

# update value
my_dict['age'] = 27
print(my_dict)

# add item
my_dict['address'] = 'Downtown'
print(my_dict)

# remove particular element
my_dict.pop('age')
print(my_dict)

# access a particular element
print("Address :", my_dict.get('address'))

# remove all the elements
my_dict.clear()
print(my_dict)
