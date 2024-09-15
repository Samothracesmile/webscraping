
# Web Scraping Project

This project includes a set of Jupyter notebooks that demonstrate how to perform web scraping for various types of content. These notebooks allow you to scrape text, tables, and export HTML content to PDF format using different tools and techniques.

## Table of Contents
- [Requirements](#requirements)
- [Notebooks Overview](#notebooks-overview)
    - [1. Scraper Website Text](#1-scraper-website-text)
    - [2. Scraper Table](#2-scraper-table)
    - [3. HTML to PDF](#3-html-to-pdf)
- [How to Use](#how-to-use)
- [Disclaimer](#disclaimer)

## Requirements

To run the notebooks, you'll need the following Python packages:

- `beautifulsoup4`
- `requests`
- `pandas`
- `pdfkit`
- `html5lib`
- `lxml`
- `PyMuPDF` (optional for PDF handling)
  
You can install the necessary dependencies by running the following command:

\`\`\`bash
pip install beautifulsoup4 requests pandas pdfkit html5lib lxml PyMuPDF
\`\`\`

Additionally, if you're using the `pdfkit` library for generating PDFs from HTML, you may need to install [wkhtmltopdf](https://wkhtmltopdf.org/) on your system.

## Notebooks Overview

### 1. Scraper Website Text
This notebook demonstrates how to scrape textual content from websites using `BeautifulSoup`. It includes:

- Fetching HTML content using the `requests` library.
- Parsing and extracting specific text elements from the webpage, such as headers, paragraphs, and other text-based tags.
- Saving the extracted text to a `.txt` file.

### 2. Scraper Table
This notebook is focused on scraping tables from web pages. It includes:

- Extracting HTML tables using `BeautifulSoup` and `pandas`.
- Parsing the table data into a `pandas` DataFrame for further analysis.
- Exporting the table data to a CSV or Excel file for easy usage.

### 3. HTML to PDF
This notebook shows how to convert web pages or raw HTML into PDF format. It includes:

- Fetching the HTML content of a webpage using `requests`.
- Using the `pdfkit` library to render the HTML content as a PDF.
- Alternatively, handling PDFs via `PyMuPDF` for post-processing or further manipulation.

## How to Use

1. Clone the repository to your local machine:
   \`\`\`bash
   git clone <repository-url>
   \`\`\`

2. Install the required dependencies:
   \`\`\`bash
   pip install -r requirements.txt
   \`\`\`

3. Open the Jupyter notebooks in your preferred environment (e.g., Jupyter Lab, VSCode, or Jupyter Notebook):
   \`\`\`bash
   jupyter notebook
   \`\`\`

4. Run the individual notebooks based on your scraping needs:
   - For scraping text: open and run `scraper_website_text.ipynb`.
   - For scraping tables: open and run `scraper_table.ipynb`.
   - For converting HTML to PDF: open and run `html2pdf.ipynb`.

5. Modify the URLs or selectors in the notebooks according to the website or content you want to scrape.

## Disclaimer

Please ensure that you comply with the Terms of Service and the legal requirements for any website you are scraping. Web scraping can sometimes violate site terms, and scraping certain websites without permission may be illegal. Always make sure to respect `robots.txt` rules, if applicable.
