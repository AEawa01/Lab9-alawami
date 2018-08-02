1. Try using a TreeMap and a HashMap instead of MyHashMap.
a. Are the resulting word frequencies any different?
Answer:
--------
No. The resulting word frequencies remain same.


b. Is the time performance any different? If so, how would you rank the three implementations (in increasing order of time complexity)?
Answer:
--------
Performance of TreeMap is low. Because TreeMap sorts the keys, so it takes time to arrange the words in the map in sorted order.
All the methods and data structure used in the built-in HashMap are much efficient than the MyHashMap.   
So, Rank the three implementations from low to high are TreeMap, MyHashMap, HashMap


2. How are % and Math.floorMod different? Which works more reliably for computing a hash table index?
Answer:
--------
Math.floorMod has the same sign as the divisor, where as % has the same sign as the dividend.
In our case size of the hash table is positive. So, divisor is always a positive value.
So, if we use Math.floorMod then we always get positive value as index.
But, If we want to use % then the hashcode may be negative so, we get negative index value. Which is invalid.


3. What is the time complexity of MyHashMap.size(), and how could you make it much more efficient?
Answer:
--------
Time complexity of MyHashMap.size() is O(n)
Where n is the size of table.
We could make it much more efficient by keeping a private size variable and incrementing the value while inserting a key and decrementing value while deleting key from table.


4. How does this implementation compare to one where you would directly use your linked Node class from the earlier assignment? Answer briefly in terms of ease of implementation, correctness, reliability, and performance.
Answer:
--------
We are using table variable of type 2D list(ArrayList and LinkedList).
ArrayList is most efficient than LinkedList in most cases(Insert, Access).
We can also use our Node class to do same task. But, we have to first implement linked list class using Node class by adding all the methods that have already there in built-in LinkedList class.
If we use our user defined linked list for 2D list then performance may less because built-in ArrayList is most efficient than our linked list.
