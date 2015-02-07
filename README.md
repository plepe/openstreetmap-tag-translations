In OpenStreetMap every map feature is described by tags, which are key-value-pairs. Usually these tags contain English values, but for localized maps these tags can be translated into the native language.

This repository contains translations of common tags and additionally language names. The format is based on the i18n format for the [Chrome browser](https://developer.chrome.com/extensions/i18n-messages).

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

Directories
-----------
* The directory `tags/` contains the tag translations
* The directory `languages/` contain language name translations. There's always the string `lang:current` with the full name of the language in question (E.g. file `fr.js` contains `lang:current` = "Français" and translations of other languages, e.g. `lang:de` = "Allemand" (the french name for German).

Contributors
------------
Contributers via Git:
* Shu Higashi
* Stephan Bösch-Plepelits

Alphabetic list of contributors, with the full names from OpenStreetBrowser user names:
* Aivo
* Artur Zgodziński
* Barboska
* bazgal
* ciprian
* HgO
* higa4
* Jens Hyllegaard
* Jochen Kiene
* magnumns
* Michal Pustějovský
* Pascal Dugendre
* pinkpussy
* Remco
* Sven N
* Toni
* Wombalton
* Xuacu Saturio
* Yannis Giftomitros

Additionally the following users contributed via OpenStreetMap Wiki (which was used earlier):
* !i!
* Avila.gas
* Bb-osm
* Derstefan
* Dr&mx
* Driver2
* E-Malte
* Higa4
* Hunsly
* Invisible
* Jezevec
* Luis Latin
* Mage Whopper
* Mar4s
* Pbelas
* PierZen
* Rethna
* Richtest
* Soldier Boy
* Sven Eppler
* Vanchester
* Viw
* Xuacu

I hope I didn't miss any contributors. If you fill missed out or like to change information about you, please contact me.
