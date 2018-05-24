# RAIDA-Language


### Name Spaces
Name spaces are held in folder names. 
The root folder is Lib. Then there are other folders such as Util,System, etc. 


### Entities
Entites. RAIDA language classes are know by their file names and have an "Entites" extension. Each entity has its own file. 
```
programName.dm //the DM (Dungeon Master) main program that auto starts
die.entity //for normal classes
die.abstract //abstract class
die.enum //enumerator
die.interface //Interface
die.global //Creates classes, variables and methods that will be available to all classes. 

gui.console
gui.web
gui.window
gui.iPhone
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

-uid--------------------
#id +4byte
-fields------------------
#sides +1byte { *NOT NULL, !UNIQUE, !PRIMARY KEY, *DEFAULT:10, *INDEX }//Number of sides the dice has
#sideUp +1byte //The side the is facing up
NOT NULL - Ensures that a column cannot have a NULL value
UNIQUE - Ensures that all values in a column are different
PRIMARY KEY - A combination of a NOT NULL and UNIQUE. Uniquely identifies each row in a table
FOREIGN KEY - Uniquely identifies a row/record in another table
CHECK - Ensures that all values in a column satisfies a specific condition
DEFAULT - Sets a default value for a column when no value is specified
INDEX - Used to create and retrieve data from the database very quickly
-constructors-----------------------
()
#sides = 6;
#sideUp = 1


-


```


## Primitive Types

### Default Integers:
#a = 10 //default Signed 4 byte integer. 

global.a# = 10 //Global Integer

output #a

### Advanced Integers
Advanced Integers have the # sign and Byte Lenght befor the name

#a +4byte //Unsigned four byte integer

#b -1byte //Signed one byte integer. 

### Decimals
#.a = 10.4 //Simiple 

### Boolean
?a = true //

### Text
$a =yea!//

### Type Conversions: 
$a = 43//
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






