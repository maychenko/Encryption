# Encryption Tool (C++)

A C++ application for text data encryption and decryption supporting classical cipher algorithms. Designed using Clean Architecture principles to separate core encryption logic, data handling, and user interface components.

---

## Tech Stack & Tools

Language: C++17 / C++20
Build System: CMake / MSBuild (Visual Studio)
Configuration Format: JSON

---

## Project Structure

The codebase is organized into distinct logical layers:

Domain: Core algorithms including XOR and Caesar cipher logic.
Application: High-level orchestration of encryption workflows.
Infrastructure: File system operations and configuration processing via JSON.
UI: Terminal interface for user interaction and options configuration.
Utils & Data: Key management and utility helper functions.

---

## Key Features

Supported Algorithms
XOR Cipher: Symmetric byte-level manipulation using custom encryption keys.
Caesar Cipher: Substitution-based character shifting mechanism.

Configuration Management
Supports dynamic configuration parameters through external config.json settings (UI language, theme colors, and automatic key saving preferences).

---

## Build & Run Instructions

Clone the repository:
git clone https://github.com/maychenko/Encryption.git

Open Encryption.sln in Visual Studio or build via C++ compiler tools, then run the resulting executable file.

## Usage Example

The application operates as an interactive command-line interface. Below is an example execution flow for encrypting and decrypting a message using the Caesar cipher:

1. Select operation mode:
Select mode: [1] Encrypt  [2] Decrypt  [3] Exit
> 1

2. Select algorithm:
Select algorithm: [1] XOR Cipher  [2] Caesar Cipher
> 2

3. Input text and key parameter:
Enter text: Hello World
Enter key shift (integer): 3

Output:
Encrypted Text: Khoor Zruog

4. Decryption flow:
Select mode: [2] Decrypt
Select algorithm: [2] Caesar Cipher
Enter text: Khoor Zruog
Enter key shift (integer): 3

Output:
Decrypted Text: Hello World
