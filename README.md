# Similarities

This project is a web application built with Flask that compares two text files to identify similarities based on selected algorithms. It supports comparison by lines, sentences, or substrings and highlights the common elements in the provided text files.

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
git clone https://github.com/yourusername/similarities.git
cd similarities
```

2. Install the required packages:

```bash
pip install -r requirements.txt
```

### Usage

1. Run the Flask application:

```bash
python app.py
```

2. Open your web browser and navigate to:

```
http://127.0.0.1:5000/
```

3. Upload two text files, select the desired comparison algorithm, and submit the form to view the highlighted similarities.

### Project Structure

- `app.py`: Main application file.
- `templates/`: Contains HTML templates for the application.
  - `index.html`: Main page template.
  - `compare.html`: Comparison results template.
  - `error.html`: Error handling template.
- `static/`: Static files (CSS, JS, images).
- `helpers.py`: Contains helper functions for text processing.

### Comparison Algorithms

The application supports three comparison algorithms to identify similarities between two text files: lines, sentences, and substrings.

#### Lines

Compares the files line by line, highlighting lines that are exactly the same in both files. Useful for structured text like code or logs.

#### Sentences

Compares the files sentence by sentence, highlighting identical sentences. Ideal for comparing prose or documentation.

#### Substrings

Compares files for common substrings of a specified length, highlighting matching substrings. Suitable for detailed text analysis.

#### Highlighting

Matching elements are highlighted to visually indicate similarities, making it easy to see where the text files overlap.

### Helper Functions

- `lines(file1, file2)`: Returns common lines between two text files.
- `sentences(file1, file2)`: Returns common sentences between two text files.
- `substrings(file1, file2, length)`: Returns common substrings of a specified length between two text files.

### Error Handling

The application handles various errors such as missing files, invalid files, and missing or invalid algorithm parameters. Custom error messages are displayed for user guidance.

### Configuration

- `TEMPLATES_AUTO_RELOAD`: Reload templates automatically when they are changed.
- `Cache-Control`: Disable caching to ensure the most recent version of files is used.

## Acknowledgments

- [CS50](https://cs50.harvard.edu/): For the CS50 library and inspiration.
- [Flask](https://flask.palletsprojects.com/): For the web framework.

---
