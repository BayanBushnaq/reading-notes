# Encryption, decryption, and cracking

## what is Encrypting a message ?
### Encryption converts data into scrambled text. The unreadable text can only be decoded with a secret key. The secret key is a number that's: Created on your device and the device you message.


### One of the earliest encryption techniques is the Caesar Cipher, invented by Julius Caesar more than two thousand years ago to communicate messages to his allies.


## what is Decrypting a message ?
### Decryption is the process of converting an encrypted message back to its original (readable) format. The original message is called the plaintext message. The encrypted message is called the ciphertext message.


## What are the three main methods for cracking a cipher?
- Frequency analysis :
  - Frequency analysis generates an histogram that allows decrypting a text by comparing letters          frequencies in a plain text message with letters frequences in a ciphered message.

- Known plaintext :
  - Known plaintext attack is a scenario in which the attacker has access to pairs of known plaintexts and their corresponding ciphertexts. The goal is to guess the secret key (or a number of secret keys) or to develop an algorithm which would allow him to decrypt any further messages.

- Brute force:
  - A brute force attack against a cipher consists of breaking a cipher by trying all possible keys. Statistically, if the keys were originally chosen randomly, the plaintext will become available after about half of the possible keys are tried.


## A Brief Word on Polymorphism :
### Polymorphism is basically a cipher that changes itself with each use. Meaning that each time it is used, it produces a different set of results. So, if you encrypted the exact same set of data twice, each new encryption would be different from the previous one.


## Types of Cryptography:
- Hashing : Hashing is a type of cryptography that changes a message into an unreadable string of text for the purpose of verifying the message’s contents, not hiding the message itself.

- Symmetric Cryptography : This type of cryptography uses a single key to encrypt a message and then decrypt that message upon delivery.

- Asymmetric Cryptography : uses two different keys for encryption and decryption, as opposed to the single key used in symmetric cryptography.

- Key Exchange Algorithms : Unlike other forms of encryption, you are not sharing information during the key exchange. The end goal is to create an encryption key with another party that can later be used with the aforementioned forms of cryptography.

## There are four primary ways that cryptography is implemented in information security. These four applications are called “cryptographic functions”. :
 1- Authentication 
 2- Nonrepudiation
 3- Confidentiality
 4- Integrity


 ## here are a couple of ways that you can implement even more encryption into your life:
 - Download a VPN.
 - Download HTTPS Everywhere.
 - Install BitLocker (for Windows) or FileVault2 (for Mac).




 # How Computers Generate Random Numbers ?

 ## Computers generate random number for everything from cryptography to video games and gambling. There are two categories of random numbers — “true” random numbers and pseudorandom numbers — and the difference is important for the security of encryption systems.

 ## What Random Numbers Are Used For
### Random numbers have been used for many thousands of years. Whether it’s flipping a coin or rolling a dice, the goal is to leave the end result up to random chance. Random number generators in a computer are similar — they’re an attempt to achieve an unpredictable, random result.


### Random number generators are useful for many different purposes. Aside from obvious applications like generating random numbers for the purposes of gambling or creating unpredictable results in a computer game, randomness is important for cryptography.

### Cryptography requires numbers that attackers can’t guess. We can’t just use the same numbers over and over. We want to generate these numbers in a very unpredictable way so attackers can’t guess them. These random numbers are essential for secure encryption, whether you’re encrypting your own files or just using an HTTPS website on the Internet.

## True Random Numbers:
### A TRNG is a function or device based on an unpredictable physical phenomenon, called an entropy source, that is designed to generate non-deterministic data (e.g., a succession of numbers) to seed security algorithms.

## Pseudorandom Numbers:
### Pseudorandom numbers are an alternative to “true” random numbers. A computer could use a seed value and an algorithm to generate numbers that appear to be random, but that are in fact predictable. The computer doesn’t gather any random data from the environment.