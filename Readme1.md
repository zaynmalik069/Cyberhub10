# Chmod permissions

| Octal | Permission | Who Can Do What                      |
| ----- | ---------- | ------------------------------------ |
| `777` | rwxrwxrwx  | Everyone: read, write, execute       |
| `755` | rwxr-xr-x  | Owner: all, Others: read & execute   |
| `700` | rwx------  | Only owner has all rights            |
| `644` | rw-r--r--  | Owner: read/write, Others: read-only |
| `600` | rw-------  | Owner: read/write only               |
| `400` | r--------  | Owner: read-only                     |
| `000` | ---------  | No one has any permission            |

# syntax
chmod 777 filename/foldername 

for example 
all permission access--

chmod +777 "filename"
* Removing all permission
* chmod -777 "file name"


# permissions explain 
r- read
w- write
x- exicute

syntax--
chmod a+r "filename/folder"
a- all permissions

* chmod o+r "filename/folder"
o- other permissions

* chmod g+r "filename/folder"
g- group permissions

* chmod u+r "filename/folder"
u - user permissions


# Chown-- To change user ownership
# chgrp-- to chnage group ownership

syntax 

sudo chown -c "username" "filename"


sudo chgrp -c "groupname: "filename"

----------------------------------------------------------

# basic command

cut command basically use to cut any record using character and fields drom any file or frome any command output 

-c= cut by charecters
-f= cut by fields
-d= define the delimeter symbol.. it can be anything like --- .;'" space
syntax--
for example--
1.cut -c1-5 /etc/passwd
2.cut -c2-8 /etc/passwd
----------------------------------------------
specific charecter print---
head -1 /etc/passwd | cut =c1-4
result= root
save thi file using command 
head -1 /etc/passwd |cut -c1-6 >/save

--- command - "Head"= first 10 line print 
and "tail" last 10 line print .
----------------------------------------------
cut -d : -f1 /etc/passwd 
result - print  total filed 


----------------------------------------------
