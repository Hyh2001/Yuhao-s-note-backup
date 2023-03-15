

## creating

	np.array(data,dtype=)
Data can be any sequence like objects, data also can have multiple dimensions

	np.zeros([number,number])
To create arrays with zeros

	np.empty([number,number])
To create arrays with uninitialized value

	np.arange(start,stop,step)
to create array with number start from 0 to range-1

	np.random.rand(m,n)
Random values in a given shape

## monitoring of arrays

	array.ndim
to show the dimension

	array.shape
to show the shape(m and n)

	array.dtype
to show the data type of the array

## data type conversion

	array.astype(np.int32) #np.int32 can be any data types

## calculation of arrays

### array *  array

each number in the array = number * number

### array - array

each number in the array = number - number

### 1/array

each number in the array = 1/number

### array ** number

each number in the array = number ** number

### matrix multiplication

	np.dot(array.T,array)

## indexing and slicing

### copy

	x = array[x1:x2:n]
data is not copied and if you want to change something of the arrays based on the original one, you will change the original array

### indexing

	array[x][y][z] or array[x,y,z]

#### Boolean indexing

Boolean indexing will always copy array

	array[array == value]
will return the value where the equation is true

	array[-(array == value)]
will return the value where the equation is false

#### fancy indexing

pass a list or a ndarry of integers to get desired rows and desired order. when passing multiple ndarry, you will get the corresponding single number in the place of (x1,y1)....
will always copy data

	array[x1,x2,...]

### transpose

	array.T

### swapping

Interchange two axes of an array. Used for higher dimension data

	array.swapaxes(x1,x2)
