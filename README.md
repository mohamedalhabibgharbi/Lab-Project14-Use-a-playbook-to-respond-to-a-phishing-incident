# 🛡️ Use a Playbook to Respond to a Phishing Incident  
**Google Cybersecurity Professional Certificate – Hands-on Lab**

---

## 📘 Scenario

You are a level-one security operations center (SOC) analyst at a financial services company. Previously, you received a phishing alert about a suspicious file being downloaded on an employee's computer. After investigating the email attachment file's hash, the attachment has already been verified malicious. Now that you have this information, you must follow your organization's process to complete your investigation and resolve the alert.  
Your organization's security policies and procedures describe how to respond to specific alerts, including what to do when you receive a phishing alert.  
In the playbook (attached), there is a flowchart and written instructions to help you complete your investigation and resolve the alert. At the end of your investigation, you will update the alert ticket with your findings about the incident.

---

## 📎 Additional Information

- **Known malicious file hash:**  
  `54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b`

- **Email details:**  
  From: Def Communications `<76tguyhh6tgftrt7tg.su>` `<114.114.114.114>`  
  Sent: Wednesday, July 20, 2022 09:30:14 AM  
  To: `<hr@inergy.com>` `<176.157.125.93>`  
  Subject: Re: Infrastructure Egnieer role  

> Dear HR at Ingergy,  
>  
> I am writing to express my interest in the engineer role posted from the website.  
> There is attached my resume and cover letter. For privacy, the file is password protected. Use the password **paradise10789** to open.  
>  
> Thank you,  
> Clyde West  
>  
> Attachment: filename="bfsvc.exe"

---

## 🧾 Ticket Update

| Ticket ID | Alert Message                                  | Severity | Details                                                          | Ticket Status |
|-----------|------------------------------------------------|----------|------------------------------------------------------------------|---------------|
| A-2703    | SERVER-MAIL Phishing attempt possible download of malware | Medium   | The user may have opened a malicious email attachment or clicked links. | Escalated     |

---

## 📝 Ticket Comments

The alert indicated an employee downloaded and opened a dangerous file from a phishing email.  
There is a mismatch between the sender’s email address (`76tguy6hh6tgftrt7tg.su`), the sender name in the email (`Clyde West`), and the displayed sender company (`Def Communications`). The email contained grammar mistakes in the body and subject.

The attachment, a password-protected file named **bfsvc.exe**, was confirmed as malicious after checking the hash on **VirusTotal**.

Given these findings, the alert severity is marked **Medium**, and I escalated the case to a level-two SOC analyst for further investigation.

---

## ⚠️ Disclaimer

**This scenario is part of a hands-on lab from the Google Cybersecurity Professional Certificate. It is hypothetical and created for training purposes only.**
