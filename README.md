# String Content Classifier (C++)

This C++ program is designed to process and filter text input. It takes a string of up to 80 characters and separates its content into two distinct buffers: one for numeric digits and another for all other symbols (letters, spaces, punctuation).

###  Logic & Implementation
The application treats the input as a character array (C-string) and performs a single-pass scan to categorize each element.

**Classification Criteria:**
* **Numbers:** Characters $c$ where `isdigit(c)` is true (ASCII values $48$ to $57$).
* **Other Symbols:** Any character $c$ that does not satisfy the digit condition.



The program utilizes safe string functions like `strncat_s` to prevent buffer overflows, ensuring that the filtered data remains within the allocated memory bounds.

###  Key Features
* **Safe Buffer Handling:** Implements `strncat_s` and `cin.getline` to manage a fixed-size buffer of 81 bytes (80 characters + null terminator).
* **Real-time Processing:** Uses `strlen()` to iterate precisely over the length of the entered text.
* **Header Proficiency:** Demonstrates the use of `<cstring>` and `<iostream>` for standard C++ data management.

###  Technical Stack
* **Language:** C++
* **Key Functions:** `isdigit()`, `strncat_s()`, `cin.getline()`.
* **Data Structures:** Character arrays (char arrays).

### How to Use
1. Compile the program using a C++ compiler.
2. Enter a line of text (up to 80 characters).
3. The program will display the "Numbers" and "Others symbols" as separate strings.
