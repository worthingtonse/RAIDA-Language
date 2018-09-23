# RAIDA-Language

### case insensitve
In this language, case does not matter. 

### Program Name
The name of the program is the name of the folder that holds all the class fies. This assumes that there is a main executale file.
If not then the folder name is just part of the name space.  


### Name Spaces
Name spaces are held in folder names that don't and may or may not include a main program

### Types of files in a program:
.class //for classes

.enum //for enumerators

.row //for data structures like a row in a table This may also be called entity

.icon //for the graphics of a program

.pk //the signature of a program

.main //code that will start the execution

.global  //For static global variables

.config  //any configuration

.test //Code that tests other classes

.abstract // abstract class

.interface //rules for connecting classes

.bus //communications code allowing code to talk to each other. 

.gui //Specifice handles to allow the program to communicate in different ways. 

### Class
Classes. RAIDA language classes are know by their file names and have an "class" extension. Each class has its own file. 
However, there are other componets besides classes including, main, entity, abstract, enum, interface, and global. 
There are also files called "bus" files that allow other classes to monitor and discover. 
Gui files allow the code to be displayed in certain GUIs.  
```
programName.main //the DM (Dungeon Master) main program that auto starts
Car.class //for normal classes
Person.entity //for normal classes
Vehicle.abstract //abstract class
DaysOfWeek.enum //enumerator
Agreement.interface //Interface
Config.global //Creates classes, variables and methods that will be available to all classes. 
Gui.bus //Allows classes to fee information and recieve intformation from other classes
console.gui
web.gui
windows.gui
iPhone.gui
Signature.pk
graphic.icon
```
### Junctions

### Global

### GUIs 




### Entity parts
Each Entity has parts seperated by "-------------"
```
Rights
--------------
Unique Identifier (Assigned at run time)
------------
Properties
------------
Foreign Keys
------------
constructors
------------
methods
------------
Communication
------------
gui aspects
------------
Aspects Used for Global stuff
```
## Sample Class called Die (like a dice)

```
-About----------------
Up here it is all notes.
You can write what you want. 

-RIGHTS
*Persistant
*Gui
*Enrypted
*Static
*

-fields------------------
#sides //Number of sides the dice has
#sideUp //The side the is facing up

-constructor_1( @#sides, p#b)
{
   #sides is p#sides;
   #sideUp is p#up
}//end Constructor_1

-Methods
*add( p#FirstNumber p#SecondNumber)
{ 
  *random = random(10,20)
  return p#FirstNumber + p#SecondNumber
}*add


```


## Primitive Types

### Default Integers:
```
#age is 10 ;  12 byte double that can handle almost any computation 
#height is 2.4
#duration is .09998883

global.#age = 10 ; Global Integer
```
### Boolean
?oldEnough is true ;

### Text is an array of unicode characters and can be char or string
$firstName is Billy ;

### Type Conversions: 
$age is 43//
#age from $age Fail{"Sorry fucker"}
$age from #age
$oldEnough from ?oldEnough
?oldEnough from $oldEnough

VERT: #a to $a FAIL: GOTO ^here
V: #a to $a F: GOTO ^here

### Variable names
Variables can start with letters or numbers. No spaces or other characters

### Operators
+, -, *, /,
#a = 5 mod 5
^Concatinate this $stuff with #a^
<> not equal


if(){}
M:

## Text

### Escape 

To escape, simply put some angle brackets around it:

p( The value of the variable <#>a is now #a )//prints: " The value of the variable #a is now 15 "

### Concatination

$fullName =Sean H. Worthington//
$myString =What the hell are you writing about $fullName?

### conatination with white space

$emailToCustomer=

The wite space is now recording.
It will now include character returns and 
  tabs like that one
  
  And empty lines like the one above.//
  
  
### Ignoring all   






