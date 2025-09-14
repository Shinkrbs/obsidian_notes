Tags: #FuzzyExpertSystem #ExpertSystem

## Introduction

* **Fuzzy Logic** was introduced in 1965 by ***Lofti A. Zadeh*** in his research paper **"Fuzzy Sets"**. 
* **Lofti A. Zadeh** is considered as the ***father of the Fuzzy Logic***.
* A theory of Fuzzy Sets (sets that calibrate vagueness)
* Resembles the human decision-making methodology.
* It deals with vague and imprecise information.
* It is based on degrees of truth than usual true/false or 1/0 like Boolean logic.

![[Pasted image 20250914194922.png]]

### Applications of Fuzzy Logic

1. Video Camcorder - determine best focusing and lighting when there is movement in the picture.
2. Washing Machine - adjust washing machine cycle by judging the dirt, size of the load, and type of fabric
3. Television - adjust brightness, color, and contrast of picture to please viewers.
4. Motor Control - improve accuracy and range of motion control under unexpected conditions.
5. Subway Train - increase the stable drive and enhance the stop accuracy by evaluating the passenger traffic conditions. Provide a smooth start and smooth stop.
6. Vacuum Cleaner - adjust the vacuum cleaner motor power by judging the amount of dust and dirt and the floor characteristics.
7. Hot Water Heater - adjust the heating element power according to the temperature and the quantity of water being used.
8. Helicopter Control - determine the best operation actions by judging human instructions and the flying conditions including wind speed and direction.

## Fuzzy Sets

![[Pasted image 20250914205258.png]]

Definitions:

-  define **X** as the universal set
- Universe is the overall context or the collection of all possible things in the domain.
- **"A fuzzy set A⊂X..."**,  A is a subset of X
- **"...is characterized by a _membership function_ fA​(x):X→[0,1] which associates each point in X a real number in the interval [0,1]."** : The membership function is a **rule** that takes an item from the universe (X) and assigns it a "membership score" between 0 and 1.
- Example : The input x is a specific height (eg. 5'5 or 6'2), then the function name is fA​(x). The subscript A suggests that this function belongs to the set A (set of "tall"), so it can also be written as ftall​(x). The output is a number between 0 and 1.
- **"fA​(x) represents the grade of membership of x in A."** suggests that the output score tells how much an item belongs to the set.
- A score of 1 means the item is a full member. It completely belongs to the set.
- A score of 0 means the item is not a member at all.
- A score between 0 and 1 (like 0.3, 0.5, or 0.8) means it has **partial membership**. It "kind of" belongs.

***A fuzzy set defines a vague category by creating a function that assigns a "degree of belonging" (from 0 to 1) to every possible item.***

## Membership Function

![[Pasted image 20250914211856.png]]

- **μ** is the symbol used to represent the **membership function**.

## Representing Fuzzy Sets

![[Pasted image 20250914212738.png]]

1. Singleton (single value)
2. Triangular
3. Trapezoidal
4. Sigmoid Function
5. Z-Function
6. Bell Function Moratorium