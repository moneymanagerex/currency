# Currency Exchange Rate Viewer

This is a simple static web application that shows live currency exchange rates. The exchange rates are fetched from the [ExchangeRate-API](https://www.exchangerate-api.com/), stored in JSON files, and displayed in a table.

## Data Source

The exchange rate data comes from the [ExchangeRate-API](https://www.exchangerate-api.com/), which provides up-to-date exchange rates for various currencies. The rates are fetched and saved as JSON files in the `data/` folder.

- Example file: `data/latest_USD.json` contains the latest exchange rates for USD as the base currency.

## How the Data is Stored

- The exchange rates are stored as JSON files in the `data/` folder.
- Each file is named based on the base currency (e.g., `latest_USD.json`).
- The JSON file includes the base currency, conversion rates, and update timestamps.

## API Access

Third-party services or applications can fetch the exchange rate data through the public API available at:
https://moneymanagerex.github.io/currency/data/latest_{baseCurrency}.json

For example:
https://.github.io/currency/data/latest_USD.json
This will return the exchange rates for USD as the base currency in a JSON format.

## Usage
1. Clone or download the repository.
2. Open the `index.html` file in a web browser to view the exchange rates.
3. The base currency can be changed from the dropdown list to see rates for other currencies.

or visit https://moneymanagerex.org/currency
