:javascript:array:

toString() - turns an array of strings(ie names) into one contigous string.
join() - similar to toString() but with an added parameter of joining them with a character or string between(ie. join(',')adds a coma to every value in index)
concat() - combined arrays together. several arrays can be added by adding 2 or more in the parameters
splice() - remove a value in an index of array. parameter 1 is the index number and parameter 2 is the number of values to be deleted after the first parameter.
copy the original array to be splice to avoid mutation. 
slice() - takes the value of the original array from and index up to the next but not excluding the current index.
indexOf() - finds the location of the value in an array. The first from left to right
splice() - removes a specified index from and array on the first parameter. second parameter indicates how many indexes to remove starting from the index specified in the first parameter.


sort() - sorts the array in ascending order. if you want to descend the order you can chain the method by doing sort().reverse() but the drawback with this method is it's slow in terms of effeciency. you can however use a callback function in the sort method. 

sort((a, b) => {
  if(a === b) return 0;
  if(a > b) return -1;
  return 1;
})
// 0, a === b, there is no change
// -1, a sorted before b
// 1, b sorted before a

indexOf() - starts to search which index of is the first value in the parameter from index 0. returns -1(false) if it didn't find the searched value. if there are
two or more values that are the same in an array, this method would find the first instance of that searched value. You can however find the next instance of that
value by adding a second parameter. indexOf(value1, 1) 1 is the index the method would start searching. if you want to search from the last index instead of index
0, you can use the method lastIndexOf().

findIndex() useful for finding objects in an array.

includes() - checks if a value in an array exist. returns true or false.

some() -  checks if "some" value in an array is true. returns boolean
every() - checks if "every" value in an array is true. returns boolean


[javascript](javascript.md)
