# //TODO: Lists Simplified

See https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet#code for tips on using *Markdown* tags to format __.md__ files

## Goal

Work as a team to create a project proposal for your X-team to complete together.
The project does not have to be extremely difficult,
but there must be work to do for each member of your team.
You may reference figures using "See figure 1".  
Be sure to submit corresponding image files, i.e. figure1.png (or figure1.jpg) for each figure.

## Grading: To earn full credit, your team's proposal must include:

* (md) documentation: [this file] describing purpose and use of your program

* Description of a program that has:

  ** a main Java program class in a file named Main.java
  
  ** a custom data structure designed and built by your team
  
  ** comprehensive testing of individual units
  
 Caution: You are not being asked to implement this program, at least not yet. 
 We just want your group to make a proposal or pitch for your program.
 
 Tip: Your custom data structure can be composed of or extensions of data structures that you have learned and used in previous programming assignments.  We're looking for decisions about how to build a high-level data structure that will likely have lower-level components.

## Problem Description

Life is busy so why waste time. Our group recognizes that people have lots of things to and organization of these ideas is important for efficient time usage. There are many prexisting TODO or List programs but none that our group knows of allows cross listing tasks. Many tasks are part of or involve other tasks and recognizing the connection between tasks will allow users to save precious time in their busy lives. Our group will design a "TODO list" program that organizes tasks according to priority set by the user or any other variety of parameters such as due date, or time since creation. The biggest feature of this TODO list program is that the user will be able to link tasks by adding them to other lists. An example is that a project might require a certain part to complete so the user can add "get part" to both the project list and a shoping list. When the user marks the part task complete on the shopping list the program will also mark that task as done on the project list. This will help people streamline their TODO lists by preventing them from forgetting important tasks and will minimize inefficiencies in the daily lives of the users.

## Questions to answer for Exercise #2

1. Name: Give your project proposal a name (and edit the top line of this file)

*//TODO: Lists Simplified* (That is the name of the "TODO list" project its a play on the computer science java comments we didnt forget to do this part)

2. Output: Describe the output your program will produce.  Include and example format of the output produced.

Program will have easy to use GUI to keep track of lists and tasks. The output will be a visual list with tasks that can be checked off and edited.

3. Input: Describe the data that is needed to solve your problem. Include an example format of the input data.

The user will need to input tasks, priority of the task and other optional info, and if that task is linked to any other lists.

4. User Interface: Describe a user interface for your program.  Use text menus or a simple graphic user interface.

The user interface will be a GUI that allows settings and features to be tweaked regarding the program, its display, a specific task, its related tasks, priority and other parameters. The user will be able to click on and search through their various lists which will be displayed in a sublist on the side of the program.

5. Types List: Break your solution idea down into units that you think can be implemented with a single class.

* GUI update and draw
* GUI advanced features like menus, search box interaction and such
* List arrangement and data management, remove, insert, get ect
* List node and features reguarding TODO objects including parameters

Name each interface or class and briefly describe its function or purpose.
1. Main.java
* Runs the main loop for the GUI. Will listen to click events, as well as handling the addition and removal of TODO list items

2. List Node Interface
* Is a single todo task, contains text, priority, time and date, and additional features like due date
* has getter and setter methods for editable parameters so that the GUI can draw the TODO and access them
* contructors
* extended by created List Nodes

3.List Array
* an array of List Node objects that is the list itself, order can be changed by user and filtered according to different parameters
* title of list/array set by user
* is the unique data type created by our team. Its linked or interesecting arrays.

4.GUI
* constantly updates the graphical aspects of the program by checking data movement on the backend
* has buttons for adding lists, nodes, setting additional parameters of a node
* optional search capabilities

5.State Saving
* writes TODO lists to SQLite data base after each opperation to save the data
* loads the SQLite data base that saves the program state

6. Testing.java
* A JUnit test class used to test the implementation of the List Node and List array methods. Will test that when an event is fired, Main.java correctly calls the correct methods and produces the correct result.
## Edit and Submit this file and any figures referenced by this document.

