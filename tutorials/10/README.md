---
layout: default
permalink: /tutorials/10/
---

There are three parts in project 4:

1. Indexed and Extensible Files
2. Subdirectories
3. Buffer Cache

The handout recommends to start with part 3 first about the file system buffer cache. Managing the buffer cache is very similar to managing the virtual memory (by using the clock algorithm to manage cached blocks). So even if there is quite a lot of code to write for this part, you should be able to get done with it quite quickly since the design is very similar to what you have done for project 3.

During the lecture we have seen that:
- the file systems is logically divided into units called blocks
- the disk is physically divided into units called sectors (that are always 512 bytes) 

In Pintos (like in the original Unix file system), things are simple: 1 block = 1 sector = 512.

However, modern Operating systems define block size of 4 KB or 8 KB. 

1. What is an inode?

2. Given an inode, how to find the blocks that hold the data? 

3. What is a buffer cache and how does it things more efficient?

4. What is the max number of sectors for a buffer cache?

5. So what is the total capacity of the buffer cache partition? 

6. How does the bounce buffer in `inode.c` in the functions `inode_read_at` and `inode_write_at` work?

7. What is write-behind?

8. What is read-ahead?

9. Why should we do read-ahead asynchronously?

10. [Exam] What is the difference between a memory-mapped file and a file in the buffer cache? What advantages each solution provides? Can you use both or are they mutually exclusive?