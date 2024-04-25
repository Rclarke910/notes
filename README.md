# notes

Objects in Java are created using the new keyword followed by a constructor call. Constructors initialize the newly created object and can be overloaded to provide different initialization options.

ex: Farmer farmer = new Farmer(variable)

Objects are accessed through reference variables, which hold the memory address (reference) of the object. Reference variables can be assigned to different objects of compatible types, allowing flexibility in object usage

ex:  farmer = new Farmer()

Objects are initialized by calling constructors, which can accept parameters to set initial state. Constructors can also call other constructors using this() or super() to reuse initialization code

ex: this.name = name super(name)

Objects have instance variables that define their state. These variables are declared within the class but outside of any method and are accessible throughout the object's lifetime.

ex: int cows;  
public Farmer(int cowNum){
cowNum = cows
}

Objects have methods that define their behavior. These methods can access and modify instance variables and perform operations specific to the object's purpose.

ex: public void moreCows() {
        cows *= 2;
    }

Java's garbage collector automatically deallocates memory used by objects that are no longer reachable. Objects become unreachable when there are no references to them, allowing the garbage collector to reclaim their memory.

Java has a finalize() method that can be overridden in a class to perform cleanup operations before an object is garbage collected. However, relying on finalize() for resource cleanup is discouraged due to uncertainty about when it will be called.

Assigning one object reference variable to another does not create a new object; it only copies the reference

The equals() method is used to compare objects for equality based on their contents. By default, equals() compares references, but it can be overridden in classes to provide custom equality comparisons.

Primitives are basic data types in Java, such as integers (int), floating-point numbers (double), characters (char), and booleans (boolean). These types hold simple values directly. References are variables that hold memory addresses pointing to objects. Unlike primitives, they don't hold the actual object data but rather a way to access it. Variables, both primitives and references, can be passed to methods as arguments. Primitives are passed by value, while references are passed by reference.
