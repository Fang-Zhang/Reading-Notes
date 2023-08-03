## Learnnig Approach
1. Vedio -> Official Doc
2. Coding can make understanding clearly

## Basics (Refer to the official document for more)
1. Type
   - string
   - number (not int, float, or numbers)
   - boolean
2. function
   - void vs null vs never vs undefined
3. class
4. Object
5. Type Aliases
6. read-only
7. Union
8. Array
9. Tuple: order is also a matter
10. Enum
11. Interface vs Type
12. Class - the public and private member
13. Getter and Setter
14. Access Modify: protected
15. Interface and Class implements
16. Abstract Class vs Interface: Actually, both of them are blueprints.
17. Generics vs Array and Arrow function
18. Type Narrowing

## TypeScript Setup for the Project
1. tsc --init
2. npm init -y
3. index.html -> <script src="./dist/index.js"></script>

## TypeScript Best Practice
1. Don't put the annotation too explicitly. (such as: let mynum: number = 3.14)
2. Don't use "any" type anywhere. Basically, "any" means turning off the type-checking function for variables. Using compiler flag "noImplicitAny" to flag any implicit "any" as an error.