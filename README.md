# File Compression Tool using Huffman Coding

## Overview

This project is a desktop-based file compression tool built in Python using the Huffman Coding algorithm. The application reduces the size of text files while ensuring that no information is lost during the compression process.

A graphical interface built with Tkinter allows users to compress and decompress files without using the command line. The tool also displays useful statistics such as original size, compressed size, and compression ratio after processing a file.

---

## Features

- Compress text files using Huffman Coding
- Decompress files back to their original form
- User-friendly GUI built with Tkinter
- Custom `.huf` file format for storing compressed data
- Displays compression statistics
- Handles invalid input and empty files
- Lossless compression (original content is fully restored)

---

## How Huffman Coding Works

The compression process follows these steps:

1. Read the input text file
2. Count the frequency of each character
3. Build a Huffman Tree using a min-heap
4. Generate binary codes for each character
5. Encode the text using generated codes
6. Store encoded data and mapping information in a `.huf` file

For decompression:

1. Read the compressed file
2. Extract stored encoding information
3. Decode the binary data
4. Reconstruct the original file

---

## Technologies Used

- Python
- Tkinter
- Heap Queue (`heapq`)
- File Handling
- Data Structures and Algorithms

---

## Project Structure

```bash
project-folder/
│
├── main.py
├── compressed_files/
├── decompressed_files/
├── README.md
```

---

## Running the Project

### Clone the repository

```bash
git clone https://github.com/your-username/your-repository-name.git
```

### Move into the project directory

```bash
cd your-repository-name
```

### Run the application

```bash
python main.py
```

---

## Output Example

Compression results displayed by the application:

```text
Original Size: 1500 bytes
Compressed Size: 820 bytes
Compression Ratio: 45.33%
```

---

## Time Complexity

| Operation | Complexity |
|------------|------------|
| Frequency Counting | O(n) |
| Heap Construction | O(k) |
| Huffman Tree Building | O(k log k) |
| Encoding | O(n) |
| Decoding | O(n) |

Where:

- `n` = total number of characters
- `k` = number of unique characters

---

## Testing

The application was tested with different text files to verify:

- Correct file compression
- Successful decompression
- Accurate restoration of original content
- Error handling for invalid or empty inputs

The decompressed output matched the original file content, confirming lossless compression.

---

## Future Improvements

Some possible improvements for future versions:

- Support additional file types
- Improve compression efficiency
- Add drag-and-drop functionality
- Display Huffman Tree visualization
- Add progress indicators for large files

---

## Contributors

- Muhammad Taha — Core Compression Logic
- Syed Shaheer Sohail — Decompression and File Handling
- Syed Irfan Raza — GUI Development
- Muhammad Abdullah — Integration and Testing

---

## License

This project is created for educational purposes.
