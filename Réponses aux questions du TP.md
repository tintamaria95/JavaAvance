
## Exercice 1 :
  
  2. Eclypse écrit directement System.out.println() lorsque l'on écrit sysout et Ctrl + Space.
  3. Eclypse propose de faire un Override de la méthode toString().
  4. Eclypse propose de faire apparaître la main méthode directement.
  5. Eclypse propose d'écrire certaines méthodes comme equals(), hashcode(), toString(). Aprèsavoir écrit le set, et d'avoir pressé Ctrl + Space,
  		Eclypse propose de créer un Setter pourl'entier foo.
  6. Le Alt+Shift + R permet de renommer soit le nom de la class, soit le nom de la variable foo. Le renommage peut être effectué sur toutes les apparitions du nom de la class/variable.
  
 ## Exercice 2 :
  1. It works because the two private fields and the method newly created are a part of the same class Pointand we have a default constructor for Point which doesn't take any variable.
  2. It doesn't work because now the fields cannot be accessed by the new class TestPoint : we should change the x and y from "private" to "public"/"protected" or add a getter method.
  3. Because, we must be sure that value changes will be done by using a "setter method" and then that the new value will respect the will of the precedent programmer. (the caller cannot directly access to the variables and change them inappropriatly).
  4. The accessor allows a class to get the value (getter method) of an other class field. Here, it's needed by the class TestPoint to access the fields x and y. 
  5. The problem is that px and py do not exist as local variables. (we now have a constructor taking variables)
  6. To not have our programm to be confused between values, we must use the "this" key-word to specify that we point the object field.
  7. We could create a static variable number_of_points and increment it each time a new Object Point is created (add a "number_of_points++ in the constructor).
  8. It knows which one to call depending which arguments the constructor takes when we create an Object Point. For example, we could pass two double variables x and y or pass one parameter Point p.
  
 ## Exercice 3:
  1. It prints "true/nfalse". The true shows that the Objects p1 and p2 are the same by pointing on the same address.
  	  Even if p1 and p3 have the same coodinates, they stay two diferent obkjects with two different addresses.
  2. First the code printed 0 because in memory we have p2 pointing to p1. Also indexOf checks where the object is using the reference in memory, so it printed 0
It printed -1 meaning that p3 is not in the list but actually p3 is the same as p1. It should have printed 0

  
 ## Exercice 4 :

  2. If we try to add more points to the array than its capacity, then it throws the exception "ArrayIndexOutOfBoundsException"
  Then we should resize it.
  5. We get a "NullPointerException".In the case, we add a null value to point in the add methode, the Objects.requireNull throws an exception with a personnalidsed message
  6. In an arrayList we don’t have a limit to the size of the list.
  
 ## Exercice 5 :
  1. Les deux options sont les suivantes : faire une méthode translate qu'on appelle via un Point créé,
  ou faire une méthode static avec le Point à translater en paramètre.
  5. La translation est appliquée au point qui est le centre des deux cercles. Lorsqu'on appelle la méthode c2.translate, la translation s'applique aussi à c1.
  On doit faire en sorte que le point du centre du cercle ne soit pas mutable.
  9. La méthode devrait être déclarée dans la class TestPoint.
  
 ## Exercice 6 :
  1. Oui, on peut faire hériter ring de la classe Cercle en rajoutant simplement un rayon externe.
  4. Le Sysout renvoie le hashcode de l'adresse de l'objet. Il est nécessaire de réécrire la fonction toString().
  
