
# Currency Converter Package Documentation

## Overview

This document provides documentation for the main functions developed in the Currency Converter package. The Currency Converter package allows users to convert amounts from one currency to another.

## Functions

### `convert_currency`

#### Purpose

The `convert_currency` function converts a given amount from one currency to another.

#### Inputs

- `amount`: Numeric value representing the amount to convert.
- `from_currency`: Character string specifying the currency to convert from (e.g., 'USD').
- `to_currency`: Character string specifying the currency to convert to (e.g., 'INR').

#### Outputs

- Numeric value representing the converted amount.

#### Usage

```r
converted_amount <- convert_currency(1, 'USD', 'INR')
print(converted_amount)
```

### `fetch_exchange_rate`

#### Purpose

The `fetch_exchange_rate` function retrieves the exchange rate between two currencies.

#### Inputs

- `from_currency`: Character string specifying the currency to convert from (e.g., 'USD').
- `to_currency`: Character string specifying the currency to convert to (e.g., 'INR').

#### Outputs

- Numeric value representing the exchange rate.

#### Usage

```r
exchange_rate <- fetch_exchange_rate('USD', 'INR')
print(exchange_rate)
```

## Additional Information

- The `convert_currency` function assumes a fixed conversion rate. For real time applications , consider using `fetch_exchange_rate` to fetch real-time rates from an API.
- Error handling is included to check if the provided currencies are available for conversion.

## Insights and Challenges

- One crucial factor to take into account was how to keep the package design simple while still retaining flexibility..
- Future upgrades could involve introducing methods for currency caching and supporting more currencies.

