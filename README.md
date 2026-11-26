# 🛡️ StegoGuard – Image Forensics Lab

Automated steganography detection using **GitHub Actions** and **Python**.

## 📌 Overview
StegoGuard scans PNG images for hidden data on every commit.  
If suspicious data is found, the workflow **fails** automatically.

## 📂 Project Files
| File | Purpose |
|------|---------|
| `lab_mode.txt` | Switch between `clean` and `suspicious` |
| `make_demo_image.py` | Creates a demo PNG (adds hidden text in suspicious mode) |
| `scanner.py` | StegoGuard scanner |
| `.github/workflows/stegoguard.yml` | GitHub Actions workflow |
| `student_note.txt` | Student note |

## 🔍 What StegoGuard Detects
1. Invalid file signatures
2. Extra data after the PNG `IEND` ending marker
3. Suspicious keywords inside file bytes

## ⚙️ How It Works
1. Edit `lab_mode.txt`
2. GitHub Actions starts automatically
3. Python creates a demo PNG image
4. StegoGuard scans the image
5. ❌ Hidden data found → workflow fails
6. ✅ No hidden data → workflow passes

## 🧪 My Custom Rules
- Added keyword: `confidential`
- Added keyword: `private`

## ⚠️ Safety Note
This project is for **educational and defensive cybersecurity** only.  
All hidden data used is harmless demo text.

---
👤 **Student:** Dhalee MD Srijon
