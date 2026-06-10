# 🚀 Advanced QR Code Generator using Python

A Python-based QR Code Generator that demonstrates multiple QR code generation techniques, from simple text QR codes to customized QR codes with logos and UPI payment integration.

## 📌 Project Overview

This project showcases the use of the Python `qrcode` library along with `PIL (Pillow)` and `Tkinter` to create different types of QR codes. It is designed as a beginner-friendly project to understand QR code generation and customization.

## ✨ Features

### 1. Basic QR Code Generation

* Generate QR codes from plain text.
* Save generated QR codes as image files.

### 2. URL QR Code Generator

* Convert website links into scannable QR codes.
* Example: WhatsApp Web, ChatGPT, etc.

### 3. Colored QR Codes

* Create customized QR codes with different foreground and background colors.
* Improve visual appearance while maintaining scan functionality.

### 4. UPI Payment QR Code Generator

* Generate QR codes for digital payments.
* Accepts:

  * UPI ID
  * Merchant Name
  * Payment Amount
* Creates a ready-to-scan payment QR code.

### 5. QR Code with Logo

* Embed a logo/image at the center of the QR code.
* Uses high error correction to maintain readability.
* Useful for branding and business applications.

### 6. GUI-Based QR Code Generator

* User-friendly graphical interface built using Tkinter.
* Allows users to:

  * Enter text or URL
  * Select a logo
  * Generate customized QR codes
  * Save QR codes locally

---

## 🛠️ Technologies Used

* Python 3.x
* qrcode
* Pillow (PIL)
* Tkinter
* IPython Display

---

## 📂 Project Structure

```bash
QR-Code-Generator/
│
├── project.ipynb
├── basic_qr.png
├── qr.png
├── colored_qr.png
├── upi_payment_qr.png
├── qr_with_logo.png
├── logo.png
└── README.md
```

## 📦 Installation

### Clone the Repository

```bash
git clone https://github.com/your-username/QR-Code-Generator.git
cd QR-Code-Generator
```

### Install Dependencies

```bash
pip install qrcode[pil]
pip install pillow
```

---

## ▶️ Usage

### Generate a Basic QR Code

```python
import qrcode

data = "Hello World"
img = qrcode.make(data)
img.save("qr.png")
```

### Generate a UPI Payment QR Code

```python
upi_id = "example@upi"
name = "Merchant Name"
amount = 100

upi_link = f"upi://pay?pa={upi_id}&pn={name}&am={amount}&cu=INR"

qr = qrcode.make(upi_link)
qr.save("upi_payment_qr.png")
```

---

## 🎯 Applications

* Contact Sharing
* Website Linking
* Digital Payments
* Business Branding
* Product Packaging
* Event Registration
* Marketing Campaigns

---

## 🔮 Future Enhancements

* QR Code Scanner Integration
* Bulk QR Code Generation
* PDF Export Support
* Database Connectivity
* QR Analytics Tracking
* Web-Based QR Generator using Flask/Django

---

## 📸 Sample Outputs

* Basic QR Code
* Colored QR Code
* UPI Payment QR Code
* QR Code with Logo
* GUI-Based QR Generator

---

## 👨‍💻 Author

Arpit Santra

B.Tech Computer Science Engineering

Passionate about Python Development, Machine Learning, and Real-World Software Projects.

---

## 📜 License

This project is developed for educational and learning purposes.
Feel free to modify and enhance it according to your requirements.
