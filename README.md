# AES-Key-Dependent-Dynamic-S-Box

The provided code snippet is from a Java class called AES2 that implements the Advanced Encryption Standard (AES) algorithm. Here's a breakdown of the code:
Key Initialization:

[Springer Link](https://link.springer.com/chapter/10.1007/978-981-19-7753-4_8 "Publication of this project")

## AES Encryption/Decryption in Java

**Features:**

* Implements the Advanced Encryption Standard (AES) for encryption and decryption.
* Supports 128-bit keys.
* Utilizes a pre-computed S-Box for non-linear data substitution.
* Performs various round-based operations for enhanced security.

**Functionality:**

* **Key Initialization:**
    * Takes a byte array as the key.
    * Sets internal variables like state matrix, expanded key, and round parameters.
* **Encryption/Decryption:**
    * `cipher`: Encrypts input data (2D byte array) through multiple rounds of:
        * Adding round key.
        * Substituting bytes using the S-Box.
        * Shifting rows of the state matrix.
        * Mixing columns within the state matrix.
    * `decipher`: Decrypts data using the inverse operations of encryption.
* **S-Box Operations:**
    * `subBytes` and `invSubBytes`: Perform byte substitution based on the pre-defined S-Box table.
    * (Commented) "dynamic S-Box" section offers an alternative approach (not used by default).
* **Other Methods:**
    * `expandKey`: Generates the expanded key from the initial key.
    * `shiftRows`, `mixColumns`, `invShiftRows`, `invMixColumnas`: Handle specific byte manipulations within the state matrix during encryption/decryption rounds.

**Benefits:**

* Provides secure and efficient AES implementation for 128-bit data.
* Offers clear separation of key initialization, encryption/decryption, and internal operations.
* Includes commented sections for further exploration and understanding.

**Note:**

This is a concise overview for a README file. For detailed instructions and code explanations, please refer to the complete source code.

