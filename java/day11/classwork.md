
 
*lambda expressions are referenced by functional interface reference.
*lambda arg scope is limited to lambda expression body/implementation.
*non-capturing lambda
*capturing lambda -- (are also called closure in some programming languages) 

*// capturing lambda - captures (attach) a variable out-side the lambda implementation.
// can capture variables that are final or effectively final.





## demo04 - Lambda expressions
A Stream in Java is a sequence of elements (data) that can be processed in a functional style.
It is not a data structure but a view of data from collections, arrays, or I/O channels.
## demo05 - Java Streams
		//Input : 1 , 2 , 3 , 4 , 5 , 6 , 7 , 8 , 9 , 10 
		//step1 : Square of each number : 1 , 4 , 9 , 16 , 25 , 36 , 49 , 64 , 81 , 100 
		//step2 : get all odd numbers : 1 , 9 , 25 , 49 , 81 
		//step3 : append "java" :  "java1" , "java9" , "java25" , "java49" , "java81"
		// print each element 
		
		

* Stream operations
    * filter()
    * map()
    * sorted()
    * map()
    * forEach()
* Stream execution

# demo01 - Stream/Optional
* `Stream<Double>`//Arrays.stream(); 
    * skip()
    * limit()
* `Stream<String>`//list.stream(); 
    
* `Stream<Integer>`
    * reduce() 
    
* `Stream<Integer> strm = Stream.iterate(); 
    * print table of number

* Stream of primitive values
     
## demo02 - Method references
// lambda expr = short-hand implementation of SAM (functional interface)
// method ref = short-hand of lambda expr
* static method reference // static method of a class --> ClassName.method(arg1, arg2); i.e. static method called on ClassName
* non-static method reference // non-static method of a class -- Comparator--> arg1.method(arg2); i.e. non-static method called on arg1
* object method reference //consumer<> non-static method to call on obj --> obj.method(arg); i.e. non-static method called on given object
* constructor reference// param-less constructor is called after creating object of given class.

//For every class you write in Java, the JVM automatically creates a single java.lang.Class object that represents that class.
## demo04 - Reflection


## demo03 - enum
* enum Arithmetic
* Menu driven program
* enum fields


## demo02 - Annotations
* String(value , designation , company())
* Pre-defined annotations
* Custom annotations 


## demo03 - File class ( java.io.File) 
/*
1. Input a path from user.( java.io.File) 
2. If path is invalid, print error.
3. If path is of directory, display contents of that directory.
4. If path is of file, display information about that file.
*/
* Get file/directory information

## demo04 - File class
* create directory
* create file
* delete file


## demo05 - File Copy
* FileInputStream
* FileOutputStream
