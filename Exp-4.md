# Analyzing Email Headers and Detecting Email Spoofing using MHA

## Aim
To examine email headers using the **Message Header Analyzer (MHA)** tool in order to detect signs of email spoofing, phishing, or suspicious sender activity.

---

## Description
Every email comes with a hidden **header** that contains technical details such as the sender’s IP address, mail servers involved, timestamps, and authentication checks (SPF, DKIM, DMARC).  

Attackers often forge these headers to make emails look like they come from trusted sources — this is called **email spoofing**.  
By analyzing headers with the **MHA tool** (such as Microsoft’s [Message Header Analyzer](https://mha.azurewebsites.net/) or Outlook’s built-in MHA add-in), investigators can trace the real source and check for red flags.

---

## Tools Required
- **Message Header Analyzer (MHA)**  
  - Online tool: [https://mha.azurewebsites.net/](https://mha.azurewebsites.net/)  
  - Or Microsoft Outlook Add-in (if using Outlook)  
- A sample email suspected of spoofing (with headers)  
- Computer with internet access  

---

## Procedure
1. **Get the Full Email Header**  
   - In Gmail: Open the email → Click **More (⋮)** → **Show Original**.  
   - In Outlook: Right-click email → **View Message Options** → Copy the header text.  
   - In Yahoo/others: Look for “View Raw Message” or “Full Header”. 
![alt text](<Screenshots/exp4/Screenshot (2).png>)    

2. **Open MHA Tool**  
   - Go to [Message Header Analyzer](https://mha.azurewebsites.net/).
 ![alt text](<Screenshots/exp4/Screenshot (1).png>)    
   - Paste the copied email header into the input box.  
   - Click **Analyze**. 
 ![alt text](<Screenshots/exp4/Screenshot (3).png>)  

3. **Review Results**  
   - MHA displays key information such as:  
     - **From / To / Subject / Date** (basic info)  
     - **Received lines** (mail server hops with IP addresses and timestamps)  
     - **SPF/DKIM/DMARC status** (authentication results) 
![alt text](<Screenshots/exp4/Screenshot (4).png>) 

4. **Detect Email Spoofing Clues**  
   - Check if **“From” domain matches the “Received” server**.  
   - Look at SPF/DKIM/DMARC:  
     - Pass = sender is authentic.  
     - Fail = possible spoofing attempt.  
   - Look for mismatched domains (e.g., claiming from `paypal.com` but actual server is `randommail.ru`).  
   - Check unusual sending IPs (suspicious countries or blacklisted IPs).  
![alt text](<Screenshots/exp4/Screenshot (2.1).png>)
![alt text](<Screenshots/exp4/Screenshot (7).png>)

5. **Document Findings**  
   - Note down suspicious fields, IP addresses, and failed authentication checks.  
![alt text](<Screenshots/exp4/Screenshot (5).png>)
  

---

## Outcome
By following these steps, you can **analyze an email’s true origin and detect spoofing attempts** using the **MHA tool**.  
This helps in identifying phishing attacks, preventing fraud, and strengthening cybersecurity awareness.
