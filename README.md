# 🧠 LSB Image Steganography (C Project)

## 📘 Overview
This project implements **Least Significant Bit (LSB) Image Steganography** in **C**, allowing you to **hide (encode)** secret messages within an image file and **retrieve (decode)** them later.

The concept of steganography is to conceal information within another medium so that its presence is not detected. Here, the **least significant bits of the image pixels** are modified to embed secret data, making changes imperceptible to the human eye.

---

## 🚀 Features
- 🔒 **Encode a secret message** into an image file (e.g., `.bmp`).
- 🔍 **Decode the hidden message** from a previously encoded image.
- 🖼️ Supports **24-bit BMP image format**.
- 💡 Detects and validates input image and message files.
- ⚙️ Modular C code structure for readability and maintenance.


---

## ⚙️ How It Works

### **Encoding Process**
1. Reads the input BMP image file.
2. Opens the text file containing the secret message.
3. Modifies the least significant bits (LSBs) of pixel values to store message bits.
4. Saves the output as a new **encoded image file**.

### **Decoding Process**
1. Reads the encoded BMP image.
2. Extracts the bits stored in the LSBs of the pixels.
3. Reconstructs and displays or saves the hidden message.

---

## 🧪 Example Usage

### **Encoding**
```bash
$ ./a.out stego -e beautiful.bmp secret.txt encoded.bmp

## 🧪 Example Usage

### **Decoding**
```bash
$ ./a.out stego -d encoded.bmp decoded.txt



