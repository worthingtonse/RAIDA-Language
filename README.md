# RAIDA-Language


### Name Spaces
Name spaces are held in folder names. 
The root folder is Lib. Then there are other folders such as Util,System, etc. 


### Classes
Classes. RAIDA language classes are know by their file names. Each class has its own file. 
```
programName.dm //the DM (Dungeon Master) main program that auto starts
die.class //for normal classes
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




### Class parts
Each class has three parts seperated by "-------------"
```
Unique Identifier (Assigned at run time)
------------
fields
------------
Foreign Keys
------------
constructors
------------
methods
------------
services
------------
gui aspects
------------
Aspects Used for Global stuff
```
## Sample Class called Die (like a dice)

```
Up here it is all notes.
You can write what you want. 
-uid--------------------
#id +4byte
-fields------------------
#sides +1byte //Number of sides the dice has
#sideUp +1byte //The side the is facing up
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
?a = true

### Text
$a =  yea!

### Type Conversions: 
$a = 43
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





