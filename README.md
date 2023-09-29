# KSA Fuel Price API
> A user-friendly API designed to provide real-time fuel price data for the Kingdom of Saudi Arabia. 

[Project Page](https://fuel.abbara.dev)

- [KSA Fuel Price API](#ksa-fuel-price-api)
  - [Documentation](#documentation)
  - [Examples](#examples)
      - [Python](#python)
      - [Sample response](#sample-response)

<!-- ## Introduction
some intro text here? -->

## Documentation

Parameter | Description | Options
----------|----------------------------|-----------------------------------------------------------------
fuelType  | Fuel type to fetch price of. | Gasoline 91, Gasoline 95, Diesel, Kerosene, LPG, All

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
