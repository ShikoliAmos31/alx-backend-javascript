0x02. ES6 classes
OOP
JavaScript
ES6
 Weight: 1
 Project will start Jun 27, 2024 6:00 AM, must end by Jun 28, 2024 6:00 AM
 Checker was released at Jun 27, 2024 12:00 PM
 An auto review will be launched at the deadline


Resources
Read or watch:

Classes
Metaprogramming
Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

How to define a Class
How to add methods to a class
Why and how to add a static method to a class
How to extend a class from another
Metaprogramming and symbols
Requirements
All your files will be executed on Ubuntu 18.04 LTS using NodeJS 12.11.x
Allowed editors: vi, vim, emacs, Visual Studio Code
All your files should end with a new line
A README.md file, at the root of the folder of the project, is mandatory
Your code should use the js extension
Your code will be tested using Jest and the command npm run test
Your code will be verified against lint using ESLint
Your code needs to pass all the tests and lint. You can verify the entire project running npm run full-test
Setup
Install NodeJS 12.11.x
(in your home directory):

curl -sL https://deb.nodesource.com/setup_12.x -o nodesource_setup.sh
sudo bash nodesource_setup.sh
sudo apt install nodejs -y
$ nodejs -v
v12.11.1
$ npm -v
6.11.3
Install Jest, Babel, and ESLint
in your project directory, install Jest, Babel and ESList by using the supplied package.json and run npm install.

Configuration files
Add the files below to your project directory

package.json
Click to show/hide file contents
babel.config.js
Click to show/hide file contents
.eslintrc.js
Click to show/hide file contents
and…
Don’t forget to run $ npm install when you have the package.json

Tasks
0. You used to attend a place like this at some point
mandatory
Implement a class named ClassRoom:

Prototype: export default class ClassRoom
It should accept one attribute named maxStudentsSize (Number) and assigned to _maxStudentsSize
bob@dylan:~$ cat 0-main.js
import ClassRoom from "./0-classroom.js";

const room = new ClassRoom(10);
console.log(room._maxStudentsSize)

bob@dylan:~$ 
bob@dylan:~$ npm run dev 0-main.js 
10
bob@dylan:~$ 
Repo:

GitHub repository: alx-backend-javascript
Directory: 0x02-ES6_classes
File: 0-classroom.js
  
1. Let's make some classrooms
mandatory
Import the ClassRoom class from 0-classroom.js.

Implement a function named initializeRooms. It should return an array of 3 ClassRoom objects with the sizes 19, 20, and 34 (in this order).

bob@dylan:~$ cat 1-main.js
import initializeRooms from './1-make_classrooms.js';

console.log(initializeRooms());

bob@dylan:~$ 
bob@dylan:~$ npm run dev 1-main.js 
[
  ClassRoom { _maxStudentsSize: 19 },
  ClassRoom { _maxStudentsSize: 20 },
  ClassRoom { _maxStudentsSize: 34 }
]
bob@dylan:~$ 
Repo:

GitHub repository: alx-backend-javascript
Directory: 0x02-ES6_classes
File: 1-make_classrooms.js
  
2. A Course, Getters, and Setters
mandatory
Implement a class named HolbertonCourse:

Constructor attributes:
name (String)
length (Number)
students (array of Strings)
Make sure to verify the type of attributes during object creation
Each attribute must be stored in an “underscore” attribute version (ex: name is stored in _name)
Implement a getter and setter for each attribute.
bob@dylan:~$ cat 2-main.js
import HolbertonCourse from "./2-hbtn_course.js";

const c1 = new HolbertonCourse("ES6", 1, ["Bob", "Jane"])
console.log(c1.name);
c1.name = "Python 101";
console.log(c1);

try {
    c1.name = 12;
} 
catch(err) {
    console.log(err);
}

try {
    const c2 = new HolbertonCourse("ES6", "1", ["Bob", "Jane"]);
}
catch(err) {

