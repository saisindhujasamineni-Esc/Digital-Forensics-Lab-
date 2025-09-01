# Experimet -2 : Recovering Deleted Files from a Storage Device using TestDisk

## Aim
To recover accidentally deleted or lost files from a storage device (like a USB drive, hard disk, or memory card) using the **TestDisk** tool.

---

## Description
TestDisk is a free and open-source data recovery tool that works on Windows, Linux, and macOS.  
It is mainly designed to recover lost partitions and fix boot issues, but it can also **undelete files** from file systems like FAT, NTFS, and ext2/3/4.  

The best part is that it works from the command line, so it’s lightweight, fast, and doesn’t make changes to your drive unless you confirm them. This makes it safe for forensic or recovery use.

---

## Tools Required
- **TestDisk software** (free download from [https://www.cgsecurity.org](https://www.cgsecurity.org))  
- The storage device (USB, HDD, SSD, memory card, etc.) with deleted files  
- A computer (Windows/Linux/macOS)  
- Another storage device to copy the recovered files into (very important – don’t save back to the same drive!)

---

## Procedure
**Install and Launch TestDisk**  
   - Download TestDisk from the official website.  
   - Extract the files and run `testdisk_win.exe` (for Windows) or run `sudo testdisk` (Linux/Mac). 

**Create/Skip Log File**  
   - When TestDisk starts, it will ask if you want to create a log file.  
   - Choose **[Create]** (or **[No Log]** if you don’t need one).
   ![alt text](<Screenshots/Exp2/Screenshot 2025-09-01 152328.png>)  

**Select the Drive**  
   - Use the arrow keys to highlight the storage device where files were deleted.  
   - Press **Enter**.  

**Choose Partition Table Type**  
   - TestDisk usually detects this automatically (e.g., Intel/EFI GPT).  
   - Confirm and continue. 
![alt text](<Screenshots/Exp2/Screenshot 2025-09-01 152347.png>)  
![alt text](<Screenshots/Exp2/Screenshot 2025-09-01 152355.png>) 
![alt text](<Screenshots/Exp2/Screenshot 2025-09-01 152423.png>)
![alt text](<Screenshots/Exp2/Screenshot 2025-09-01 152432.png>)

**Select Advanced → Undelete**  
   - In the menu, choose **[Advanced] Filesystem Utilities**. 
![alt text](<Screenshots/Exp2/Screenshot 2025-09-01 152843.png>)   
   - Then pick **[Undelete]**.  
   - TestDisk will scan the file system and show a list of deleted files (in red).  

**Recover the Files**  
   - Navigate through the list using arrow keys. 
 ![alt text](<Screenshots/Exp2/Screenshot 2025-09-01 152906.png>)   
   - Highlight the files/folders you want to recover.  
   - Press **C** (uppercase C) to copy them.  

**Choose Destination**  
   - TestDisk will ask for a location to save the recovered files.  
   - **Important:** Always save them to a different drive than the one you’re recovering from, to avoid overwriting.  
![alt text](<Screenshots/Exp2/Screenshot 2025-09-01 152925.png>)
**Finish Up**  
   - Once recovery is done, check the destination folder to make sure your files are restored.  
   - Exit TestDisk by pressing **Q** multiple times.  
![alt text](<Screenshots/Exp2/Screenshot 2025-09-01 153004.png>)
---

## Result
By following this process, you can safely bring back accidentally deleted files using **TestDisk**.  
It’s simple, effective, and works even when other file recovery tools fail — as long as the deleted data hasn’t been overwritten.

