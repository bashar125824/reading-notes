*[Back to Reaading Notes](/README.md)*

# Files and I/O Streams

---

***When you want to do input or output to a file, you have a choice of two basic mechanisms for representing the connection between your program and the file : Files and Streams .***
 

***Files and I/O Streams are used for writing and reading data on / from syorages , like disk or memory .***
 

***We can use System.IO to interact with files and directories .***
 

# Differences between files and streams
 

**Files** descriptors are represented as objects of type int .


**streams** are represented as FILE * objects .
 

**some commonly used file and directory classes:**

 

- File
- FileInfo
- Directory
- DirectoryInfo
- Path
- and each class has it's functionality .

---

Stream

---

***there is 3 functionalities for streams :***

1. **Reading** from a data structure , like arrays .

2.  **Writing** on a storage .

3.  **Seeking** : Adjusting and editng a stream .

 

***some commonly used stream classes:***

 

- FileStream
- IsolatedStorageFileStream
- MemoryStream
- BufferedStream
- Network stream 

*and other classes .*

 ---

Readers and Writers 

---


*How can we perform reading and writing in streams ?*

***using Readers and Writers .***

***some commonly used stream classes***

 

- Binary Reader and Binary Writer 
- Stream Reader and Stream Writer
- String Reader and String Writer
- Text Reader and Text Writer
- Asynchronous I/O operations

---

# Asynchronous I/O operations

---
 

*If your app is large , and need to be responsive with the user , then you should perform reading / writing data **Asynchronously** .*

 

***Asynch methods :***

 

- CopyToAsync
- FlushAsync
- ReadAsync
- WriteAsync 


 ---



# Compression


***there is 2 processes :***

**Compression** : refering to maintain storage , we reduce size of folders .

**Uncompression** : Extract contents of compressed file .

 

***Some compressing and decompressing files and streams classes :***

- ZipArchive
- ZipFile

*and other classes .*

 ---

# Isolated storage

 ---

- ***Mechanism for adding more safety and isolation  for saved data .***

- ***It'a a useful otion when program has no access for user files .***

