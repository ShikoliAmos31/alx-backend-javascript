
Short Specializations
Average: 145.07%
0x04. Typescript
JavaScript
TypeScript
 Weight: 1
 Project will start Jul 3, 2024 6:00 AM, must end by Jul 4, 2024 6:00 AM
 Manual QA review must be done (request it when you are done with the project)


Resources
Read or watch:

TypeScript in 5 minutes
TypeScript documentation
Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

Basic types in Typescript
Interfaces, Classes, and functions
How to work with the DOM and Typescript
Generic types
How to use namespaces
How to merge declarations
How to use an ambient Namespace to import an external library
Basic nominal typing with Typescript
Requirements
Allowed editors: vi, vim, emacs, Visual Studio Code
All your files should end with a new line
All your files will be transpiled on Ubuntu 18.04
Your TS scripts will be checked with jest (version 24.9.* )
A README.md file, at the root of the folder of the project, is mandatory
Your code should use the ts extension when possible
The Typescript compiler should not show any warning or error when compiling your code
Configuration Files
Please use these files for the following tasks

package.json
Click to show/hide file contents
.eslintrc.js
Click to show/hide file contents
tsconfig.json
Click to show/hide file contents
webpack.config.js
Click to show/hide file contents
Tasks
0. Creating an interface for a student
mandatory
Copy the following configuration files (provided above) into the task_0 directory: package.json, .eslintrc.js, tsconfig.json, webpack.config.js

Write your code in the main.ts file:

Write an interface named Student that accepts the following elements: firstName(string), lastName(string), age(number), and location(string)
Create two students, and create an array named studentsList containing the two variables
Using Vanilla Javascript, render a table and for each elements in the array, append a new row to the table
Each row should contain the first name of the student and the location
Requirements:

When running, Webpack should return No type errors found.
Every variable should use TypeScript when possible.
Repo:

GitHub repository: alx-backend-javascript
Directory: 0x04-TypeScript
File: task_0/js/main.ts, task_0/package.json, task_0/.eslintrc.js, task_0/tsconfig.json, task_0/webpack.config.js
 
1. Let's build a Teacher interface
mandatory
Create a directory task_1 and copy these configuration files into this folder: package.json, tsconfig.json, webpack.config.js

firstName(string) and lastName(string). These two attributes should only be modifiable when a Teacher is first initialized
fullTimeEmployee(boolean) this attribute should always be defined
yearsOfExperience(number) this attribute is optional
location(string) this attribute should always be defined
Add the possibility to add any attribute to the Object like contract(boolean) without specifying the name of the attribute
Example:

const teacher3: Teacher = {
  firstName: 'John',
  fullTimeEmployee: false,
  lastName: 'Doe',
  location: 'London',
  contract: false,
};

console.log(teacher3);

// should print
// Object
// contract: false
// firstName: "John"
// fullTimeEmployee: false
// lastName: "Doe"
// location: "London"
Repo:

GitHub repository: alx-backend-javascript
Directory: 0x04-TypeScript
File: task_1/js/main.ts, task_1/webpack.config.js, task_1/tsconfig.json, task_1/package.json
2. Extending the Teacher class
mandatory

