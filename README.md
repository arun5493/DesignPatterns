# HW2

##Creational Design Pattern
### 1) Singleton:
Singleton pattern is used when the application requires only one instance of the object. This design pattern should be such that it allows initializations on demand and should be accessible globally. Singleton pattern is implemented when the ownership of a single instance cannot be distinctly assigned.

<img src ="SingletonPattern.png"></img>

Other design patterns such as Factory, Prototype can implement singleton design in them. Singleton pattern is implemented by declaring all constructors to be private and by providing a static method returning a reference to the instance.

Example:
Consider the CEO of the company. There can always be one CEO for any organization and even though the person can be replaced, the title will be present. Some functions of the CEO will be to provide guidelines and conducting research/development activities.


### 2) Prototype

Prototype pattern refers to creating duplicate object after creation of a single object (Prototype). We have to specify the kinds of objects to create a prototype and later create new objects by copying this prototype. Prototyping is done by defining an abstract class specifying a virtual clone, maintaining the dictionary of all clone-able derived classes. Creating a prototype often means, creating an object to perfection before production of other objects. Keeping performance in mind, even though the cost of initial creation of a prototype is high, the cost of subsequent production of objects is very minimal as prototype will be &#39;cached&#39;. Prototyping, thus avoids creation from scratch, supporting cheaper production of the clones. A subtle difference between factory pattern and prototype is that, prototype pattern implements creation through delegation, whereas factory pattern implements creation through inheritance. Prototype co-opts one instance of a class and be used as a breeder of all future instances.

<img src ="PrototypePattern.png"></img>

Example: Consider car manufacturing, before a car is being mass produced, a single car will be fully built and tested thoroughly and only upon satisfying the requirement, it will be sent for mass production. Now, the cost of building up a single instance is going to be high, but when seen with a broader perspective, this method seems to more efficient and profitable.


##Structural Design Pattern
###1)Decorator

Decorator is a type of structural pattern which is primarily used to embellish the application as per the clients&#39; requirement. This type of design pattern does not implement inheritance for the decoration purpose, instead will add a decorator function to the existing application, without breaking the other functionalities.

<img src ="DecoratorPattern.png"></img>

Example:

Consider the same car production. After manufacturing the car in a mass –production manner, all the cars look alike. Thus according to the user&#39;s requirement, a &#39;decorator function&#39; can be used to add extra components like spoilers, bumpers, hoodie etc. The user has the option of choosing which decorator function to use and accordingly embellish the end product.


###2) Façade

The English definition of façade is &quot;An outward appearance that is maintained to conceal a creditable reality&quot;

The Façade design pattern also does the same – wrap a complex subsystem into a simpler one, thus enabling the ease of use for the clients. One effect of using such a design pattern is that, it restricts the features and power of the subsystem, as it allows only a certain level of flexibility to the end users. This type of design patter is followed where the need to abstract the complex activity is high as compared to the need of learning the subsystem.

<img src ="FacadePattern.png"></img>

Example: Consider a UI that connects to a complex database. The UI will mostly be designed such that the client/user only sees the end result, after fetching from the database. While in reality, complex codes are ran to fetch the data in the appropriate manner, which the user need not necessarily know. Such a system can be considered as a Façade design pattern.


## Behavioral design patterns
###1) Template

Template method is a type of behavioral pattern which defines the skeleton of an algorithm as an abstract class, allowing its subclasses to provide concrete behavior. The interfacing method that the user calls is actually the template method. For analogy purpose, we can even think about the concept of inheritance. The base class will hold a standard set of methods and the derived class can be modified such that new methods can be added, including the ones from the base class. Template Method uses inheritance to vary part of an algorithm whereas strategy uses delegation in modifying the algorithm. Factory method is a special form of template method.

<img src ="TemplatePattern.png"></img>

Example:  Consider the example of an institution which has different departments.  A template method can be used for implementing such a design, as each department shares some common features, like classroom, faculty, No. of students. In addition, each department varies with the courses they offer, laboratories they have etc. Exams and grading methods will be common across all institutions.

###2) State

State pattern is one of the behavioral design patterns which are used when an Object changes its behavior based on its internal state. Such a pattern can be implemented by having a state variable in the object and by using If-Else conditions to select different states. The state machine&#39;s interface is encapsulated in the wrapper class.

<img src ="StatePattern.png"></img>

Example: Consider the example of TV remote. A TV remote often has various functionalities, like volume control, program changing, power on/off etc. A remote here acts as the wrapping function and depending the state variable ( the button pressed) the remote performs appropriate actions.



