Tags: #Codingtechniques

## Collection of coding techniques found from different sources.

---
# Reversing a string using JavaScript

Tags: #String #Reverse



---

# Find index position fastest way possible

Tags: #Array #DynamicProgramming #Functions 

There can be a normal way of finding out a specific index of a number in an array just by looping throughout the array. But this can take too much time because it scans the whole array. One way of shortening this task is by scanning whether the current index number is greater than or less than the target number. If the target does not exist and the loop ends, we can just return the size of the array since the index of the target number will always be greater than the values existing inside the array.

```C
for(int i = 0; i < size; i++)
{
	if(array[i] < target)
		return i;
}
return size;
```
