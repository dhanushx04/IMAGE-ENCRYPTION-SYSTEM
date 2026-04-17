# 🔐 Image Encryption System using AES & RSA

## 📌 Overview

The **Image Encryption System** is a secure client-server application designed to protect image data during transmission and storage. It combines **symmetric encryption (AES)** for fast data encryption and **asymmetric encryption (RSA)** for secure key exchange.

This project also integrates **user authentication** and a **Flask-based server** to simulate secure communication between a client and a server.


## 🎯 Objectives

* Ensure confidentiality of image data
* Implement hybrid encryption (AES + RSA)
* Provide secure key exchange mechanism
* Enable authenticated access to the system



## 🧠 Key Concepts Used

* AES (Advanced Encryption Standard)
* RSA (Public Key Cryptography)
* Hybrid Encryption
* Hashing (SHA-256)
* Client-Server Architecture
* REST API using Flask



## ⚙️ Features

* 🔑 User Registration & Login with hashed passwords
* 🖼️ Image encryption using AES algorithm
* 🔐 AES key encryption using RSA
* 🌐 Secure file transfer via HTTP (Flask server)
* 📁 Storage of encrypted files on server
* 🔓 Decryption support for retrieving original image



## 🏗️ Project Structure


image-encryption-system/
│
├── auth.py        # Authentication system (SQLite + hashing)
├── aes.py         # AES encryption & decryption logic
├── rsa.py         # RSA key generation & encryption
├── server.py      # Flask server to receive encrypted data
├── client.py      # Sends encrypted file & key to server
├── main.py        # Main program (integration)
│
├── requirements.txt
├── README.md
└── sample/
    └── input.jpg


## 🛠️ Technologies Used

* **Python**
* **Flask**
* **PyCryptodome**
* **SQLite**
* **Requests Library**



## 🔄 Workflow

1. User registers and logs in securely
2. Image is selected for encryption
3. AES key is generated and used to encrypt the image
4. RSA key pair is generated
5. AES key is encrypted using RSA public key
6. Encrypted image and key are sent to server
7. Server stores encrypted data securely



## 🚀 Installation & Setup



### 2️⃣ Install Dependencies


pip install -r requirements.txt


### 3️⃣ Run the Server


python server.py


### 4️⃣ Run the Client Application

python main.py


## 📦 Requirements


flask
pycryptodome
requests


## 🔐 Security Features

* Passwords stored using **SHA-256 hashing**
* AES used for fast and secure data encryption
* RSA ensures secure key transmission
* Separation of encryption and key handling



## 📸 Example Use Case

This system can be used in:

* Secure image sharing platforms
* Medical image protection
* Military or confidential data transmission
* Cloud storage security systems



## ⚠️ Limitations

* Basic UI (command-line based)
* Localhost server (not deployed)
* Key management can be enhanced
* No database encryption


## 🚀 Future Enhancements

* Add GUI using Tkinter or Web Interface
* Deploy server on cloud (AWS/Heroku)
* Implement HTTPS for secure communication
* Add multi-user support
* Improve error handling and logging


## ⭐ Acknowledgements

* Cryptography concepts from academic coursework
* Python documentation and open-source libraries



