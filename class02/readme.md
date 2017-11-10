Multiple ways to generate random numbers
----

# Math.random() versus Random.nextInt(int)
https://stackoverflow.com/questions/738629/math-random-versus-random-nextintint

# How do I generate random integers within a specific range in Java?
https://stackoverflow.com/questions/363681/how-do-i-generate-random-integers-within-a-specific-range-in-java


The ultimate way to generate random numbers
Usage:
~~~~
import java.util.concurrent.ThreadLocalRandom;

// nextInt is normally exclusive of the top value,
// so add 1 to make it inclusive
int randomNum = ThreadLocalRandom.current().nextInt(min, max + 1);
~~~~

https://docs.oracle.com/javase/8/docs/api/java/util/concurrent/ThreadLocalRandom.html