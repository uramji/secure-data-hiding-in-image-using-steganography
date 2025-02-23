# secure-data-hiding-in-image-using-steganography
# Image-Based Steganography

This repository contains a simple **image-based steganography** implementation using Python and OpenCV. It allows you to **hide a secret message** inside an image and later **retrieve it** using a passcode.

## Features
- Hides a secret message inside an image by modifying pixel values.
- Extracts the hidden message from the encrypted image.
- Uses a passcode to prevent unauthorized access.

## Requirements
Make sure you have the following dependencies installed:

```bash
pip install opencv-python
```

## Usage

### Encryption (Hiding a Message)
This script embeds a secret message into an image by modifying its pixel values.

```python
python encrypt.py
```
**Steps:**
1. Enter the secret message.
2. Enter a passcode for protection.
3. The encrypted image is saved as `encryptedImage.jpg`.

### Decryption (Retrieving the Message)
This script extracts the hidden message from the encrypted image.

```python
python decrypt.py
```
**Steps:**
1. Enter the passcode used during encryption.
2. If the passcode is correct, the hidden message is displayed.

## Files
- `encrypt.py` - Script to hide a message inside an image.
- `decrypt.py` - Script to extract the hidden message.
- `godshiva.jpg` - Sample image for testing.

## Notes
- The passcode is only used for authentication, **not encryption**. Future improvements could involve encrypting the message before embedding.
- Ensure the message length does not exceed the image capacity.
- The script modifies pixel values directly, which may introduce noticeable changes to the image.
- For better security and minimal distortion, consider **LSB (Least Significant Bit) encoding** or **AES encryption** before embedding.

## License
This project is open-source and available under the **MIT License**.

## Contributions
Feel free to submit issues or pull requests for improvements!

---
### Author: [U RAMA RAO]  
GitHub: [uramji]

