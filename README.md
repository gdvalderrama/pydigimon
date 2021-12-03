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

## Packaging and releases

### Automated flow

Packaging is automated with github actions.
To release a new version:

* tag release commit with `git tag x.y.z`
* push tag to github `git push origin --tags`
* in github, make a new release from the tag
* the github action is triggered

### Manual release

To manually build package and publish to pypi:

* `python3 -m build`
* `python3 -m twine upload dist/*`
