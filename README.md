# Week 3: Password Cracking & Hash Extraction Lab

## 📌 Project Overview
This repository documents the completion of Week 3 essential modules for the Networkwalks Cybersecurity & Ethical Hacking Internship, covering cryptographic hash extraction and offline dictionary-based password recovery across all provided target files[cite: 69, 72].

- **Modules Completed:**
  - **W3-PM1:** Password Cracking with John the Ripper (JTR) on Kali Linux (`My Locked PDF1.pdf`, `My Locked PDF2.pdf`, and `My Locked PDF3.pdf`)[cite: 69, 80]
  - **W3-PM2:** Password Cracking with Networkwalks Browser Tools (`My Locked PDF1 (for NW Tools Lab WK3-PM2).pdf`)[cite: 69, 72, 73]

---

## 🛠️ Tools Used
| Tool | Platform | Purpose |
| :--- | :--- | :--- |
| **Networkwalks Hash Calculator** | Web Browser | Extract `$pdf$` cryptographic hashes from password-protected PDFs[cite: 72] |
| **Networkwalks Password Cracker** | Web Browser | Perform dictionary-based hash matching to recover plaintext passwords[cite: 72, 76] |
| **pdf2john** | Kali Linux CLI | Convert encrypted PDF metadata into John the Ripper compatible hash strings |
| **John the Ripper (JTR)** | Kali Linux CLI | Execute offline dictionary/wordlist attacks against extracted hashes[cite: 80] |

---

## 🔍 Execution Summary

### 1. Module W3-PM2: Networkwalks Browser Tools
1. Uploaded `My Locked PDF1 (for NW Tools Lab WK3-PM2).pdf` to the Networkwalks Hash Calculator to extract the `$pdf$` hash[cite: 73, 74].
2. Submitted the hash to the Networkwalks Password Cracker using the built-in wordlist[cite: 75, 76].
3. Recovered the plaintext password and unlocked the document to verify flag capture[cite: 77, 78].

### 2. Module W3-PM1: John the Ripper (Kali Linux)
1. Extracted the hashes from `My Locked PDF1.pdf`, `My Locked PDF2.pdf`, and `My Locked PDF3.pdf` using `pdf2john`[cite: 80].
2. Executed `john` to recover the passwords via offline dictionary attack[cite: 80].
3. Verified all plaintext passwords with `john --show` and unlocked all three target PDFs[cite: 91, 92, 93].

---

## 📸 Lab Evidence & Screenshots

### Module W3-PM2 Evidence
#### 1. Hash Extraction (Networkwalks Hash Calculator)

<img width="959" height="441" alt="Screenshot 2026-11-21 200633" src="https://github.com/user-attachments/assets/48b9d2e6-d7c0-4c20-9955-2a2d781f193c" />

#### 2. Dictionary Attack Result (Networkwalks Password Cracker)

<img width="959" height="434" alt="Screenshot 2026-11-21 200858" src="https://github.com/user-attachments/assets/60c1fe08-870c-43d5-a979-e919d0a3bbf3" />


#### 3. Unlocked Target PDF (Flag Verification)

<img width="958" height="395" alt="Screenshot 2026-11-21 201144" src="https://github.com/user-attachments/assets/d3edf4eb-c49f-4429-8f20-5cfa8688d1da" />


---

### Module W3-PM1 Evidence
#### 4. Kali Linux Terminal (`pdf2john` & `john` Output for PDF1, PDF2 & PDF3)

<img width="959" height="434" alt="Screenshot 2026-11-21 202451" src="https://github.com/user-attachments/assets/83ba5a9a-3228-47dd-8a05-5cbfeaea32c3" />
<img width="959" height="289" alt="Screenshot 2026-11-21 203034" src="https://github.com/user-attachments/assets/9a3bd3c1-5a39-4ca3-bceb-dd53af5845b2" />
<img width="959" height="249" alt="Screenshot 2026-11-21 203725" src="https://github.com/user-attachments/assets/26e1268e-8e68-4493-bc9d-3474273ade29" />


#### 5. Unlocked Target PDF (`My Locked PDF1.pdf`)

<img width="959" height="389" alt="Screenshot 2026-11-21 202410" src="https://github.com/user-attachments/assets/e1b3822c-62b9-42ff-aa57-f71ada689e6b" />


#### 6. Unlocked Target PDF (`My Locked PDF2.pdf`)

<img width="959" height="425" alt="Screenshot 2026-11-21 203151" src="https://github.com/user-attachments/assets/6887d51b-9e94-4e88-b9bb-0a9ae0e2b210" />


#### 7. Unlocked Target PDF (`My Locked PDF3.pdf`)

<img width="959" height="431" alt="Screenshot 2026-11-21 203640" src="https://github.com/user-attachments/assets/a5263829-8fe4-42a1-9910-6ae35eb23ae1" />

---

## 🔧 Troubleshooting Experience
- **Issue:** File names containing spaces (such as `My Locked PDF1.pdf`) caused argument parsing errors when passed directly to `pdf2john` in the Linux terminal.
- **Resolution:** Enclosed the file paths in double quotes (`"My Locked PDF1.pdf"`) so the shell interpreted each full filename as a single argument.

---

## ⚖️ Disclaimer
All password recovery exercises were conducted strictly on authorized educational lab files provided by Networkwalks for learning purposes[cite: 68, 71].
