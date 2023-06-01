# Functions
Functions assignment

a=3;b=11
li=[]
for i in range(a,b+1):
	li.append(i)
odd_num = list(filter(lambda x: (x%2!=0),li))
print(odd_num)

def myFun(**kwargs):
	for key, value in kwargs.items():
		print("%s == %s" % (key, value))


myFun(first='Data', mid='Science', last='Masters')

test_list = [1, 2, 3, 4, 5, 6, 6, 6, 6]
 
N = 5
i = 0
while True:
    print(test_list[i])
    i = i + 1
    if i == N:
        break
     
     def my_generator(n):

    value = 0

    while value < n:

        yield value

        value += 1

for value in my_generator(5):

    print(value)
    
    def prime(x, y):
	prime_list = []
	for i in range(x, y):
		if i == 0 or i == 1:
			continue
		else:
			for j in range(2, int(i/2)+1):
				if i % j == 0:
					break
			else:
				prime_list.append(i)
	return prime_list

starting_range = 2
ending_range = 20
lst = prime(starting_range, ending_range)
if len(lst) == 0:
	print("There are no prime numbers in this range")
else:
	print("The prime numbers in this range are: ", lst)


The def keyword is used to create, (or define) a function.
'args' and 'kwargs' are used in a function to pass a keyworded ,variable length argument list.
An iterator is an object that allows you to iterate over collections of data, such as lists, tuples, dictionaries, and sets.
A Python generator function allows you to declare a function that behaves like an iterator, providing a faster and easier way to create iterators.
The yield keyword will convert an expression that is specified along with it to a generator object and return it to the caller.
