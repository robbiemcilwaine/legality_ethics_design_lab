### What do we mean by coupling and cohesion when discussing structured design?

- In software engineering, structured design entails breaking large processes into smaller, more manageable modules. This has the effect of reducing complications and increasing reusability.
- Coupling in the context of structured design refers to relationship or the degree of interdependence between modules in a software system. This can be further divided into high and low coupling which detail how closely connected different modules are and how much changes in one affect the other.
- Cohesion, on the other hand, refers to the extent to which a module's components are connected and how much they work collectively towards the module's purpose. High cohesion involves components working closely together towards this purpose and low cohesion means that components are loosely related and fulfill various roles within the module.

### What is the difference between top-down and bottom-up design? Which best describes a function oriented design?

- Function oriented design (FOD) is a method in which a model is broken down into a set of units, each with a clearly defined function, which interact with each other.
- Top down design involves defining a general outline of a system, and then defining each part more specifically until the entire outline is ready for validation.
- Conversely, the bottom up design approach involves defining respective parts in detail and joining these to form the entire system.
- Since function oriented design decomposes the larger system into smaller, well defined parts, this is a top down design approach.

### In which design methodology would a class diagram be most useful?

- Object oriented design (OOD) bases software design around objects instead of functions and logic.
- Class diagrams provide a visual representation of a system's classes, their respective attributes and methods, as well as the relationship between classes.
- Since OOD revolves around objects, which are instances of classes, class diagrams are most appropriate for this design methodology.

### What are the four pillars of object oriented programming? Give a single-sentence description of each.

- **Encapsulation**: Object categorise variables (state) and methods (changing and using state) into a single *object* to restrict access to these parts.
- **Abstraction**: Removing parts of a class that are deemed unnecessary in order to reduce complexity.
- **Polymorphism**: The capacity of a single class to represent multiple different forms.
- **Inheritance**: The ability of a *child class* (or subclass) to inherit methods and variables from a *parent class* (or superclass)

### What is the strategy pattern? How would its implementation differ between a functional and object oriented system?

- The strategy pattern allows engineers to employ different strategies through selecting behaviour from an object into classes that are interchangeable at runtime, leading to greater flexibility and reusability and leaving the object's code unchanged.
- This follows the concept of encapsulation in OOD by grouping behaviour from an object together and making them interchangeable. The key difference is that OOD is a broader technique for designing software around objects, and that the strategy pattern is a specific design approach within OOD.
- FOD, on the other hand, achieves similar goals through functions and their arrangements within a system. Since this method doesn't involve the use of objects, employing the strategy pattern would be redundant within a FOD context.

### Imagine your is creating a new online payment system. In order to gain maximum market share it can't be tied to a particular sector - it needs to work just as well when ordering a takeaway as when buying a new coat. Which design methodology would you suggest following? Give some justification for your decision.

To ensure adaptability over sectors and enhance market share, I would suggest employing an object oriented approach:

1. **Flexibility**
- OOD allows the encapsulation of data and methods related to payments within objects, meaning you can create various classes, each for different sectors, and the payment methods offered within these sectors. Each of these defined classes can encapsulate logic specific to each sector.
- As well as this, polymorphism allows a common interface to be defined for different sectors, which can be useful when implementing sector classes into the program. You could define a class that contains the essential methods and data needed for an online purchase to be made, and each sector class that you implement can be represented by this class, while defining their unique data and functionality.
2. **Design Patterns**
- Since the strategy pattern falls under the category of OOD, this design method will be useful in this scenario as flexibility is required - different strategies can be implemented, depending on whether you're ordering a takeaway or buying a coat, at runtime (the time of the purchase) making the process consistent across sectors.
3. **Modularity**
- OOD promotes the development of separate modular components in a system. For example, if the takeaway sector requires some additional functionality, like applying a service charge, a new module can be created to implement this without compromising the rest of the system.

# Resources:
[Structured Design](https://www.sciencedirect.com/topics/computer-science/structured-design)\
[Coupling and Cohesion 1](https://www.geeksforgeeks.org/software-engineering-coupling-and-cohesion/)\
[Coupling and Cohesion 2](https://unstop.com/blog/difference-between-cohesion-and-coupling-in-software-engineering)\
[Function Oriented Design](https://www.geeksforgeeks.org/software-engineering-function-oriented-design/)\
[Top Down vs. Bottom Up Design](https://www.geeksforgeeks.org/difference-between-bottom-up-model-and-top-down-model/)\
[Object Oriented Programming](https://www.techtarget.com/searchapparchitecture/definition/object-oriented-programming-OOP#:~:text=Object%2Doriented%20programming%20(OOP)%20is%20a%20computer%20programming%20model,has%20unique%20attributes%20and%20behavior.)\
*The Self Taught Programmer - Cory Althoff*\
[Strategy Pattern 1](https://www.freecodecamp.org/news/a-beginners-guide-to-the-strategy-design-pattern/#:~:text=The%20Strategy%20Design%20Pattern%20is,statically%20choosing%20a%20single%20one.)\
[Strategy Pattern 2](https://www.geeksforgeeks.org/strategy-pattern-set-1/)\
[Modularity](https://www.lenovo.com/gb/en/glossary/modularity/?orgRef=https%253A%252F%252Fwww.google.com%252F)