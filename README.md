# Week 3 – Password Cracking Project Submission

**Name:** Maryam Batool
**Student ID:** NW-084-980
**Course:** Cybersecurity & Ethical Hacking (Networkwalks)
**Week:** 3 – Project Modules 1 & 2
**Environment used:** Kali Linux (VM)
**Date:** 20 November 2026

## What this submission contains

| Folder / File | Description |
|---|---|
| `Report/` | The full written report (PDF and Word versions). **Open the PDF first** — it explains the background, steps, and results for both modules with screenshots and explanations. |
| `Screenshots/Module1-JTR/PDF1/` | 4 screenshots: hash extraction, John the Ripper cracking the password, xpdf open attempts, and the PDF opened successfully. |
| `Screenshots/Module1-JTR/PDF2/` | 2 screenshots: hash extraction + cracking, and the PDF opened successfully. |
| `Screenshots/Module1-JTR/PDF3/` | 2 screenshots: hash extraction + cracking, and the PDF opened with the captured flag. |
| `Screenshots/Module2-NWTools/` | 3 screenshots: Networkwalks Password Cracker finding the password, an xpdf open attempt, and the PDF opened with the captured flag. |

## Summary of Results

| # | File | Tool Used | Recovered Password | Status |
|---|------|-----------|--------------------|--------|
| 1 | My Locked PDF1.pdf | John the Ripper (`pdf2john` + `john`) | `good-luck` | Cracked |
| 2 | My Locked PDF2.pdf | John the Ripper (`pdf2john` + `john`) | `password1` | Cracked |
| 3 | My Locked PDF3.pdf | John the Ripper (`pdf2john` + `john`) | `1qaz2wsx` | Cracked |
| 4 | My Locked PDF1 (for NW Tools Lab WK3-PM2).pdf | Networkwalks Hash Calculator + Password Cracker | `password1` | Cracked |

## How the work was done (short version)

**Module 1 – JTR (Kali Linux):**
For each locked PDF, the hash was extracted with `pdf2john`, then cracked with `john` using the built-in wordlist or `rockyou.txt`. The recovered password was used to open the PDF in `xpdf` to confirm it and capture the flag.

**Module 2 – Networkwalks Tools:**
The PDF was uploaded to the Networkwalks Hash Calculator to extract its `$pdf$` hash, which was then pasted into the Networkwalks Password Cracker to run a dictionary attack. The recovered password was used to open the PDF and capture the flag.

Full step-by-step details, explanations, and all screenshots (with captions) are in the report inside the `Report/` folder.
