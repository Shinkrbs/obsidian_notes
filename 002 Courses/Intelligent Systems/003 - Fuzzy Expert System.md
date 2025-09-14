Tags: #FuzzyExpertSystem #ExpertSystem

## Introduction

* **Fuzzy Logic** was introduced in 1965 by ***Lofti A. Zadeh*** in his research paper **"Fuzzy Sets"**. 
* **Lofti A. Zadeh** is considered as the ***father of the Fuzzy Logic***.
* A theory of Fuzzy Sets (sets that calibrate vagueness)
* Resembles the human decision-making methodology.
* It deals with vague and imprecise information.
* It is based on degrees of truth than usual true/false or 1/0 like Boolean logic.

![[Pasted image 20250914194922.png]]

--- 
### Applications of Fuzzy Logic

1. Video Camcorder - determine best focusing and lighting when there is movement in the picture.
2. Washing Machine - adjust washing machine cycle by judging the dirt, size of the load, and type of fabric
3. Television - adjust brightness, color, and contrast of picture to please viewers.
4. Motor Control - improve accuracy and range of motion control under unexpected conditions.
5. Subway Train - increase the stable drive and enhance the stop accuracy by evaluating the passenger traffic conditions. Provide a smooth start and smooth stop.
6. Vacuum Cleaner - adjust the vacuum cleaner motor power by judging the amount of dust and dirt and the floor characteristics.
7. Hot Water Heater - adjust the heating element power according to the temperature and the quantity of water being used.
8. Helicopter Control - determine the best operation actions by judging human instructions and the flying conditions including wind speed and direction.

---
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

---
## Membership Function

![[Pasted image 20250914211856.png]]

- **μ** is the symbol used to represent the **membership function**.

---
## Representing Fuzzy Sets

![[Pasted image 20250914212738.png]]

1. Singleton (single value)
2. Triangular
3. Trapezoidal
4. Sigmoid Function
5. Z-Function
6. Bell Function Moratorium

---
## Operations of Fuzzy Sets

![[Pasted image 20250914214850.png]]

***A fuzzy set is a way to handle concepts that are not clear-cut or "crisp." Unlike a standard set where an item is either **in** the set or **out** of it (a 1 or 0), a fuzzy set allows an item to **partially belong**.***

***Equivalence (A=B)*** : Two fuzzy sets, A and B are considered identical.

***Implication (A⊆B)***: Set A is a subset of set B. This means that "being in A" implies "being in B" to at least the same degree.

***Complement (Aˉ)***: The negation or NOT operation. Represents everything that is not in set A.

***Union (A∪B)***: The OR operation. IT combines two sets to represent elements that belong to A or B, or both.

***Intersection (A∩B)***: The AND operation. It finds the common ground, representing the elements that belong to both A and B.

---
## Fuzzy Hedges

![[Pasted image 20250914225203.png]]

***A hedge is a word that modifies the meaning of a fuzzy set, much like an adverb (e.g., "very," "slightly," "somewhat") modifies an adjective in everyday language. Hedges work by mathematically changing the membership function, μA​(x), of a set, making the concept it represents either stronger or weaker.***

**Concentrators (Making things more specific)**: These hedges strengthen the meaning of a set, making the criteria for membership stricter. They do this by raising the membership value to a power **greater than 1**. This reduces all membership values (except 1 and 0), so only the elements with a very high original membership retain a significant value.

**Example:** If a temperature has a membership of 0.8 in the set "Warm," its membership in the set "**Very** Warm" would be (0.8)2=0.64. It becomes less "warm."

**Dilators (Making things less specific)**: These hedges weaken or broaden the meaning of a set, making the criteria for membership less strict. They do this by taking a root of the membership value (or raising it to a power **less than 1**). This increases most membership values, allowing more elements to be considered part of the set.

**Example:** If a car has a membership of 0.3 in the set "Fast," its membership in "**Somewhat** Fast" would be sqrt(0.3)​≈0.55. Its membership has increased.

---
## Fuzzy Rule

**Fuzzy Rules** are linguistic IF-THEN constructions that have the general form: **IF A THEN B***, where A and B are propositions containing linguistic variables.

**Types of Fuzzy Rules**:

1. **Fuzzy Mapping Rules***: provide a functional mapping between the input and the output using linguistic variables.
2. **Fuzzy Implication Rules**: describes a generalized logic implication relationship between inputs and outputs.

---
## Fuzzy Inference

It is the process within a fuzzy logic system that uses fuzzy rules to map vague or imprecise inputs (like how or slow) to fuzzy or crisp outputs, mimicking human reasoning. 

1. Fuzzyfication
2. Rule Evaluation
3. Defuzzyfication

---
