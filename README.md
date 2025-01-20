# SystemDesign
## class diagram
![](https://substackcdn.com/image/fetch/f_auto,q_auto:good,fl_progressive:steep/https%3A%2F%2Fsubstack-post-media.s3.amazonaws.com%2Fpublic%2Fimages%2F72d3654b-44b5-4708-a634-527534bd0937_3772x3040.png)

### Key Concepts Summary
#### 1. Association
Definition: A basic relationship between two entities where they can interact but exist independently of one another.
Characteristics:
No ownership or part-whole distinction.
Both entities can exist independently.
Example:
Entities: Student and Course
Description: A student can enroll in one or more courses, and a course can exist without any students enrolled.
#### 2. Aggregation
Definition: A specialized form of association that indicates a "whole-part" relationship. The whole can contain multiple parts, and while the parts can exist independently, they are conceptually connected to the whole.
Characteristics:
Represents a whole-part relationship.
Parts can exist independently of the whole.
Example:
Entities: Person and Pet
Description: A person can have multiple pets. The person can own several pets, but those pets can also exist by themselves if they are given away or adopted.
#### 3. Composition
Definition: A specific type of aggregation relationship that implies a strong life-cycle dependency between the whole and its parts. If the whole is destroyed, the parts also cease to exist.
Characteristics:
Strong ownership and part-whole relationship.
Parts cannot exist independently of the whole.
Example:
Entities: House and Room
Description: A house consists of multiple rooms. If the house is demolished, the rooms also cease to exist.
Summary Table of Relationships
Table
Relationship Type	Example Pair	Description	Existence Independence
Association	Student - Course	Students enroll in courses.	Yes, both can exist independently.
Aggregation	Person - Pet	A person has multiple pets.	Yes, pets can exist independently of the person.
Composition	House - Room

#### Summary of Relationships
1. Person and Phone
Type: Association
Definition: A loose relationship where the entities (person and phone) can exist independently.
Key Points:
Ownership does not imply dependency: A person can sell or discard their phone without affecting their identity.
Nature of relationship: More transactional. Phones are tools and can be replaced.
2. Person and Pet
Type: Aggregation
Definition: A whole-part relationship where pets are considered parts of a person's life.
Key Points:
Significant connection: Pets are integral to a person’s identity and well-being.
Nature of relationship: Represents care and companionship. Pets cannot be simply treated as objects and often form emotional bonds with their owners.
Visual Summary
Person - Phone:
Association: Person --- (owns) --- Phone
Person - Pet:
Aggregation: Person <>--- (has) --- Pet

####

##### Abstract Class
Definition: An abstract class can have both implemented and unimplemented methods.
Use Cases:
Shared Code: When multiple related classes share common functionality.
Example: A Vehicle class that has a common method like startEngine(), but different types of vehicles (like Car and Truck) can implement their own drive() method.
Partial Implementation: When you want to provide some default behavior but still require certain methods to be overridden.

##### Interface
Definition: An interface only declares methods (usually with no implementation).
Use Cases:
Multiple Implementations: When different classes, possibly unrelated, need to implement the same methods.
Example: An animal interface with a method called makeSound(). Both Dog and Cat classes can implement this method in their own way.
Contract for Behavior: When you want to define capabilities without worrying about how they are implemented.

#### References:
https://blog.algomaster.io/p/uml-class-diagram-explained-with-examples
