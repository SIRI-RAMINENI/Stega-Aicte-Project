# Steganography Tool

This project is a simple steganography tool that allows users to hide secret messages within images using Python. The tool provides a graphical user interface (GUI) for both encrypting and decrypting messages.

## Features

- **Encrypt a Message**: Embed a secret message into an image file by modifying the least significant bits (LSB) of the image's pixel data.
- **Decrypt a Message**: Retrieve the hidden message from an encrypted image.
- **User-Friendly GUI**: Built using Tkinter for easy interaction.

## Requirements

- Python 3.x
- Pillow (PIL Fork)
- Tkinter (usually comes pre-installed with Python)

## Installation

1. Clone the repository:
git clone https://github.com/SIRI-RAMINENI/Stega-Aicte-Project.git
cd Stega-Aicte-Project

2. Install the required libraries:
pip install pillow


## Usage

  ### Encrypting a Message

  1. Run the encryption script:
  python encrypt.py


  2. In the GUI that opens:
  - Enter your secret message in the text box.
  - Click on "Select Image" to choose an image file (PNG or JPG) where you want to hide your message.
  - Click "Encrypt Message" to save the encrypted image as `encryptedImage.png`.

  ### Decrypting a Message
  
  1. Run the decryption script:
      python decrypt.py
  
  2. In the GUI that opens:
  - Click on "Select Encrypted Image" to choose the previously encrypted image.
  - The hidden message will be displayed in a pop-up window.

## Important Notes

- The tool currently supports PNG and JPG images.
- Ensure that your input images are large enough to accommodate your secret messages; otherwise, you may encounter issues with longer messages.
- The delimiter used to indicate the end of the hidden message is `1111111111111110`.

## Acknowledgments

- This project utilizes the Pillow library for image processing.
- Special thanks to [Tkinter](https://docs.python.org/3/library/tkinter.html) for providing a simple way to create GUIs in Python.
