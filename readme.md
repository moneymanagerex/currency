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
https://moneymanagerex.github.io/currency/data/latest_USD.json
This will return the exchange rates for USD as the base currency in a JSON format.

## Usage
1. Clone or download the repository.
2. Open the `index.html` file in a web browser to view the exchange rates.
3. The base currency can be changed from the dropdown list to see rates for other currencies.

## Available Currency Exchange APIs

Below is a comparison of various currency exchange rate APIs, including their free plan quotas, update frequency, supported currencies, and base currency support.

| API Name                   | Free Request Quota   | Update Frequency | Supported Currencies | Base Currency Support | Notes |
|----------------------------|----------------------|------------------|----------------------|------------------------|-------|
| **ExchangeRate-API**       | 1,500 requests/day   | Every 24 hours   | 161                  | ✅ Free choice          | Good for general use |
| **Yahoo Finance**          | No official API      | Varies           | Unknown              | ✅ Available but unstable | Requires scraping or third-party tools |
| **Open Exchange Rates**    | 1,000 requests/day   | Hourly           | 170                  | ❌ Only USD             | Free plan limits base currency to USD |
| **CurrencyLayer**          | 250 requests/month   | Hourly           | 168                  | ❌ Only USD             | Good for small-scale applications |
| **Fixer.io**               | 1,000 requests/month | Daily            | 170                  | ❌ Only EUR             | Data from European Central Bank |
| **Alpha Vantage**          | 5 requests/min       | Every minute     | Multiple (includes stocks & crypto) | ✅ Free choice | Offers broader financial data |
| **X-Rates**                | No API, web-only     | Daily            | Major currencies     | ✅ Manual selection    | Suitable for manual lookups |
| **CurrencyFreaks**         | 1,000 requests/month | Real-time        | 150+                 | ✅ Free choice          | Provides real-time and historical rates |
| **CurrencyScoop**          | 1,000 requests/month | Hourly           | 168                  | ✅ Free choice          | Supports historical rates |
| **Exchangerate.host**      | Unlimited            | Daily            | 150+                 | ✅ Free choice          | Free and requires no API key |
| **聚合数据 (Juhe.cn)**      | 100 requests/day     | Every 5 minutes  | 120+                 | ✅ Free choice          | Chinese API service |
| **天聚数行 (TianAPI)**      | Free trial, then paid | Real-time       | Multiple             | ✅ Free choice          | Chinese API service |
| **XE**                     | Free trial, then paid | Real-time       | 100+                 | ✅ Free choice          | Professional-grade data |


or visit https://moneymanagerex.org/currency
