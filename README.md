# File Encryption & Decryption Tool

A simple Python-based **file encryption and decryption tool** using **Fernet symmetric encryption** from the Python `cryptography` library.

This project allows users to securely encrypt files and decrypt them using a generated secret key.

## Features

- Automatically generates a secret encryption key
- Encrypts files using Fernet encryption
- Decrypts encrypted files
- Handles invalid encryption keys
- Checks whether the requested file exists
- Built entirely with Python

##  Technologies Used

- **Python**
- **Cryptography**
- **Fernet Symmetric Encryption**
- **OS module**

##  Installation

Install the required library:

```bash
pip install cryptography
```

##  How to Run

Run the Python file:

```bash
python encryption.py
```

Choose an operation:

```text
Enter 'E' to encrypt or 'D' decrypt the file:
```

### Encrypt a file

Enter:

```text
E
```

Then provide the file name, including its extension.

Example:

```text
Enter the file name to encrypt: example.txt
```

### Decrypt a file

Enter:

```text
D
```

Then provide the encrypted file name.

The program uses the `Secret.key` file to decrypt the data.

##  Secret Key

The program automatically creates:

```text
Secret.key
```

if it does not already exist.

**Important:** Keep `Secret.key` safe. If the key is lost, encrypted files cannot be decrypted.

 **Do not upload `Secret.key` to GitHub.**

Add it to `.gitignore`:

```text
Secret.key
```

##  Project Structure

```text
File-Encryption-Tool/
│
├── encryption.py
├── README.md
├── .gitignore
└── Secret.key        # Do not upload
```

## How It Works

The program uses **Fernet symmetric encryption**, meaning the same secret key is used for both encryption and decryption.

```text
Original File
     ↓
Fernet Encryption
     ↓
Encrypted File
     ↓
Fernet Decryption
     ↓
Original File
```

##  Disclaimer

This project was created for **educational and cybersecurity learning purposes**.

Always keep backups of important files before testing encryption/decryption tools.

##  Author

**Sahil Jaiswal**

Cybersecurity & Forensics Student
