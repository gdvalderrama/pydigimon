# pydigimon

Python implementation of the [Digimon API by Shadow Smith](https://digimon-api.vercel.app/).

## Installation

`pip install pydigimon`

## Usage

```
from digimon.client import DigimonClient
client = DigimonClient()
response = client.get_digimon_by_name("agumon")
print(response.json())
```

## Packaging

To build package and publish to pypi:

* `python3 -m build`
* `python3 -m twine upload dist/*`
