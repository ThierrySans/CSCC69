---
layout: default
permalink: /tutorials/10/
---

There are two parts in project 4:

1. Indexed and Extensible Files
2. Subdirectories

During the lecture we have seen that:
- the file systems is logically divided into units called blocks
- the disk is physically divided into units called sectors (that are always 512 bytes) 

In Pintos (like in the original Unix file system), things are simple: 1 block = 1 sector = 512.

However, modern Operating systems define block size of 4 KB or 8 KB. 

1. What is an inode?

2. Given an inode, how to find the blocks that hold the data? 

3. What are bitmaps?

4. How do we set the nth bit in a bitmap?

5. How do we unset the nth bit in a bitmap?
    
6. How do we toggle the nth bit in a bitmap?
   
7. What is a bitmask?

8. In the orignal Pintos design, the file's data is stored in contiguous data blocks (the inode stores the pointer to the first block and the total file size). What are the two majors drawbacks of this design? 

9. According to the Pintos documentation, what is the solution to resolve the problems encountered in question 6? 

10. Considering a design with only one double indirect block pointer? What is the largest file size that you could store? 

11. Why having direct and single indirect blocks when a double indirect can store that much data? 
