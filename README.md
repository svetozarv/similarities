# Similarities

This project is a web application built with Flask that compares two text files to identify similarities based on selected algorithms. It supports comparison by lines, sentences, or substrings and highlights the common elements in the provided text files.
![image](https://github.com/svetozarv/similarities/assets/106545363/bd808358-0c14-46eb-9f44-496abb1e80ba)

## Features

- Upload two text files for comparison.
- Select comparison algorithm: lines, sentences, or substrings.
- Highlights common elements found in the text files.

## Getting Started

### Prerequisites

- Python 3.x
- Flask
- CS50 Library for Python

### Installation

1. Clone the repository:

```bash
git clone https://github.com/svetozarv/similarities.git
```

2. Install the required packages (flask, cs50, ntlk):

```
pip install -r requirements.txt
```

### Usage

1. Run the Flask application:

```
flask run
```

2. Open your web browser and navigate to:

```
http://127.0.0.1:5000/
```

3. Upload two text files, select the desired comparison algorithm, and submit the form to view the highlighted similarities.
- `inputs/`: Contains files for comparison.


## Comparison Algorithms

The application supports three comparison algorithms to identify similarities between two text files: lines, sentences, and substrings.

#### Lines

Compares the files line by line, highlighting lines that are exactly the same in both files. Useful for structured text like code or logs.

#### Sentences

Compares the files sentence by sentence, highlighting identical sentences. Ideal for comparing prose or documentation.

#### Substrings

Compares files for common substrings of a specified length, highlighting matching substrings. Suitable for detailed text analysis.

#### Highlighting

Matching elements are highlighted to visually indicate similarities, making it easy to see where the text files overlap.


## Acknowledgments

- [CS50](https://cs50.harvard.edu/): For the CS50 library and inspiration.
- [Flask](https://flask.palletsprojects.com/): For the web framework.

---
