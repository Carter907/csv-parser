# CSV Parser CLI Program

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Usage](#usage)
- [Build Instructions](#build-instructions)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Introduction
This project aims to develop a simple command-line interface (CLI) program in C to parse CSV (Comma Separated Values) files. It will provide basic functionality to read, process, and potentially output data from CSV files.

## Features
- **File Input:** Read data from a specified CSV file.
- **Delimiter Support:** Support comma (`,`) as the default delimiter, with potential for custom delimiter specification.
- **Header Detection:** Optionally detect and handle header rows.
- **Field Extraction:** Extract data from specified columns/fields.
- **Basic Data Processing:** (Future) Potential for simple filtering or transformation of data.
- **Error Handling:** Robust error handling for file operations and malformed CSV data.

## Usage
The program will be executed from the command line.

`./csv_parser [options] <input_file.csv>`

**Example:**
`./csv_parser -c 0,2 -h data.csv` (Extracts columns 0 and 2, assuming a header, from `data.csv`)

### Options
- `-i <file>`: Specify input CSV file.
- `-o <file>`: (Future) Specify output file for processed data.
- `-d <delimiter>`: (Future) Specify a custom delimiter character.
- `-h`: Indicate that the CSV file has a header row.
- `-c <columns>`: Specify comma-separated column indices to extract (e.g., `0,2,3`).

## Build Instructions

### Prerequisites
- GCC (GNU Compiler Collection) or Clang
- Make (for Makefile projects)

### Steps
1. Clone the repository:
   `git clone https://github.com/yourusername/csv-parser.git`
   `cd csv-parser`

2. Build the project:
   `make` (or `gcc -o csv_parser main.c -Wall -Wextra -std=c11`)

3. Run tests (if any):
   `(Future) make test`

## Project Structure
```
.
├── CMakeLists.txt
├── main.c              # Main program logic
├── README.md           # Project documentation
└── .gitignore          # Git ignore file
```

## Contributing
(Future) Guidelines for contributing to the project.

## License
(Future) Information about the project's license (e.g., MIT, Apache 2.0).
