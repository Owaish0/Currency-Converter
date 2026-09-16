# Currency Converter

A React learning project for selecting currencies, converting an amount, and swapping the source and target currencies. Built with **React, Vite, and Tailwind CSS**.

## Data source

`src/hooks/useCurrencyInfo.js` fetches the Fawaz Ahmed currency dataset through jsDelivr. The source currently pins the dataset to **2024-03-06**. Results use that historical snapshot; they are not live exchange rates.

## Run locally

Requires Node.js and npm.

```bash
git clone https://github.com/Owaish0/Currency-Converter.git
cd Currency-Converter
npm ci
npm run dev
```

Open the local address printed by Vite. Select the source and target currencies, enter an amount, and click Convert. Swap exchanges the selected currencies.

```bash
npm run build
npm run preview
```

## Source guide

- `src/App.jsx`: selected currencies, amount, swap, and conversion state.
- `src/components/InputBox.jsx`: reusable amount and currency input.
- `src/hooks/useCurrencyInfo.js`: fetches rate data when the base currency changes.

## Next improvements

Add loading and failure states, validate unavailable rates, and make the dataset date visible to the user. A switch to current rates should be an explicit implementation change with a displayed data timestamp.

## Attribution

The previous README linked to [aayush2761/currencyConverter](https://github.com/aayush2761/currencyConverter). That reference is retained here for provenance; this README does not assert sole original authorship. Rate data comes from [Fawaz Ahmed's currency API](https://github.com/fawazahmed0/exchange-api).
