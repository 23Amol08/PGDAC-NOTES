# Day12 - Classwork



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

Movies class : - id(int) , title(String) , rating(double)
List<Movie> list = new ArrayList<>();
list.add(new Movie(1, "Star Wars", 7.5));
list.add(new Movie(2, "Godfather", 8.0));
list.add(new Movie(3, "Hidden Figures", 7.0));
list.add(new Movie(4, "Bruce Almighty", 6.5));
list.add(new Movie(5, "Forest Gump", 8.5));

## demo01 - Data streams
* DataOutputStream
* DataInputStream

## demo02 - Object streams ( check size) 
* ObjectOutputStream
* ObjectInputStream
* Serializable, serialVersionUID

## demo03 - Buffered streams
* BufferedOutputStream
* BufferedInputStream


#Movies class : - id(int) , title(String) , rating(double)
List<Movie> list = new ArrayList<>();
list.add(new Movie(1, "Star Wars", 7.5));
list.add(new Movie(2, "Godfather", 8.0));
list.add(new Movie(3, "Hidden Figures", 7.0));
list.add(new Movie(4, "Bruce Almighty", 6.5));
list.add(new Movie(5, "Forest Gump", 8.5));


## demo04 - PrintStream
* formatted output

## demo05 - Reader/Writer
* Character encoding i.e. Charset.availableCharSets() , print size (map.forEach((K,V) -> System.out.println(K + "--" +V)))
* FileReader
  Charset charset = Charset.forName("UTF-16LE");
* FileWriter
* FileInputStream , InputStreamReader(for Reading) 
* FileWriter 
* FileOutputStream , OutputStreamWriter (for writing) 

------------------
#demo02 
Creating process in java( rt.exec(note) , process.waitfor()) 

##demo04
*Creating the thread in java 
*// thread creation - method 1
// step1: create a new class inherited from thread class and override its run() method.
// step2: create object of that thread class and call its start() method.
*// thread creation - method 2
// step1: create a new class inherited from Runnable interface and implement its run() method.
// step2: create object of Thread class with the object of above Runnable class and call thread's start() method
//class YourRunnable implements ( Thread th2 = new Thread(new YourRunnable());) 

##demo05 - Daemon threads
// thread is by default non-daemon thread (foreground)
// daemon (background) threads are for giving services to non-daemon (foreground) threads.
// when all non-daemon threads in a java process are terminated, the JVM exits.
// due to this all daemon threads are automatically (forcefully) terminated.

// main thread is non-daemon thread (foreground)
* setDaemon()

