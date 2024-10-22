
# Note: Due to the potential for misuse, I can not share this source code publicly on GitHub or LinkedIn.

# 🛡️ Browser Password Extractor and Cleaner

![Project Logo](https://img.shields.io/badge/Browser-Password%20Extractor-blueviolet)  
A Python tool that extracts and optionally deletes saved passwords from popular browsers like **Google Chrome**, **Microsoft Edge**, and **Mozilla Firefox**. This tool is designed for penetration testers, security enthusiasts, and anyone interested in understanding browser security mechanisms.

## 📋 Table of Contents
- [Features](#-features)
- [Requirements](#-requirements)
- [Installation](#-installation)
- [Usage](#-usage)
- [Demo](#-demo)
- [Disclaimer](#-disclaimer)
- [License](#-license)

## ✨ Features
- Extract saved passwords from Google Chrome, Edge, and Firefox.
- Decrypt stored passwords using Chrome's and Edge's internal encryption.
- Optionally delete all saved passwords for a clean slate.
- Auto-install dependencies on the first run for easy setup.

## ⚙️ Requirements
- **Python 3.6+** installed.
- Compatible with Windows OS.
- **Google Chrome**, **Microsoft Edge**, or **Mozilla Firefox** installed.

## 📦 Installation
Clone this repository and navigate to the project folder:
```bash
git clone https://github.com/cyberprogramming1/Browser-Password-Extractor.git
cd Browser-Password-Extractor
```

Ensure Python is installed and available in your system's PATH.

## 🚀 Usage
The script automatically installs dependencies on the first run. Follow these steps:

1. **Run the Script**:  
   ```bash
   python Browser-Password-Extractor.py
   ```
   
2. **Extract and View Passwords**:  
   The passwords will be saved to a `chrome_data.txt` file.

3. **Delete All Passwords (Optional)**:  
   Follow the on-screen instructions to delete passwords after extraction.

## 🛠️ Code Overview
Below is a breakdown of the key parts of the code:

### Extracting Passwords
```python
def main():
    # Decrypt stored passwords
    key = get_encryption_key()
    ...
    password = decrypt_password(row[3], key)
    ...
```

### Deleting Passwords (Optional)
```python
def delete_passwords():
    # Deleting saved passwords from browsers
    db_path = os.path.join(os.environ["USERPROFILE"], "AppData", "Local",
                           "Google", "Chrome", "User Data", "default", "Login Data")
    ...
```


## 📜 Disclaimer
This tool is intended for educational purposes only. Unauthorized access to someone else’s data is illegal and unethical. Always obtain permission before attempting to access or manipulate any data that isn't your own.

# Important Note
1. Ethical Use: This script should be used responsibly and ethically. Ensure you have permission to access the password data and do not use this script for malicious purposes.
2. Data Loss Warning: Deleting passwords is irreversible. Use caution when using the delete feature.



**Follow Me on [LinkedIn](https://www.linkedin.com/in/raul-yarmemmedov/) | Check the Code on [GitHub](https://github.com/cyberprogramming1/Browser-Password-Extractor)**
