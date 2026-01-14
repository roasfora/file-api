Python Notebook: File Operations & API Interactions

This notebook demonstrates fundamental data handling in Python using Pandas for CSV/Excel/JSON files and interacting with external APIs.

## Table of Contents

1.  [Working with Files](#working-with-files)
    *   [Creating Excel and CSV Files](#creating-excel-and-csv-files)
    *   [Reading CSV and Excel Files](#reading-csv-and-excel-files)
    *   [Writing a CSV File](#writing-a-csv-file)
    *   [Writing and Reading JSON](#writing-and-reading-json)
2.  [API Interactions](#api-interactions)
    *   [Pokémon API](#pokemon-api)
    *   [Weather (Open-Meteo API)](#weather-open-meteo-api)
    *   [Bitcoin Price (CoinGecko & CoinMarketCap APIs)](#bitcoin-price-coingecko--coinmarketcap-apis)

---

## 1. Working with Files

This section covers how to create, read, and write different file formats commonly used in data science.

### Creating Excel and CSV Files

The notebook starts by creating a Pandas DataFrame with city data and then saving it to both an Excel file (`.xlsx`) and a CSV file (`.csv`).

### Reading CSV and Excel Files

It then demonstrates how to load data back into a Pandas DataFrame from the previously created CSV and Excel files.

### Writing a CSV File

This part shows how to modify the DataFrame (by adding a new city) and then save the updated data to a new CSV file.

### Writing and Reading JSON

Finally, the notebook illustrates how to convert a Pandas DataFrame to a JSON format, save it to a `.json` file, and then load it back into Python.

---

## 2. API Interactions

This section explores how to fetch data from various public APIs.

### Pokémon API

An example of fetching data for 'Pikachu' from the PokeAPI is provided, showcasing how to extract specific information like name, height, weight, and abilities.

### Weather (Open-Meteo API)

This part demonstrates how to use the Open-Meteo API to get current weather data for a specific location (Lisbon, Portugal), including temperature, wind speed, and weather code.

### Bitcoin Price (CoinGecko & CoinMarketCap APIs)

Two methods for retrieving Bitcoin price are shown:

*   **Without API Key (CoinGecko)**: A simple request to CoinGecko API to get the current Bitcoin price in USD without requiring an API key.
*   **With API Key (CoinMarketCap)**: An example using the CoinMarketCap Pro API, which requires an API key for access. This demonstrates how to include API keys in request headers.

**Important Note on API Keys:** Never expose your API keys directly in your code or public notebooks. For Colab, it's recommended to use the Secrets Manager (🔑 icon in the left panel) to securely store your keys and access them in your code.

---

## Usage

To run this notebook:

1.  Ensure you have Python installed.
2.  Install the necessary libraries:
    ```bash
    pip install pandas requests openpyxl
    ```
3.  If you plan to use the CoinMarketCap API, obtain an API key and store it securely in Colab's Secrets Manager.
4.  Execute the cells sequentially.
