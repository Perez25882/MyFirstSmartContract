My First Smart Contract - SimpleStorage
This project expands on my first Solidity contract, following the tasks outlined in Solidity Programming 101, Modules 2.2 – 2.4. The contract now demonstrates the use of various data types, functions, and visibility specifiers to provide a solid foundation for more advanced features.

Features Implemented
1. Data Types and Variables
I enhanced the contract with new variables and data types to manage more complex data:

State Variable: uint256 private favoriteNumber – Stores a single favorite number.
Dynamic Array: uint256[] public favoriteNumbers – Stores multiple favorite numbers.
Struct: struct Person – Groups a person’s name and favorite number.
Person[] public people – Array to store multiple people’s data.
Enum: enum ContractState – Defines two states: Active and Inactive.
ContractState public state – Stores the current contract state.

2. Solidity Functions, Conditionals, and Loops
storeNumber(uint256 _favoriteNumber): Takes a number and sets it as the new favorite number.
getFavoriteNumber(): A public view function that returns the stored favorite number.
isGreaterThan(uint256 _number): A conditional function that compares favoriteNumber to a given value and returns true or false.
sumToFavoriteNumber(): Uses a for loop to calculate the sum from 1 to the current favoriteNumber.

4. Visibility Specifiers
Private State Variable: favoriteNumber – Changed the visibility of this variable to private.
Internal Function: internalFunction() – Returns a simple string but can only be accessed internally.
Wrapper Function: callInternalFunction() – Exposes the internal function via a public wrapper.
External Function: externalFunction() – Returns a string, but can only be called externally.
Test Function: testExternalFunction() – Calls the external function using the this keyword.

6. Arrays, Structs, and Enums
addFavoriteNumber(uint256 _number): Adds a new number to the favoriteNumbers array dynamically.
addPerson(string memory _name, uint256 _number): Adds a new person with their name and favorite number to the people array.
Enum Functions:
activateContract() – Sets the contract state to Active.
deactivateContract() – Sets the contract state to Inactive.
isActive() – Checks if the contract is currently active.
Challenges Faced and How I Solved Them
Managing Private Variables:

I initially forgot to create a public getter function for the favoriteNumber variable. Fixed this by implementing getFavoriteNumber() to make the value accessible.
Using Internal and External Functions Correctly:

It was tricky to understand the difference between internal and external visibility. I used the this keyword inside testExternalFunction() to call externalFunction() correctly.
Working with Arrays:

I had some issues with adding elements dynamically to the favoriteNumbers array, but reviewing the example in Module 2.4 helped me fix the logic.
Conclusion
This project has been a great learning experience. I’ve gained a deeper understanding of Solidity’s data types, visibility specifiers, and functions. I’m excited to keep building on this foundation and explore more advanced features in future lessons.

