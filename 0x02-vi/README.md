# 0x02. vi 

![Shell](https://img.shields.io/badge/Shell-121011?style=flat&logo=gnubash&logoColor=white)
![Editor](https://img.shields.io/badge/Editor-121011?style=flat&logoColor=white)

## Concept Learnt

- What is vi
- Who is Bill Joy
- How to start and exit vi
- What are the command and insert modes, and how to switch from one to the other
- How to edit text
- How to cut and paste lines
- How to search forward and backward
- How to undo
- How to quit vi

## Tasks
### 0. Create your answer directory

Navigate to /root and create a directory named `0x02_vi`
```bash
root@a710280214ff:/# cd /root
root@a710280214ff:~# mkdir 0x02_vi
root@a710280214ff:~# cd 0x02_vi
root@a710280214ff:~/0x02_vi# 
```

### 1. Inserting

What is the command to insert text before the cursor?

Write the answer into the file `/root/0x02_vi/inserting`.
```bash
root@a710280214ff:~/0x02_vi# echo "<Esc>i" > inserting
root@a710280214ff:~/0x02_vi# cat inserting 
<Esc>i
root@a710280214ff:~/0x02_vi# 
```

### 2. Cutting

What is the command to delete and cut the current line?

Write the answer into the file `/root/0x02_vi/cutting.`

**Tips:**

- [ How to Copy, Cut and Paste ](https://linuxize.com/post/how-to-copy-cut-paste-in-vim/)
```bash
root@a710280214ff:~/0x02_vi# echo "<Esc>dd" > cutting
root@a710280214ff:~/0x02_vi# cat cutting 
<Esc>dd
root@a710280214ff:~/0x02_vi# 
```

### 3. Pasting

What is the command to paste the lines in the buffer into the text after the current line?

Write the answer into the file `/root/0x02_vi/pasting`.
```bash
root@a710280214ff:~/0x02_vi# echo "<Esc>y" > pasting
root@a710280214ff:~/0x02_vi# cat pasting 
<Esc>y
root@a710280214ff:~/0x02_vi# 
```
### 4. Undoing

What is the command to undo what you just did?

Write the answer into the file `/root/0x02_vi/undoing`.
```bash
root@a710280214ff:~/0x02_vi# echo "<Esc>u" > undoing
root@a710280214ff:~/0x02_vi# cat undoing
<Esc>u
root@a710280214ff:~/0x02_vi# 
```

### 5. Exiting

What is the command to quit vi even though latest changes have not been saved for this vi call?

Write the answer into the file `/root/0x02_vi/exiting`.
```bash
root@a710280214ff:~/0x02_vi# echo "<Esc>:q!" > exiting
root@a710280214ff:~/0x02_vi# cat exiting 
<Esc>:q!
root@a710280214ff:~/0x02_vi# 
```

### 6. Beginning of the line

What is the command to move the cursor to the start of the current line?

Write the answer into the file `/root/0x02_vi/beginning_of_the_line`.
```bash
root@a710280214ff:~/0x02_vi# echo "<Esc>0" > beginning_of_the_line
root@a710280214ff:~/0x02_vi# cat beginning_of_the_line 
<Esc>0
root@a710280214ff:~/0x02_vi# 
```

### 7. End of the line

What is the command to move the cursor to the end of the line?

Write the answer into the file `/root/0x02_vi/end_of_the_line`.
```bash
root@a710280214ff:~/0x02_vi# echo "<Esc>$" > end_of_the_line
root@a710280214ff:~/0x02_vi# cat end_of_the_line 
<Esc>$
root@a710280214ff:~/0x02_vi# 
```

## Resources
- [Basic vi Commands]()
