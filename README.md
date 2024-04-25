# Linux-File-IO-Systems-locking
Ex07-Linux File-IO Systems-locking
# AIM:
To Write a C program that illustrates files copying and locking

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Write the C Program using Linux IO Systems locking

### Step 3:

Execute the C Program for the desired output. 

# PROGRAM:

## 1.To Write a C program that illustrates files copying 
```
#include <unistd.h>
#include <sys/stat.h>
#include <fcntl.h>
#include <stdlib.h>
int main()
{
char block[1024];
int in, out;
int nread;
in = open("filecopy.c", O_RDONLY);
out = open("file.out", O_WRONLY|O_CREAT, S_IRUSR|S_IWUSR);
while((nread = read(in,block,sizeof(block))) > 0)
write(out,block,nread);
exit(0);}

```

## 2.To Write a C program that illustrates files locking
```
```



## OUTPUT

## 1.To Write a C program that illustrates files copying 

![Screenshot 2024-04-25 105318](https://github.com/Bakkiyalakshmiethiraj/Linux-File-IO-Systems-locking/assets/144870983/46d4be2a-a2c8-4b34-9687-dec2167fcbdb)

## 2.To Write a C program that illustrates files locking



# RESULT:
The programs are executed successfully.
