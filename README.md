# KSA Fuel Price API
Description like this?
> or like this?

- [KSA Fuel Price API](#ksa-fuel-price-api)
  - [Introduction](#introduction)
  - [Documentation](#documentation)
  - [Examples](#examples)
      - [Python](#python)

## Introduction
some intro text here?

## Documentation

Parameter | Description | Options
----------|----------------------------|-----------------------------------------------------------------
fuelType  | Fuel type to get price of. | Gasoline 91, Gasoline 95, Diesel, Kerosene, LPG

## Examples

#### Python
```py
import requests

url = "https://abbara.dev/gasPriceApi/api.php"

params = {"fuelType": "gasoline 95"}

response = requests.request("GET", url, params=params)

print(response.text)

```
