# 0x01. Emacs 

![Shell](https://img.shields.io/badge/Shell-121011?style=flat&logo=gnubash&logoColor=white)
![Editor](https://img.shields.io/badge/Editor-121011?style=flat&logoColor=white)

## Concepts Learnt

- What is Emacs
- Who is Richard Stallman
- How to open and save files
- What is a buffer and how to switch from one to the other
- How to use the mark and the point to set the region
- How to cut and paste lines and regions
- How to search forward and backward
- How to invoke commands by name
- How to undo
- How to cancel half-entered commands
- How to quit Emacs

## Tasks
### 0. Create your answer directory

Navigate to `/root` and create a directory named `0x01_emacs`
```
bash: cd: root: No such file or directory
root@a710280214ff:~# cd /root
root@a710280214ff:~# mkdir 0x01_emacs
root@a710280214ff:~# ls
0x01_emacs  new_school  school  school_is_amazing  so_cool
root@a710280214ff:~# 
```

### 1. Opening

What is the command to open a file from within Emacs?

Write the answer into the file `/root/0x01_emacs/opening.`
```
root@a710280214ff:~# cd 0x01_emacs/
root@a710280214ff:~/0x01_emacs# echo "C-x C-f" > opening
root@a710280214ff:~/0x01_emacs# cat opening 
C-x C-f
root@a710280214ff:~/0x01_emacs# 
```

### 2. Saving

What is the command to save a file?

Write the answer into the file `/root/0x01_emacs/saving`.
```
root@a710280214ff:~/0x01_emacs# echo "C-x C-s" > saving
root@a710280214ff:~/0x01_emacs# cat saving 
C-x C-s
root@a710280214ff:~/0x01_emacs# 
```

### 3. Cutting

What is the command to cut an entire line?

Write the answer into the file `/root/0x01_emacs/cutting`
```
root@a710280214ff:~/0x01_emacs# echo "C-k" > cutting
root@a710280214ff:~/0x01_emacs# cat cutting 
C-k
root@a710280214ff:~/0x01_emacs# 
```

### 4. Pasting

What is the command to paste?

Write the answer into the file `/root/0x01_emacs/pasting`.
```
root@a710280214ff:~/0x01_emacs# echo "C-y" > pasting
root@a710280214ff:~/0x01_emacs# cat pasting 
C-y
root@a710280214ff:~/0x01_emacs# 
```

### 5. Searching

What is the command to search forward?

Write the answer into the file `/root/0x01_emacs/searching`.
```
root@a710280214ff:~/0x01_emacs# echo "C-s" > searching
root@a710280214ff:~/0x01_emacs# cat searching 
C-s
root@a710280214ff:~/0x01_emacs# 
```

### 6. Undoing
What is the command to undo?

Write the answer into the file `/root/0x01_emacs/undoing`.
```
root@a710280214ff:~/0x01_emacs# echo "C-x-u" > undoing
root@a710280214ff:~/0x01_emacs# cat undoing 
C-x-u
root@a710280214ff:~/0x01_emacs# 
```

### 7. Quitting

What is the command to quit Emacs?

Write the answer into the file `/root/0x01_emacs/quitting`.
```
root@a710280214ff:~/0x01_emacs# echo "C-x C-c" > quitting
root@a710280214ff:~/0x01_emacs# cat quitting 
C-x C-c
root@a710280214ff:~/0x01_emacs# ls
cutting  opening  pasting  quitting  saving  searching  undoing
root@a710280214ff:~/0x01_emacs# 
```
## Resources
- [The Framework](./framework.pdf)
- [Shell](./shell.pdf)
- [A Guided Tour of Emacs](https://www.gnu.org/software/emacs/tour/)

