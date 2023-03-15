Different commands will be used inside the window. Typically used ones will be listed: 
# clc
?
```matlab
clc %Clean the command window without cleaning up the workspace. 
```
# clean 
?
```matlab
% clean specific variables 
clean variable_name
% Clean all the variables if there is no name provided
clean
```
# suppressing
Do not print the result of the command 
?
```matlab
a =x; % use; to suppress 
```
<!--SR:!2023-03-23,11,250-->

# Quit environment
?
```matlab
quit()
```
# Regain control 
Ctrl-c 
# saving variables <!--SR:!2023-03-22,10,250-->

Save all the variables in a . mat file
?
```matlab 
save filename.mat 
# to save only some of the variables 
save filename.mat varaible_name
```
# loading variables
?
```matlab
load filename.mat
# to load specific varaibles
load filename.mat variable_name 
```
# continue a command <!--SR:!2023-03-15,2,230-->

Add **…** at the end <!--SR:!2023-03-19,7,250-->

# repeating a command
Use up-arrow key
# get help for commands

### help
?
```matlab
help command name
```
<!--SR:!2023-03-15,3,250-->

### lookfor
?
```matlab
lookfor xyz 
```
will search *xyz* through command summaries
### doc
?
```matlab
doc name_or_phrases % this will search through the documentation
```
<!--SR:!2023-03-20,8,250-->

# block comments

Ctrl + r for **comment** the whole block
Ctrl + t for **uncomment** the whole block <!--SR:!2023-03-21,9,250!2023-03-16,3,269-->
