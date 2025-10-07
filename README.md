# StringToBin

A simple **C# console application** that writes user-input text to a **binary file** and reads it back as both **raw binary** and **decoded text**.

## Features

* Prompts the user for text input
* Validates non-empty input before writing
* Saves text as binary using **ASCII encoding**
* Reads data back dynamically until EOF (no fixed buffer size)
* Displays file contents as **8-bit binary strings**
* Converts the binary back into **human-readable text**
* Uses **safe resource management** with `using` blocks
* Handles errors gracefully with `try/catch`

## How It Works

1. The **program prompts** the user for input text.
2. Input is validated to ensure it is not empty or whitespace.
3. The **WriteFile method**:

   * Creates/overwrites `binaryFile.bin` in the working directory.
   * Encodes the text into bytes using **ASCII**.
   * Writes the bytes to the file.
4. The **ReadFile method**:

   * Opens the file and reads until EOF in chunks.
   * Prints each byte as an **8-bit binary string** (with spaces).
   * Decodes the bytes back into text using **ASCII**.
   * Displays both the binary and text output.

## Getting Started

### Prerequisites

* [.NET SDK 6.0 (or newer)](https://dotnet.microsoft.com/download)
* Basic knowledge of running C# console applications

## License

This project is licensed under the MIT License in its parent directory.