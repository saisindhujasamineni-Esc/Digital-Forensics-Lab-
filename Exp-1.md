# Experiment -1 : Evidence Acquisition using FTK Imager Tool

## Aim
To acquire and preserve digital evidence from storage media using **FTK Imager**, ensuring integrity, accuracy, and admissibility in forensic investigations.

---

## Description
FTK Imager is a forensic imaging tool developed by AccessData. It allows investigators to create forensic images (bit-by-bit copies) of storage media such as hard drives, USBs, and memory cards without altering the original evidence.  
The tool also provides options to verify evidence integrity using cryptographic hash functions (MD5, SHA1, SHA256).  
By using FTK Imager, investigators can securely extract, preview, and analyze data while maintaining forensic soundness.

---

## Tools Required
- **FTK Imager** (AccessData)
- External storage device (to save acquired image)

---

## Procedure
**Install and Launch FTK Imager**  
   - Download and install FTK Imager on the forensic workstation.  
   - Launch the application.
![alt text](<Screenshots/Exp1/Screenshot 2025-08-31 165800.png>)   

**Select Evidence Source**  
   - Go to **File → Create Disk Image**.  
![alt text](<Screenshots/Exp1/Screenshot (45).png>)
   - Choose the source type (Physical Drive, Logical Drive, Image File, Contents of a Folder, etc.).
![alt text](<Screenshots/Exp1/Screenshot (46).png>)  
   - Select the evidence device/media connected to the system.


**Choose Destination and Format**  
   - Select the type of image format (e.g., **E01 (EnCase), Raw (dd), SMART, AFF**).
![alt text](<Screenshots/Exp1/Screenshot (48).png>)     
   - Provide the destination path where the image will be stored.
![alt text](<Screenshots/Exp1/Screenshot (51).png>)     
   - Ensure enough storage space is available.

**Configure Case Information (Optional)**  
   - Enter case details such as Case Number, Examiner Name, and Description for documentation purposes.
![alt text](<Screenshots/Exp1/Screenshot (49).png>)


**Start Acquisition**  
   - Begin the acquisition process.  
   - FTK Imager will create a bit-by-bit copy of the source drive.
![alt text](<Screenshots/Exp1/Screenshot (55).png>)     
   - Progress and logs will be displayed.

**Secure Evidence Storage**  
   - Store the acquired image in a secure external storage device.  
   - Maintain proper chain of custody documentation.

---

## Result
By following this procedure, a forensic examiner can successfully acquire and preserve a forensic image of digital media using **FTK Imager**, ensuring that the evidence is accurate, reliable, and legally admissible.
