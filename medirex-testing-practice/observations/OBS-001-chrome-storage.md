# OBS-001

## Názov

Neaktívne tlačidlo Pokračovať v Chrome profile

## Popis

Počas testovania registračného formulára zostávalo tlačidlo Pokračovať neaktívne aj po vyplnení všetkých povinných polí.

Po ďalšom overovaní sa správanie nepodarilo reprodukovať:

* Mozilla Firefox
* Chrome Inkognito
* Chrome Hosť

Po vymazaní Local Storage a údajov stránky sa problém prestal prejavovať aj v pôvodnom Chrome profile.

## Záver

Pozorovanie nebolo potvrdené ako chyba aplikácie.

Pravdepodobnou príčinou bol lokálny stav prehliadača alebo uložené údaje stránky.
