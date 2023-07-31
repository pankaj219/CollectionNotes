# CollectionNotes
Methods of collection
=====================
java.util.Collection:

1.boolean add(E element): Adds an element to the collection.
2.boolean remove(Object element): Removes the specified element from the collection.
3.boolean contains(Object element): Checks if the collection contains the specified element.
4.int size(): Returns the number of elements in the collection.
5.boolean isEmpty(): Checks if the collection is empty.
6.Iterator<E> iterator(): Returns an iterator to iterate through the elements of the collection.

java.util.List (extends Collection):
===================================

1.E get(int index): Returns the element at the specified index.
2.E set(int index, E element): Replaces the element at the specified index with the specified element.
3.void add(int index, E element): Inserts the specified element at the specified index.
4.E remove(int index): Removes the element at the specified index.
5.int indexOf(Object element): Returns the index of the first occurrence of the specified element.
6.int lastIndexOf(Object element): Returns the index of the last occurrence of the specified element.

java.util.Set (extends Collection):
==================================

Since Set is a collection of unique elements, it inherits most methods from Collection without adding new ones. The primary difference is that the add() method returns false if the element is already present in the set (as it does not allow duplicates).

java.util.Map:
==============

1.V put(K key, V value): Associates the specified value with the specified key in the map.
2.V get(Object key): Returns the value associated with the specified key.
3.V remove(Object key): Removes the mapping for the specified key from the map.
4.boolean containsKey(Object key): Checks if the map contains the specified key.
5.boolean containsValue(Object value): Checks if the map contains the specified value.
6.int size(): Returns the number of key-value mappings in the map.
7.boolean isEmpty(): Checks if the map is empty.
8.Set<K> keySet(): Returns a set of all keys in the map.
9.Collection<V> values(): Returns a collection of all values in the map.
10.Set<Map.Entry<K, V>> entrySet(): Returns a set of key-value pairs (entries) in the map.


List has 3 Classes
==================
1) Arraylist
2) LinkedList
3) Vector

ArrayList
=========
It is made up by the implementation of List.
1) It has maintained the insertion order.
2) It has a Fixed size of 10 beyond the fixed size it increases the size by 50%.....means it gets 15 capacity to store the number and vice-versa.

 Syntax
 ======
 List<String> list=new ArrayList<String>();
 
LinkedList
==========
It is made up of the implementation of List and Deque(Double ended Queue)
====================================================================

1) It is empty by default.
2) It creates a node(in Java every node has an object) to keep elements linked.
3) It has a list method as well as a deque method...Like - add, remove from both ends.

Syntax
======
LinkedList<String> list=new LinkedList<String>();
