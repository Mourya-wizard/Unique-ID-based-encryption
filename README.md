# Unique-ID-based-encryption

This Python code implements a simple encrypted messaging system that allows users to encrypt and decrypt messages using a receiver's unique ID.

## Encryption

The `encrypt` function takes a receiver's ID and a message as input. It then applies a custom encryption algorithm based on the digits in the receiver's ID to transform the message. Here's a brief overview of the encryption steps:

- If a digit is '0', it adds special characters to the message.
- If a digit is '1', it duplicates the message.
- If a digit is '2', it inserts a specific emoji at a specific position in the message.
- If a digit is '3', it replaces a portion of the message with emojis.
- If a digit is '4', it adds special characters to the end of the message.
- If a digit is '5', it replaces a portion of the message with special characters.
- If a digit is '6', it inserts a specific symbol at regular intervals in the message.
- If a digit is '7', it replaces characters with special characters at regular intervals.
- If a digit is '8', it inserts a numerical code at a specific position in the message.
- If a digit is '9', it adds a specific emoji at the end of the message.

The encrypted message is then returned.
**Here, each of key value pairs for encryption can be modified based on the developers choice and design their own level of encryption technique based on their choice of algorithms.**

## Decryption

The `decrypt` function reverses the encryption process. It takes the receiver's ID and the encrypted message as input and performs the reverse operations to decrypt the message.

## User Interface

The code provides a simple command-line user interface that allows users to choose between encryption, decryption, or exiting the program. Users can input the receiver's ID and the message they want to send for encryption, and they can also decrypt a received message using the same receiver's ID.

## Usage

1. Run the code, and you will be presented with a menu:
   - Option 1: Encrypt a message
   - Option 2: Decrypt a message
   - Option 3: Exit

2. If you choose to encrypt a message (Option 1), you will be prompted to enter the receiver's ID and the message to be sent. The encrypted message will be displayed.

3. If you choose to decrypt a message (Option 2), you will need to provide the receiver's ID and the encrypted message. The decrypted message will be displayed.

4. You can continue encrypting and decrypting messages or choose to exit the program.
