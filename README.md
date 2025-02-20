# Image Steganography using OpenCV

## Overview
This project implements a simple image steganography technique using OpenCV in Python. The program hides a secret message inside an image by encoding the ASCII values of characters into the pixel values. The message can be retrieved later by using the correct passcode.

## Features
- Encrypt a secret message into an image.
- Decrypt the message using the correct passcode.
- Uses OpenCV to manipulate pixel values for encoding and decoding.

## Requirements
Ensure you have the following installed:
- Python 3.x
- OpenCV (`cv2`)

You can install OpenCV using:
```bash
pip install opencv-python
```

## How It Works
### Encryption
1. The user inputs a secret message.
2. The program modifies the pixel values of an image to store the message.
3. The modified image is saved as `encryptedImage.jpg`.

### Decryption
1. The user enters the passcode.
2. If the passcode matches the encryption passcode, the hidden message is extracted.
3. The decoded message is displayed.

## Usage
### Running the Script
1. Place an image (e.g., `Prabhas.jpg`) in the project directory.
2. Run the script:
   ```bash
   python steganography.py
   ```
3. Enter a secret message and a passcode when prompted.
4. The encoded image (`encryptedImage.jpg`) is saved.
5. To decrypt, enter the correct passcode when prompted.

## Notes
- The script modifies pixel values directly to store data.
- It currently assumes the message length is known during decryption.
- The encryption method is simple and does not use advanced cryptographic techniques.
