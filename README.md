# pydigimon

Python implementation of the [Digimon API by Shadow Smith](https://digimon-api.vercel.app/).

## Installation

TODO

## Usage

```
from digimon.client import DigimonClient
client = DigimonClient()
response = client.get_digimon_by_name("agumon")
print(response.json())
```
