# Python_Encryption_Decryption

## Overview

This is a simple GUI application for text encryption and decryption using a predefined password. This application is built with Python and Tkinter and leverages Base64 encoding for encryption.

## Features

- Encrypt text with a secret key.
- Decrypt text with a secret key.
- Reset the input fields.

## How It Works

### Main Screen

- Text Input: Enter the text you want to encrypt or decrypt.
- Password Input: Enter the secret key (password) for encryption and decryption.
- Buttons:
  - ENCRYPT: Encrypts the entered text using Base64 encoding.
  - DECRYPT: Decrypts the entered text using Base64 decoding.
  - RESET: Clears the text and password fields.

### Encryption:

- Enter the text in the provided text box.
- Enter the secret key (1234).
- Click ENCRYPT.
- A new window will display the encrypted text.

### Decryption:

- Enter the encrypted text in the provided text box.
- Enter the secret key (1234).
- Click DECRYPT.
- A new window will display the decrypted text.

### Reset:

- Clears the text input and password fields to start fresh.


## Code Explanation:

### Imported Libraries:
- tkinter: Used for the graphical user interface.
- messagebox: For displaying error messages.
- base64: For encoding and decoding text.
- os: For OS-related tasks (not used in this script).

### Main Functions:

- decrypt(): Decrypts the entered text if the password is correct.
- encrypt(): Encrypts the entered text if the password is correct.
- main_screen(): Sets up the main application window and its elements.

### Encryption and Decryption Logic

- Encoding: Converts the text to ASCII, encodes it using Base64, and then converts it back to a string.
- Decoding: Converts the encoded text to ASCII, decodes it using Base64, and then converts it back to a string.

### Password Validation

- Only the password 1234 is accepted for both encryption and decryption.
- Displays an error message if the password is incorrect or missing.

### Notes

- The secret key is hardcoded as 1234 for both encryption and decryption.
- The application uses Base64 encoding, which is not secure for serious encryption needs. For stronger encryption, consider using libraries like cryptography.

### Example

- Open the application.
- Enter "Hello World" in the text box.
- Enter "1234" as the password.
- Click ENCRYPT to see the encrypted text.
- Copy the encrypted text, clear the text box, and paste the encrypted text.
- Enter "1234" as the password again.
- Click DECRYPT to see the original text.
