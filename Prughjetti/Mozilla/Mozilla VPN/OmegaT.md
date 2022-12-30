# Istruzzioni per impiegà _OmegaT_ per a traduzzione di _Mozilla VPN_

Eccu l’istruzzioni per scaricà l’ultima versione di i schedarii di traduzzione in lingua inglese, appruntalli per un trattamentu cù l’appiecazione _OmegaT_, è rinfrescà a versione in lingua corsa.

## Scaricamentu di i schedarii di lingua inglese

Ci hè parechji schedarii à traduce.

- Nant’à un navigatore Internet, andà à st’indirizzi :  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/mozillavpn.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/guide_01_how_to_vpn/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/guide_02_is_my_vpn_working_correctly/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/guide_03_adding_and_removing_devices/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/guide_04_connecting_external_devices/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/guide_05_what_is_multi_hop/strings.xliff  
https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/guide_06_benefits_of_custom_dns/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/guide_07_app_permissions/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_privacy_bundle_staging/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_survey/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_update_v2.12/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_whats_new_v2.10/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_whats_new_v2.11/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_whats_new_v2.12/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/tutorial_01_get_started2/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/tutorial_01_get_started/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/tutorial_02_connect_on_startup/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/tutorial_03_multi_hop/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-website-l10n/blob/main/en-US/vpn.ftl

- Per ogni schedariu, fà un __cliccu dirittu__ nant’à u buttone `Raw`, à dirittu, accant’à l’icone di u screnu, di a mina, è di a curbella

- Arregistrateli, unu dopu à l’altru, cù quelli nomi :
```
  mozillavpn.xliff
  addons-guide_01_how_to_vpn-strings.xliff
  addons-guide_02_is_my_vpn_working_correctly.xliff
  addons-guide_03_adding_and_removing_devices-strings.xliff
  addons-guide_04_connecting_external_devices-strings.xliff
  addons-guide_05_what_is_multi_hop-strings.xliff
  addons-guide_06_benefits_of_custom_dns-strings.xliff
  addons-guide_07_app_permissions-strings.xliff
  addons-message_privacy_bundle_staging-strings.xliff
  addons-message_survey-strings.xliff
  addons-message_update_v2.12-strings.xliff
  addons-message_whats_new_v2.10-strings.xliff
  addons-message_whats_new_v2.11-strings.xliff
  addons-message_whats_new_v2.12-strings.xliff
  addons-tutorial_01_get_started2-strings.xliff
  addons-tutorial_01_get_started-strings.xliff
  addons-tutorial_02_connect_on_startup-strings.xliff
  addons-tutorial_03_multi_hop-strings.xliff
  vpn.ftl
```
## Preparazione di i schedarii nanzu a traduzzione

### Estensione .xliff

Ci vole à appruntà __solu__ i schedarii cù l’estensione : `.xliff`.  

In primu locu, ci vole à [installà è impiegà a prucedura di cunversione](Cunversione.md) per trasfurmà u so cuntenutu.

- Eppò lancià _Notepad++_
- Apre u schedariu `.xliff`
- Eseguisce a macro installata appostu chì si chjama `Cunversione Mozilla VPN(XLIFF)-OmegaT(XLIFF)`
- Arregistrà u schedariu cù u listessu nome
- Fà a listessa operazione per tutti i schedarii `.xliff`

S’ella hè bisognu, ci hè dinù un’altra prucedura di cunversione chì si chjama `Cunversione Mozilla VPN(XLIFF)-OmegaT(TXT)` per trasfurmà un schedariu `.xliff` in furmatu testu simplice. In stu casu, l’estensione di u schedariu trasfurmatu serà `.txt`.

### Estensione .ftl

✔️ Ùn ci nisunu approntu à fà per i schedarii cù l’estensione `.ftl`.

## Copia di i schedarii di lingua inglese

- Cupià o dispiazzà sti schedarii in u cartulare `source` di u prughjettu _Mozilla VPN_ in _OmegaT_

## Ozzione o preferenze particulare à definisce in OmegaT

- Lancià l’appiecazione _OmegaT_
- Sceglie `Ozzioni` eppò `Filtri di schedariu…`
  - Disattivà u furmatu `XLIFF`
  - Attivà u furmatu `XLIFF files (Okapi)`
  - Verificà l’ozzioni di u furmatu `XLIFF files (Okapi)` :  
    ⚫ `Use the default filter settings (okf_xliff)`  
    ⚪ `Use the following filter parameter file:`
    - [x] `Include the name of the translation unit in comments`
    - [ ] `Show and protect entries with translate='no' (if not set: they are not extracted)`
    - [x] `Protect entries with state='final' (if not set: they can be edited)`
  - Verificà l’ozzioni di u furmatu `FTL Mozilla` :  
    - [x] `Caccià e catene micca tradutte in i schedarii tradutti`

## Traduzzione in lingua corsa

- Lancià l’appiecazione _OmegaT_ è apre stu prughjettu per traducelu

## Preparazione di i schedarii dopu a traduzzione

### Estensione .ftl

✔️ Ùn ci nisunu approntu à fà per i schedarii cù l’estensione `.ftl`.

### Estensione .xliff

✔️ Ùn ci nisunu approntu à fà per i schedarii cù l’estensione `.xliff`.

### Estensione .txt

⛔ Per disgrazia, ùn ci hè alcuna prucedura, à st’ora, per trasfurmà u cuntenutu di i schedarii da u furmatu `.txt` à u furmatu `.xliff`.

## Incaricamentu di i schedarii di lingua corsa

Per ogni schedariu, ci vole à impiegà _Pontoon_ per impurtacci u schedariu traduttu in lingua corsa.
- Fà un cliccu nant’à a vostra icona d’utilizatore chì si trova insù è à dirittu, accant’à l’icona di a campana 🔔
- Sceglie a funzione _`Upload Translations`_ (ghjè una funzione riservata à u respunsevule di prughjettu)
- Selezziunà u schedariu di lingua corsa chì si trova in u cartulare `target` di u prughjettu _Mozilla VPN_ in _OmegaT_
- À a fine di stu trattamentu, _Pontoon_ hè statu rinfrescatu cù e nove traduzzioni
