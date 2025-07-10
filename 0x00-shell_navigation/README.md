# 0x00. Shell, navigation

![Shell](https://img.shields.io/badge/Shell-6f42c1?style=flat&logo=visualstudio&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-6f42c1?style=flat&logo=visualstudio&logoColor=white)

##  Concepts Learnt
### Commands

- `man pwd`
- `man ls`
- `man cd`
- `man less`
- `man touch`
- `man cp`
- `man mv`
- `man rm`
- `man mkdir`
- `man rmdir`

### General

- How to navigate in an Unix system
- How to list files and directories
- How to display the content of a file
- How to create a file or directory
- How to remove a file or directory
- How to move or copy a file or directory

## Tasks
### 0. Create me!

Access your sandbox and:

- Change your working directory to `/root`
- Then, create an empty file `so_cool`

**Advices:**

- Don’t forget to validate your current working directory
- Don’t forget to display the list of files of your current directory to validate the creation of the new file

```
root@a710280214ff:/# cd /root
root@a710280214ff:~# touch so_cool
root@a710280214ff:~# ls
empty_directory  not_here  old_school  ready_to_be_removed  school  so_cool
root@a710280214ff:~# pwd
/root
root@a710280214ff:~#
```

### 1. More of me

Access your sandbox and:

- Change your working directory to `/root`
- Then, copy the file school to `/tmp`

```
root@a710280214ff:~# cd /root
root@a710280214ff:~# cp so_cool /tmp/
root@a710280214ff:~# ls /tmp/
so_cool  tmp.DAOEzJT0J6  tmp.dOKjikw0Ig  tmpztrs6ymg
root@a710280214ff:~# 
```

### 2. To old
Access your sandbox and:

- Change your working directory to `/root`
- Then, rename the file `old_school` to `new_school` (in the same directory)

```
root@a710280214ff:/# cd /root
root@a710280214ff:~# ls
empty_directory  not_here  old_school  ready_to_be_removed  school  so_cool
root@a710280214ff:~# cd /root
root@a710280214ff:~# mv old_school new_school
root@a710280214ff:~# ls
empty_directory  new_school  not_here  ready_to_be_removed  school  so_cool
root@a710280214ff:~#
```

### 3. Not here

Access your sandbox and:

- Change your working directory to `/root`
- Then, move the file `not_here` to `/tmp/right_school`

```
root@a710280214ff:~# cd /root
root@a710280214ff:~# ls
empty_directory  new_school  not_here  ready_to_be_removed  school  so_cool
root@a710280214ff:~# mv not_here /tmp/right_school
root@a710280214ff:~# ls /tmp/
right_school  so_cool  tmp.DAOEzJT0J6  tmp.dOKjikw0Ig  tmpztrs6ymg
root@a710280214ff:~#
```

### 4. Not anymore

Access your sandbox and:

- Change your working directory to `/root`
- Then, delete the file `ready_to_be_removed`
```
root@a710280214ff:~# cd /root
root@a710280214ff:~# ls
empty_directory  new_school  ready_to_be_removed  school  so_cool
root@a710280214ff:~# rm ready_to_be_removed 
root@a710280214ff:~# ls
empty_directory  new_school  school  so_cool
root@a710280214ff:~# 
```



## Resources
- [Linux navigation](https://linuxcommand.org/lc3_lts0020.php)
- [Linux - looking around](https://linuxcommand.org/lc3_lts0030.php)
- [Linux - manipulating files](https://linuxcommand.org/lc3_lts0050.php)
- [Linux - /tmp](https://tldp.org/LDP/Linux-Filesystem-Hierarchy/html/tmp.html)
