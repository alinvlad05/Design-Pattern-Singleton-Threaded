# Design-Pattern-Singleton-Threaded
 
You create the object you want only one of when the code is first loaded into the JVM.
Don't let getInstance create any objects at all- let it RETURN only that ONE OBJECT that's already been created.
The singleton object is created before any threads can get it and returned as needed.
This is a bettern solution than synchronizing the getInstance method.
There's no possibility of creating more than one object, so there's no going to be any conflict between threads.
You've removed all the costs involved with synchronizing code just by taking the object creation code out of the getInstance method.
