# Istruzzioni per impiegà _OmegaT_ per a traduzzione di _Mozilla VPN_

Eccu l’istruzzioni per scaricà l’ultima versione di i schedarii di traduzzione in lingua inglese, appruntalli per un trattamentu cù l’appiecazione _OmegaT_, è rinfrescà a versione in lingua corsa.

## Scaricamentu di i schedarii di lingua inglese

À st’ora, schedarii, ci n’hè circa 30, in dui dipositi _GitHub_ è in parechji sottucartulari. Ancu di grazia, ci hè una prucedura per scaricalli tutti di manera autumatica. Sta prucedura, chì impiega __Windows PowerShell__, si chjama `Schedarii in inglese.ps1`.  

Per a vostra infurmazione, ci hè una prucedura simile per scaricà i schedarii in lingua corsa chì si chjama `Schedarii in corsu.ps1`.

###  A prucedura autumatica

- Apre a prucedura per [scaricà tutti i schedarii in inglese](Schedarii%20in%20inglese.ps1)
- Cliccà nant’à u buttone `Raw`, insù è à dirittu, accant’à l’icone di u screnu, di a mina, è di a curbella
- Selezziunà tutte e linee cù a cumanda `Ctrl-A`
- Cupià tutte e linee cù a cumanda `Ctrl-C`
- Lancià _Windows PowerShell_ cù un cliccu dirittu nant’à u listinu « Démarrer »
- Rimpiazzià u cartulare attuale - cù a cumanda `CD u_mo_cartulare` - da quellu induve ci vole à piazzà i schedarii scaricati, per indettu : `CD C:\Traduzzione\OmegaT\Mozilla_VPN\source\`
- Incullà e linee cupiate cù a cumanda `Ctrl-V`
- Appughjate nant’à u tastu `Entrée`
- Quandu tutte e cumande sò state passate, i schedarii d’origine in inglese si trovanu in u cartulare sceltu
- Chjode _Windows PowerShell_ cù a cumanda `exit`

###  A manera manuale

Ci hè parechji schedarii à traduce, è a lista cambia di quandu in quandu.

- Nant’à un navigatore Internet, andà à st’indirizzi :  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/mozillavpn.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/guide_01_how_to_vpn/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/guide_02_is_my_vpn_working_correctly/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/guide_03_adding_and_removing_devices/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/guide_05_what_is_multi_hop/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/guide_08_privacy_features/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/guide_09_custom_dns/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/guide_10_app_exclusions/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/guide_11_recommended_servers/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/guide_12_multi_account_containers/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_subscription_expiring/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_survey/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_update_v2.15/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_update_v2.17/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_update_v2.18/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_update_v2.19/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_upgrade_to_annual_plan/strings.xliff/  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_whats_new_v2.15/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_whats_new_v2.16/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_whats_new_v2.17/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_whats_new_v2.18/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/message_whats_new_v2.19/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/tutorial_01_get_started_recommended_locations/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/tutorial_01_get_started/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/tutorial_02_connect_on_startup/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/tutorial_03_multi_hop/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-client-l10n/blob/main/en/addons/tutorial_04_split_tunneling3/strings.xliff  
  https://github.com/mozilla-l10n/mozilla-vpn-website-l10n/blob/main/en-US/vpn.ftl

- Per ogni schedariu, fà un __cliccu dirittu__ nant’à u buttone `Raw`, à dirittu, accant’à l’icone di u screnu, di a mina, è di a curbella

- Arregistrateli, unu dopu à l’altru, cù quelli nomi :
```
  mozillavpn.xliff
  addons-guide_01_how_to_vpn-strings.xliff
  addons-guide_02_is_my_vpn_working_correctly.xliff
  addons-guide_03_adding_and_removing_devices-strings.xliff
  addons-guide_05_what_is_multi_hop-strings.xliff
  addons-guide_08_privacy_features-strings.xliff
  addons-guide_09_custom_dns-strings.xliff
  addons-guide_10_app_exclusions-strings.xliff
  addons-guide_11_recommended_servers-strings.xliff
  addons-guide_12_multi_account_containers-strings.xliff
  addons-message_subscription_expiring-strings.xliff
  addons-message_survey-strings.xliff
  addons-message_update_v2.15-strings.xliff
  addons-message_update_v2.17-strings.xliff
  addons-message_update_v2.18-strings.xliff
  addons-message_update_v2.19-strings.xliff
  addons-message_upgrade_to_annual_plan-strings.xliff
  addons-message_whats_new_v2.15-strings.xliff
  addons-message_whats_new_v2.16-strings.xliff
  addons-message_whats_new_v2.17-strings.xliff
  addons-message_whats_new_v2.18-strings.xliff
  addons-message_whats_new_v2.19-strings.xliff
  addons-tutorial_01_get_started_recommended_locations-strings.xliff
  addons-tutorial_01_get_started-strings.xliff
  addons-tutorial_02_connect_on_startup-strings.xliff
  addons-tutorial_03_multi_hop-strings.xliff
  addons-tutorial_04_split_tunneling3-strings.xliff
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
  - Attivà u furmatu `FTL Mozilla`
  - Attivà u furmatu `XLIFF (filtru anzianu)`
  - Disattivà u furmatu `XLIFF files (Okapi)`
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
