To see **what lives in the given directory**.
```shell
ls [argument]
ls -l /directory # will give you more information about the file and directory 
drwxr-xr-x 1 missing  users  4096 Jun 15  2019 missing
```
The output line can be understood in this way: 
1. d means that the argument is **a directory** 
2. rwx indicates what permissions **the owner of the file, the owning group and everyone else have**
	1. w stands for **modify**
	2. x stands for **search (enter the directory)**
	3. r stands for **read (list the content)**
3. - indicates that **the given principal does not have the given permission** * [ ] what does it means ?   <!--SR:!2023-03-21,9,250!2023-03-14,1,230-->


