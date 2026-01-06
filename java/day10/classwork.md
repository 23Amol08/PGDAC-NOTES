
## demo01 - Queue
* FIFO - Queue as (String) --ArrayDeque/LinkedList
    * offer() -- add 
    * poll()  -- remove 
    * peek()  -- element 

## demo02 - Deque
#Deque<Integer> q = new ArrayDeque<>() (only add and remove ) 
* Deque as Stack
    * offerFirst()
    * pollFirst()
    * peekFirst() *
* Deque as Queue
    * offerLast()
    * pollFirst()
    * peekFirst() *
* Time complexity --> O(1) , O(1) 

## demo03 - Queue as PriorityQueue(offer,poll ,String)(Elements are retrieved as per priority -- decided by Comparable (Natural Ordering)
* Comparable
* Comparator --- StringDescComparator(Elements are retrieved as per priority -- decided by given Comparator)
* Time complexity , heap sort , O(logn) 
## demo04 - Set of Strings
  #String
* HashSet
* LinkedHashSet
* TreeSet
* for-each loop

## demo05 - Set of Books ( id , name , subject , price) 
#set.add(new Book(4, "The Alchemist", "Novel", 493.23));
set.add(new Book(1, "The Archer", "Novel", 723.53));
set.add(new Book(5, "The Fountainhead", "Novel", 652.73));
set.add(new Book(2, "Atlas Shrugged", "Novel", 872.94));
set.add(new Book(6, "Harry Potter", "Novel", 423.68));
set.add(new Book(1, "The Archer", "Novel", 723.53));
set.add(new Book(3, "Lord of Rings", "Novel", 621.53));
System.out.println("Set Size: " + set.size());

* equals() and hashCode()
* Comparable TreeSet (Natural ordering) 
* TreeSet --- BookPriceComparator (Duplicates are removed) 

## demo06 - TreeSet<String>
* print set
* first(), last()
* headSet(), tailSet(), subSet()
* higer(), lower()
* descendingIterator() (// traverse set in descending direction)


## demo07 - hashCode()
* Box class-- (set.add(new Box(1, 2, 3)); ( Set<Box> set = new HashSet<Box>( );) 

## demo08 - Maps
* HashMap --- Map<Integer,String> map = new HashMap<>();
map.put(415110, "Karad - Satara"); // returns -- null
map.put(411052, "Hinjawadi - Pune"); // returns -- null
map.put(411046, "Katraj - Pune"); // returns -- null
map.put(400027, "Byculla - Mumbai"); // returns -- null
map.put(411002, "Bajirao Rd - Pune"); // returns -- null
map.put(411037, "Marketyard - Pune"); // returns -- null
map.put(411007, "Aundh - Pune"); // returns -- null
map.put(411052, "HINJEWADI - Pune"); // when key is duplicate, value is overwritten
* size()
* put()
* get(pin) --- Scanner 
*getOrDefault() 
* map.keySet()
* map.values()
* entrySet() ( map.entrySet() ) 
* entrySet() ( en.getKey() , en.getValue() ) 

#####
map.put(100, "DAC");
getKeys(map);  // keySet() 
getValues(map); // Values(); 
getKeyValuePair(map); //entrySet();  
getValueByKey(map); //keySet();  
removeEntry(map);  // containsKey() , remove(); 

**************************


// Java 8 allows to write static methods in interface -- No need to additional helper/utility class
* Static methods
* Default methods
* interface Shape
    * calcArea()
    * calcPeri()
    * calcTotalArea()

## demo02 - Java 8 Interfaces
* interface Printable - show() //multiple interface inheritance will not lead to any ambiguity error
			       // because interfaces doesn't contain any definitions
* interface Displayable - show()
* Java 7 Interfaces - No ambiguity


* Default methods - Ambiguity 
// compiler error: duplicate show() method in FirstClass.
// if two interfaces have default method with same signature and a class is inherited from that interface,
//then it will lead to ambiguity.



* No ambiguity - After overriding method
// if two interfaces have default method with same signature and a class is inherited from that interface,
//	then it will lead to ambiguity.
// this problem can be resolved by overriding method in sub-class.



* Super class wins Super-interfaces clash! (no override) 
    * class Printable, interface Displayable
// when same signature method is inherited from a super-class
// and a super-interface, the super-class method gets precedance.
// no compiler error for ambiguity



* Method overriding above example 
// method overrriding -- method is called depending on type of object.









## demo03 - Lambda Expression
* Sort array using Comparator
    ```Java
    Employee[] arr = new Employee[] {
        new Employee(4, "B", "Clerk", "Sales", 723.44),
        new Employee(8, "X", "Manager", "Accounts", 823.23),
        new Employee(2, "P", "Clerk", "Research", 234.23),
        new Employee(9, "N", "Manger", "Sales", 252.53),
        new Employee(5, "D", "Clerk", "Accounts", 923.23),
        new Employee(1, "Q", "Analyst", "Research", 826.23),
        new Employee(7, "H", "Clerk", "Research", 845.24),
        new Employee(6, "A", "Analyst", "Research", 832.23),
        new Employee(3, "G", "Analyst", "Sales", 952.44)
    };
    ```
*EmployeeIdComparator  -- local class
*Employees sort by name ---- Anonymous Inner class (empNameComparator)
*Empolyees sort by Job : Anonymous Inner class Anonymous object 
*Empolyees sort by Job desc    // lambda is short-hand implementation of the abstract method in the functional interface
*Empolyees sort by name desc (type inference) 
*Empolyees sort by sal Asc
*Empolyees sort by sal desc  // Single abstract method -> arguments -> one-liner implementation of functional Interface 
// single liner lambda expression doesn't need curly brace
// and the result of expression is considered to be returned.

*Emps list sorted by id in desc order:

**  Arrays.asList(arr); 

* Predifined Funtional Interfaces in java (Theory)
