# NullPointerExceptions and Exercise

## NullPointerException
~~~~
Thrown when an application attempts to use null in a case where an object is required. These include:

    1) Calling the instance method of a null object.
    2) Accessing or modifying the field of a null object.
    3) Taking the length of null as if it were an array.
    4) Accessing or modifying the slots of null as if it were an array.
    5) Throwing null as if it were a Throwable value. 
~~~~
https://docs.oracle.com/javase/7/docs/api/java/lang/NullPointerException.html


So basically NullPointerException occurs when you try to:
1) Call a method on a null object: null.methodName();
2) or access a property of a null object: null.filedName;

like
~~~~
public class Circle() {
    public int x;
    public int y;
    public int r;
    
    public boolean containsPont(int pointX, int pointY) {
        //some implementation
    }
}

public class UseCircle() {
    public static void main(String[] args) {
        Circle circle = null;
        circle.containsPont(1,2); //case 1)
        System.out.println(circle.x); //case 2
    }
}
~~~~