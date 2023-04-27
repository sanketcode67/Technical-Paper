# Technical Paper on List Methods

### All List Methods in Python
In this technical paper see all the inbuilt list methods  and we will check how they work with the list object.

1.  `append():`  adds or appends the element at the end of the list.

		item = [10,20,30]
		items.append(40)
		print(item)
	output: `[10, 20, 30, 40]`	
3.  `clear():`  clears all the elements of the list.
		
		item = [10,20,30]
		item.clear()
		print(item)
	output: `[]`
4. `copy():`  returns a new list after copy all the elements from the list.

		item = [10,20,30]
		copy_item = item.copy()
		print(copy_item)
	output: `[10, 20, 30]`
		
5. `count():`  count returns the number of occurrences of a given element in the list

		item = [10,20,10,40]
		n = item.count(10)
		print(n)
	output: `2`
	
6. `extend():`  adds all the elements of the list or any iterable in the current list

		item = [10,20,10,40]
		more_items = {50,60}
		item.extend(more_items)
		print(item)
	output: `[10, 20, 10, 40, 50, 60]`

7. `insert():`  insert method adds element to a specific position in the list and takes an index as a input on which the elements will be inserted. 

		item = [10,20,10,40]
		item.insert(0,50)
		print(item)

	output: `[50, 10, 20, 10, 40]`

8. `pop():`  removes a element at a specific position from this list. If you doesn't specify any index by default it will be -1 means last index of the list.

		item = [10,20,10,40]
		item.pop()
		print(item)
	output: `[50,10,20,10,40]`

9. `index():`  It takes an element as an input and returns the first index of the element.

		item = [10,20,40,10,40]
		index = item.index(40)
		print(index)
    output: `2`
10. `remove():`  remove method takes an element as an input and removes the first occurrence of that element from the list.

		item = [10,20,40,10,40]
		item.remove(40)
		print(item)
	 output: `[10, 20, 10, 40]`
11. `reverse():`  reverse method simply reverses the current list.

		item = [10,20,30,40]
		item.reverse()
		print(item)
	output: `[40, 30, 20, 10]`
12. `sort():`  sort method sorts the list by ascending order.Your can also change sorting order through the parameters of the sort method.

		item = [20,40,10,50]
		item.sort()
		print(item)
	output: `[10, 20, 40, 50]`	
It takes 2 arguments
	  * reverse = True OR False ,by default reverse is False ,if you write reverse =   	 True then sorting order will be descending
			
			item = [20,40,10,50]
			item.sort(reverse = True)
			print(item)
		output: `[50,40,20,10]`
	*  key = A function to define the sorting criteria
	
			def sort_by_length(ele):
			    return len(ele)

			item = ["Sanket","Ravi","Manas","Avoy"]
			item.sort()
			print(item)
		output: `[10, 20, 40, 50]`