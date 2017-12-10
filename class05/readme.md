## Object initialization in java
Lehetőségek:
 * Instance variable initializers
 * Constructor
 * Instance initializer
 
A fenti három lehetőség előnyei, hátrányai:

### Instance variable initializers
Ezt a módszert ajánlottam én, mikor a propery deklaráláskor értéket adsz neki. Előnye, hogy könnyen olvasható és minden esetben inicializálja a propertyt.
Hátránya, hogy csak akkor lehet így inicializálni egy propertyt ha azt 1 sorban meg tudjuk tenni. (Tehát nem lehet ilyenkor pl if-et használni)

### Constructor
Ezt ajánlotta a tanárod.
Előnye, hogy ilyenkor több sorban is lehet inicializálni a propertyt (tehát lehet mondjuk if-el elágaztatva egy feltétel szerint különböző értéket adni egy propertynek)
Hátránya hogy ha több konstruktorod van és mindegyik konstruktorral inicializálni szeretnéd az adott propertyt akkor azt az inicializáló részt minden konstruktorba bele kell írni.
(Ez ugye kód duplikáció amit nagyon nem szeretünk.)

### Instance initializer
Erről eddig még nem beszéltünk. Ez egy olyan kódblokk ami minden konstruktor előtt lefut és lehet benne több sorban is inicializálni a propertyket. Továbbá mivel minden konstruktor futás előtt lefut ezért nem kell a konstruktorokban duplikálni az inicializáló kódot.
Magyarul ez egyesíti az előző két megoldás jó tulajdonságait. Hátránya, hogy ritka mint a fehér holló. Egy esetre emlékszem talán, hogy ilyet láttam volna java kódban a munkahelyi projectben. (Nem ismerik az emberek)

Rövid leírás a témában:

https://www.programcreek.com/2011/10/java-class-instance-initializers/

Hosszabb leírás:

https://www.javaworld.com/article/2076614/core-java/object-initialization-in-java.html

Ahogy láthatod a mi szintünkön most kb midegy hogy a három lehetőség közül melyiket használjuk. Így ez most csak ízlés kérdése, hogy melyiket választod.

## Find the max element in an array
http://szit.hu/doku.php?id=oktatas:programoz%C3%A1s:programoz%C3%A1si_t%C3%A9telek:mondatszer%C5%B1_le%C3%ADr%C3%A1s#maximum_kiv%C3%A1laszt%C3%A1s
