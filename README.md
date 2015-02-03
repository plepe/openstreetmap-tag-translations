In OpenStreetMap every map feature is described by tags, which are key-value-pairs. Usually these tags contain English values, but for localized maps these tags can be translated into the native language.

This repository contains translations of common tags. The format is based on the i18n format for the [Chrome browser](https://developer.chrome.com/extensions/i18n-messages).

Examples:
```json
{
    "tag:barrier": {
        "message": "Barrière",
        "!=1": "Barrières"
    },
    "tag:barrier=city_wall": {
        "message": "Mur de la ville",
        "!=1": "Murs de la ville"
    },
    "tag:name": {
        "message": "Nom",
        "!=1": "Noms",
        "description": "'name' contains name of map feature"
    },
    "tag:phone": "Numéro de tél."
}
```

Every tag key and every tag key-value-pair has an entry in the JSON file. Every entry is either a string or a hash with several entries:

* `message`: default translation
* `description`: help text
* `0`, `1`, ..., `!=1`: special translation for count of map features.
