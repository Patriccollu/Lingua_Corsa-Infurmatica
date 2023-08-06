# Istruzzioni per impiegà _OmegaT_ per a traduzzione di _fre:ac_

Per fà una traduzzione, l'appiecazione _OmegaT_ hà bisognu di schedarii di fonte cù una lingua sfarente di quella di destinazione. Di regula, a lingua di fonte hè l’inglese è quella di destinazione hè u corsu. D’altronde tutte e memorie di traduzzione pruviste nant’à stu situ sò in u sensu da l’inglese ver di u corsu.

Eccu l’istruzzioni per scaricà l’ultima versione di i schedarii di traduzzione è appruntalli per un trattamentu cù l’appiecazione _OmegaT_.

## Scaricamentu di i schedarii à traduce

Si pò scaricà i schedarii __in lingua inglese__ da trè lochi :  

1- Nant’à a [pagina _Crowdin_ di u prughjettu _fre:ac_ in lingua corsa](https://crowdin.com/project/freac/co)  

2- Nant’à _GitHub_ à u furmatu impiegatu da _Crowdin_ :
- [freac.xml](https://github.com/enzo1982/freac/blob/master/i18n/freac/crowdin/freac.xml)
- [setup.xml](https://github.com/enzo1982/freac/blob/master/i18n/setup/crowdin/setup.xml)
- [tips.xml](https://github.com/enzo1982/freac/blob/master/i18n/tips/crowdin/tips.xml)
- [eupdate.xml](https://github.com/enzo1982/freac/blob/master/i18n/updater/crowdin/eupdate.xml)

- Per ogni schedariu `.xml` ci vole à :
  - Fà un cliccu drittu nant’à u buttone « _Raw_ » chì si trova à diritta, accant’à l’icone di u screnu, di a mina è di a curbella
  - Sceglie l’ozzione « _Arregistrà a sibula di a leia sottu…_ »

3- Nant’à _GitHub_ à un altru furmatu (cartulare senza `crowdin`) :
- https://github.com/enzo1982/freac/blob/master/i18n/freac/freac.xml
- https://github.com/enzo1982/freac/tree/master/i18n/setup/freac.xml
- https://github.com/enzo1982/freac/tree/master/i18n/tips/freac.xml
- https://github.com/enzo1982/freac/tree/master/i18n/updater/freac.xml

- In stu casu, ci vole à trasfurmà u cuntenutu d’ogni schedariu di traduzzione cù l’aiutu d’una prucedura di cunversione nanzu di pudè traducelu cù _OmegaT_
- Seguitate l’[istruzzioni per installà una prucedura di cunversione specifica](Cunversione.md)

## Preparazione di i schedarii nanzu a traduzzione

✔️ Ùn ci hè alcunu approntu à fà à i schedarii di lingua inglese s’elli sò stati scaricati o da _Crowdin_, o da i sottucartulari `crowdin`. In l'altru casu, ci vole à impiegà una prucedura di cunversione.

## Copia di i schedarii di lingua inglese

- Cupià o dispiazzà sti schedarii in u cartulare `source` di u prughjettu _fre:ac_ in _OmegaT_.

## Ozzione o preferenze particulare à definisce in OmegaT

- Lancià l’appiecazione _OmegaT_
- Sceglie `Ozzioni` eppò `Filtri di schedariu…`
  - Verificà chì u furmatu `XML files (Okapi - XML Filter)` hè disattivatu
  - Verificà chì u furmatu `XML files (Okapi - XML Stream Filter)` hè attivatu
  - Verificà l’ozzioni di u furmatu `XML files (Okapi - XML Stream Filter)` :  
    ⚫ `Use the default filter settings (okf_xmlstream)`  
    ⚪ `Use the following filter parameter file:`  
	   `________________________________________`
    - [x] `Include the name of the translation unit in comments`

## Traduzzione in lingua corsa

- Lancià l’appiecazione _OmegaT_ è apre stu prughjettu per traducelu.

## Preparazione di i schedarii dopu a traduzzione

✔️ Ùn ci hè alcunu approntu à fà à i schedarii di lingua corsa.

## Incaricamentu di i schedarii di lingua corsa
- Tutti in schedarii tradutti in lingua corsa da _OmegaT_ si trovanu in u cartulare `target` di u prughjettu _fre:ac_
- Per ogni schedariu traduttu, ci vole à impiegà _Crowdin_ cù l’azzione `File` > `Upload Translations…` per rinfrescallu
- Ma s’è _Crowdin_ ùn hè micca impiegatu, ci vole à incaricà i schedarii tradutti via _GitHub_
- In quellu casu, seguitate l’[istruzzioni per incaricà u schedariu traduttu via _GitHub_](Traduzzione.md#via-github-1)
