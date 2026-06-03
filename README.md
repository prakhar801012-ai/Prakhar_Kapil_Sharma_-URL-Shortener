# URL Shortener 🔗

A simple Python project that converts long URLs into shorter, more shareable links using the TinyURL service and the `pyshorteners` library.

## Description

This program asks the user to enter a URL and then generates a shortened version of that URL using TinyURL.

It is a great beginner project for learning:

- Third-party Python libraries
- User input handling
- API-based services
- String processing

## Requirements

Install the required package before running the program:

```python
!pip install pyshorteners
```

Or from the terminal:

```bash
pip install pyshorteners
```

## Code

```python
import pyshorteners

url = input("Enter URL: ")

shortener = pyshorteners.Shortener()

short_url = shortener.tinyurl.short(url)

print("Short URL:", short_url)
```

## How to Run

1. Install Python 3.
2. Install the required package:

```bash
pip install pyshorteners
```

3. Save the code as `url_shortener.py`.
4. Run the program:

```bash
python url_shortener.py
```

5. Enter a valid URL when prompted.

## Example

### Input

```text
Enter URL: https://www.google.com
```

### Output

```text
Short URL: https://tinyurl.com/xxxxx
```

*The exact shortened URL will vary.*

## Features

- Shortens long URLs instantly
- Easy to use
- Uses the TinyURL service
- Lightweight and beginner-friendly
- Requires only a few lines of code

## Concepts Used

- Python libraries
- User input with `input()`
- Variables and objects
- Working with web services
- String output formatting

## Project Structure

```text
url-shortener/
│
├── url_shortener.py
└── README.md
```

## Future Improvements

- Support multiple URL shortening services
- Add URL validation
- Store previously shortened URLs
- Create a graphical user interface (GUI)
- Generate QR codes for shortened URLs
- Copy shortened URLs directly to the clipboard

## License

This project is open source and free to use.
