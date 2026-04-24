# Train-Consist-Management-App
Drawback of UC3 Approach
In UC3, we ensured the uniqueness of bogie IDs using HashSet.
While this solves duplication, it introduces a new problem:

HashSet does not preserve order.
A train consist must follow a physical sequence:
Locomotive → Passenger → Cargo → Guard Coach.


With HashSet, the arrangement becomes unpredictable, which is unacceptable for real-world train formation.
So, we need a structure that:
Maintains insertion order
Supports fast insertion/removal
Models real train chaining
This leads us to LinkedList.