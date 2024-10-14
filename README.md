

# E-commerce Price Comparison System

## Overview

This project is designed to scrape product data from multiple e-commerce platforms (Amazon and Flipkart) and compare their prices. The system extracts relevant product details such as title, price, and other key attributes, and structures them into CSV files for easy analysis. It then compares the prices between the two platforms, displaying the lowest price for each product.

## Features

- **Data Scraping:** Automatically scrapes product details (e.g., title, price) from Amazon and Flipkart.
- **CSV Output:** Data is structured into CSV files, which include:
  - Product Title
  - Product Price
  - Platform (Amazon/Flipkart)
  - Additional product attributes (if any)
- **Price Comparison:** Compares the prices of products between the two platforms and outputs the lowest price for each product.
- **Scalable:** Easily scalable to include more platforms or categories of products.

## Technologies Used

- **Python:** Core programming language for scripting.
- **BeautifulSoup:** Web scraping tool used to parse HTML from e-commerce sites.
- **Requests:** For making HTTP requests to fetch page content.
- **Pandas:** Used to structure and process the scraped data into CSV format.

## How It Works

1. **Scraping Data:**
   - The script sends requests to the product listing pages on Amazon and Flipkart.
   - BeautifulSoup is used to parse the HTML and extract product details (e.g., title, price).

2. **Structuring Data:**
   - The extracted data is stored in two CSV files (`amazon.csv` and `flipkart_smartphone.csv`).
   
3. **Price Comparison:**
   - The prices of the same products are compared between the two CSV files.
   - The system outputs a list of the products with the lowest price across both platforms.

## Setup Instructions

### Prerequisites

- Python 3.x
- Required Python libraries:
  ```bash
  pip install beautifulsoup4 pandas requests
  ```

### Running the Project

1. Clone the repository:
   ```bash
   git clone <repo-url>
   cd e-commerce-price-comparison
   ```

2. Run the Python script to scrape data from Amazon and Flipkart:
   ```bash
   python scrape.py
   ```

3. View the structured CSV files:
   - `amazon.csv` for Amazon products.
   - `flipkart_smartphone.csv` for Flipkart products.

4. Run the comparison script to get the lowest price:
   ```bash
   python compare_prices.py
   ```

## Output

The output of the system will be a CSV file or printed results showing the product title and the lowest price between Flipkart and Amazon.

## Future Scope

- Expand to more product categories (e.g., electronics, fashion).
- Add more platforms (e.g., Myntra, Snapdeal).
- Implement a real-time price tracking system.
