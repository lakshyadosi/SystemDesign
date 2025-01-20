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
