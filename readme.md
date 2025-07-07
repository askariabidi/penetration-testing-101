# PT2025 – B032431 (B255) - PENETRATION TESTING 2024-2025 - Exam Submission

This repository contains the complete work submitted for the **B032431 (B255) - PENETRATION TESTING 2024-2025** conducted in July 2025 at the University of Florence. The project demonstrates hands-on penetration testing on a deliberately vulnerable web application using Docker, with documentation aligned to course guidelines.

---

## 🗂️ Contents

- `Assignment-July-2025.pdf` – Original assignment guidelines  
- `Final-Report.pdf` – Final report with documented vulnerability and analysis  
- `Report-Template.docx` – Supporting Word version of the report
- `course-material` – All the slides & pdfs provided by the professor 

---

## 🛠️ Test Environment Setup

1. **Operating System**: Windows 11  
2. **Environment**: Docker container using the image `gabrielec/ptexam2`  
3. **Command Used**:

```bash
docker run -dit -p 8080:80 --name ptexam2 gabrielec/ptexam2
```

This runs the vulnerable application locally on [http://localhost:8080](http://localhost:8080)

---

## 🕵️‍♂️ Performed Attack

- **Vulnerability**: SQL Injection  
- **Target Endpoint**: `/login.php`  
- **Payload Used**: `' OR '1'='1`  
- **Result**: Bypassed authentication and accessed protected area  

---

## 🧾 Report Structure

The report follows the M12 Report structure taught in class:

- Executive Summary  
- Methodology (Black-box testing)  
- Vulnerability Discovery  
- Proof of Concept  
- Risk Assessment (CVSS 9.8)  
- Suggested Mitigation  
- Tools Used  

---

## 🧰 Tools Used

- Docker  
- Brave Browser  
- Manual SQL Injection  
- Online MD5 hash crackers  
- Burp Suite (optional)  

---

## 🔐 Notes

- The goal was to confirm **at least one vulnerability** with PoC.  
- The SQLi attack was sufficient to demonstrate the impact.  

---

## 👨‍🏫 Course & Instructor

**Course**: B032431 (B255) - PENETRATION TESTING 2024-2025  
**Instructor**: Prof. Costa Gabriele  
**University**: University of Florence  

---

## 👤 Author

**Syed Mohammad Askari Abidi**  
University of Florence – Master’s in Software: Science and Technology  
Email: syed.abidi@edu.unifi.it
