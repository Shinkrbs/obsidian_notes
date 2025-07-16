Tags: #Codingtechniques #Techniques 

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

---
# Valid Parenthesis Checker using vectors

Tags: #String #Functions  #DataStructure #Vectors

The most proper way of checking validation of strings was always with a use of a queue data structure. Surprisingly, you can also use a vector to act as a container and also a queue to validate the parenthesis.

The vector is used in a manner that it will contain the open parenthesis. This way you can push the open parenthesis to the vector while ignoring the closing parenthesis and validate proper combinations of the parenthesis. If no proper combinations are seen, you can immediately return false or even if the size of the container vector is zero you can also immediately return false. If all combinations are true, then you can continue scanning the string until the length is zero.

After the length is zero and the length of the container vector is zero then we can say that the string is valid and if the length is not zero then the string is not valid.

```cpp
bool isValid(string s)
{
	std::vector<char> container;
	for(int i = 0; i < s.length(); i++)
	{
		if(s[i] == '(' || s[i] == '[' || s[i] == '{')
			container.push_back(s[i]);
		else
		{
			if(container.empty()) return false;
			
			char lastString = container.back();
			if(s[i] == ')' && last != '(' ||
			s[i] == ']' && last != '[' ||
			s[i] == '{' && last != '}' ||)
				return false;

			container.pop_back();
		}
	}
	return container.empty();
}
```
