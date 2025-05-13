# Hill Cipher Encryption

This project encrypts alphabetic characters from a plaintext file using the Hill cipher algorithm. The encryption key is provided as an n × n matrix, where the Hill matrix can be any size from 2x2 up to 9x9. The program accepts two command-line arguments: the first is the path to the encryption key file, and the second is the path to the plaintext file. It processes the input by converting all letters to lowercase, removing non-alphabetic characters, and padding the message with the letter 'x' to ensure the message length aligns with the matrix size. The final ciphertext is converted to uppercase and printed directly to the console.

# Features
Encrypts text using the Hill cipher with a matrix size between 2×2 and 9×9.

# Cleans and prepares the input by:

Converting all letters to lowercase.

Removing all non-letter characters (e.g., numbers, symbols, whitespace).

Padding the plaintext with the letter 'x' to match the required block size.

Reads encryption matrix and plaintext from specified files.

# Outputs:

The encryption matrix.

The cleaned and padded plaintext.

The resulting ciphertext in uppercase, printed to the console.

# File Input Specifications
Encryption Key File:

The first line contains a single integer n (between 2 and 9), indicating the dimension of the square key matrix.

The next n lines each include n space-separated integers, representing the matrix values in row-major order.

Plaintext File:

The message file can include both letters and non-letter characters. 

The encryption process will:

Use only alphabetic characters.

Convert all letters to lowercase.

Exclude punctuation, digits, and whitespace from encryption.

# Program Output
The program displays:

The encryption matrix used in processing.

The filtered and padded plaintext, showing exactly what will be encrypted.

The resulting ciphertext in uppercase, printed in lines no longer than 80 characters for readability.

# Compiling and Running:

To Compile: gcc -o pa01 pa01.c

To Execute: ./pa01 kX.txt pX.txt

            (Where kX.txt is the keytext file, and pX.txt is the plaintext file)

# Development Environment: MobaXterm, Eustis, and Bash
This program was developed and executed remotely using MobaXterm, a Windows-based terminal with SSH support.

The code was compiled and run on Eustis, the university’s remote Unix server.

The Bash shell was used for all command-line operations, including compiling the C program, navigating files, and running the executable.

# Workflow:

Connected to Eustis via SSH using MobaXterm.

Uploaded the source code and input files using MobaXterm’s SFTP interface.

Used Bash commands on the remote terminal to compile (gcc) and run the program.

Output was displayed directly in the terminal, and debugging was also done through Bash.
