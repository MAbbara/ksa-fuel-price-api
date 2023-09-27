# KSA Fuel Price API
> or like this?

- [KSA Fuel Price API](#ksa-fuel-price-api)
  - [Introduction](#introduction)
  - [Documentation](#documentation)
  - [Examples](#examples)
      - [Python](#python)
      - [Sample response](#sample-response)

## Introduction
some intro text here?

## Documentation

Parameter | Description | Options
----------|----------------------------|-----------------------------------------------------------------
fuelType  | Fuel type to fetch price of. | Gasoline 91, Gasoline 95, Diesel, Kerosene, LPG

## Examples

#### Python
```py
import requests

url = "https://fuel.abbara.dev/"

params = {"fuelType": "gasoline 95"}

response = requests.request("GET", url, params=params)

print(response.text)

```
#### Sample response
```json
{
    "type": "gasoline 95",
    "price": 2.33,
    "lastUpdated": "2023-09-27 17:14:36"
}
```
