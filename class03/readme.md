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

## Exercise

Készíts egy Kutya osztályt aminek két String propertyje van "nev" és "fajta"

Készíts egy Ember osztályt aminek van egy "nev" (string) és egy "kutya" (Kutya) tíspusú propertyje.

Készíts egy "Par" nevű osztályt aminek van egy "leiras" nevű (nem statikus) metódusa ami a paraméterben megadott Ember típusú mezőnek egy stringbe összekonkatenálja a nevét, ha van kutyája akkor a utána a kutya nevét és a kutya fajtáját (space-el elválasztva az egyes mezőket).

Pl.: Ha az Endre nevű "Ember"-nek nincs kutyája akkor a leiras ezzel a Stringgel tér vissza:
~~~
"Endre"
~~~
Ha van kutyája és a "Kutya" neve Morzsa a fajtája pedig puli akkor:
~~~
"Endre Morzsa puli"
~~~

Készíts egy teszt osztályt amiben példányosítasz:
 * Ember osztályból egy példányt (ember0) aminek van beállítva neve
 * A Kutya osztályból egy példányt (kutya0) aminek van beállítva neve és fajtája.
 * Az ember0 -nak állítsd be, hogy a kutya0 a kutyája.
 * Hozz létre egy példányt a Par nevű osztályból (par0)
 * Hívd meg a par0 leiras nevű metódust az ember0 paraméterrel
 * Vizsgáld meg, hogy az előző pontban lévő metódus hívás azt az eredményt adja-e vissza amire számítottál.