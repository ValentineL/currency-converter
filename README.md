## Overview

React application that allows users to convert currencies from one unit to another, based on a selection.

## Getting started

This is a React application and as such, you'll need to have installed on your machine a few dependencies:

1. Node.js
2. Git (plus a Github account)
3. Yarn or NPM

## Running the application

There are various commands already available for you to run:

### Start the dev server

Runs the local development server on port 3000.

```console
$ yarn start
```

### Run the API

Runs the local API from a static database (currency values are not real time)

```console
$ yarn api
```

There are three endpoints made available. Each is described below:

#### Currencies

Retrieve a list of all available currencies

```
GET - http://localhost:3002/currencies
```

The currencies available as part of this test are:

```json
{
  "AUD": "Australian Dollar",
  "CAD": "Canadian Dollar",
  "CHF": "Swiss Franc",
  "CNY": "Chinese Yuan",
  "EUR": "Euro",
  "GBP": "British Pound Sterling",
  "RUB": "Russian Ruble",
  "THB": "Thai Baht",
  "USD": "United States Dollar"
}
```

#### Rates

Retrieve a list of all available currencies with rates

```
GET - http://localhost:3002/rates
```

Retrieve a single currency and its rates

```
GET - http://localhost:3002/rates/{CURRENCY_CODE}
```

#### Convert

Convert an amount from one currency to another

```
http://localhost:3002/convert?from={CURRENCY_CODE}&to={CURRENCY_CODE}&amount={AMOUNT}
```

### Testing

Runs tests via Jest and React Testing Library

```console
$ yarn test
```
