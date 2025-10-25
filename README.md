# Webpage to PDF Converter (Dynamic Title & Filename)

## 📘 Overview
This Python script downloads the readable text content from any webpage and converts it into a **clean, formatted PDF** file.

It automatically:
- Extracts the main text using **trafilatura** (ignoring ads, menus, and clutter)
- Generates the **PDF filename dynamically** from the URL 
- Creates a **title inside the PDF** based on the page name 
- Formats the text into readable paragraphs using **ReportLab**

---

## 🧠 Example

If you set the URL to:

https://en.wikipedia.org/wiki/Neuro-linguistic_programming


The script will automatically generate:
- PDF file → `Neuro-linguistic_programming.pdf`
- PDF title → “Neuro-Linguistic Programming”

---

##  Requirements

Before running the script, install the following Python libraries:


pip install trafilatura reportlab


These are the main dependencies:

- trafilatura → for extracting main content from webpages

- reportlab → for generating formatted PDFs

## How to Run

- Clone or download this repository.

- Open the script in your favorite editor (VS Code, PyCharm, etc.)

- Modify the url variable inside the script to any webpage link you want.

- Run the script

- The PDF will be generated in the same folder with the URL-based name.

🧩 Code Flow Summary

- Fetch webpage using trafilatura.fetch_url()

- Extract main text from the HTML using trafilatura.extract()

- Clean and split text into paragraphs using regular expressions

- Generate filename and title dynamically from the URL

- Create and style a PDF with reportlab

- Save the final PDF



## Future Enhancements

- Fetch the actual <title> tag from the webpage for more accurate PDF titles

- Add headers, footers, and page numbers

- Convert to a function or command-line tool (python webpage_to_pdf.py <URL>)

## Author

Created by [Srinija Madireddy] — for learning and practicing web scraping, data extraction, and PDF generation in Python.


