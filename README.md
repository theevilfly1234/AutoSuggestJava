# Java Autocomplete System

This project implements an autocomplete system in Java, designed to suggest completions for a prefix based on a set of terms where each term has a query string and an associated weight. The system prioritizes suggestions based on the weight, suggesting higher-weighted terms first.

## Background

The autocomplete system is built on the principles of sorting and binary search. It uses a data structure that efficiently stores a large set of terms and quickly retrieves all terms that start with a given prefix, ordered by descending weight. This system can be utilized in various applications, such as search engines, code editors, or any user interface requiring predictive text input.

## Features

- **Term Storage**: Stores terms with a query string and an associated weight.
- **Prefix Matching**: Efficiently finds all terms that start with a given prefix.
- **Weight Sorting**: Sorts matched terms in descending order of their weights for prioritization.
- **Binary Search Optimization**: Utilizes binary search for fast lookup of terms.

## Getting Started

### Prerequisites

Ensure you have a Java Development Kit (JDK) installed on your system to compile and run this project. The project was developed and tested with JDK version 11.

### Compilation

Navigate to the project directory and compile the Java files:

### Compilation

Navigate to the project directory and compile the Java files:

```bash
javac Autocomplete.java BinarySearchDeluxe.java Term.java
```

Running

Run the autocomplete system with:
java Autocomplete <filename> <number-of-suggestions>

<filename>: Path to a text file containing the terms, one per line, with each line formatted as <weight><tab><query string>.
<number-of-suggestions>: The maximum number of suggestions to return for a given prefix.

Example
java Autocomplete cities.txt 5

This command will run the autocomplete system on the cities.txt file, returning up to 5 suggestions for each prefix entered by the user.

Contributing
Contributions to this project are welcome. Please feel free to fork the repository, make your changes, and submit a pull request with your improvements.

License
This Java Autocomplete System is made available under the MIT License. Feel free to use, modify, and distribute the code as you see fit.

Acknowledgments
Thanks to the inventors and contributors to the algorithms and data structures that make systems like this possible.
This project was inspired by the goal of understanding and implementing efficient search and sorting techniques in Java.