# Istruzzioni per impiegà _OmegaT_ per a traduzzione di _Thunderbird for Android_

Per fà una traduzzione, l'appiecazione _OmegaT_ hà bisognu di schedarii di fonte cù una lingua sfarente di quella di destinazione. Di regula, a lingua di fonte hè l’inglese è quella di destinazione hè u corsu. D’altronde tutte e memorie di traduzzione pruviste nant’à stu situ sò in u sensu da l’inglese ver di u corsu.
  
Eccu l’istruzzioni per scaricà l’ultima versione di i schedarii di traduzzione è appruntalli per un trattamentu cù l’appiecazione _OmegaT_.

## Scaricamentu di i schedarii à traduce

- Si pò scaricà i schedarii __in lingua inglese__ da quì :  
  https://hosted.weblate.org/projects/tb-android/-/en/#components

- Per ogni schedariu, ci vole à scaricallu cù un furmatu trà quelli dui :
  - u so furmatu d’origine `.xml` o `.strings` cù l’azzione `Fichiers` > `Télécharger la traduction`
  - u furmatu `.xliff` cù l’azzione `Fichiers` > `Personnaliser le téléchargement` è sceglie u furmatu preferitu, per indettu `XLIFF 1.1`

- S’ella hè bisognu, si pò scaricà i schedarii in __lingua corsa__ da quì :  
  https://hosted.weblate.org/projects/tb-android/-/co/#components

- Tutti i schedarii scaricati anu un nome chì principià cù `tb-android-`

## Preparazione di i schedarii nanzu a traduzzione

- Ci vole à appruntà i schedarii cù l’estensione : `.strings`
- Ùn ci hè nunda à fà per l’estensioni `.xml`

### Estensione .strings
- Lancià _Notepad++_
- Installà e prucedure di cunversione cum’è indicatu in [st’istruzzioni detagliate](../Prughjetti/VLC/Cunversione.md)
- Apre __tutti i schedarii__ cù l’estensione : `.strings`
- Sceglie `Macro`, eppò `Eseguisce una macro parechje volte…`
- Selezziunà u nome di a prucedura à impiegà : `Cunversione VLC(.strings)-OmegaT(.strings)`
- Cliccu nant’à `Eseguisce 1 volta`
- Appughjà nant’à u buttone `Eseguisce`
- Arregistrà u schedariu cù u nome : `tb-android-_xxxxxxxx_-OmegaT.strings`

## Copia di i schedarii di lingua inglese

- Cupià o dispiazzà sti schedarii in u cartulare `source` di u prughjettu _Thunderbird for Android_ in _OmegaT_

## Ozzione o preferenze particulare à definisce in OmegaT

- Lancià l’appiecazione _OmegaT_
- Apre u prughjettu `Thunderbird for Android`
- Sceglie `Prughjettu` eppò `Pruprietà…`
- Fà un cliccu nant’à u buttone `Filtri lucali di schedariu…`
- Attivà l’ozzione `Impiegà i parametri di i filtri lucali di schedariu`
  - Verificà chì u furmatu `Risorse Android` hè attivatu
  - Verificà chì u furmatu `Testu` hè attivatu.  
  - Verificà l’ozzione di u furmatu `Testu` : 
          `Taglià u testu d’origine per fà paragrafi :`  
    - [x] `À ogni linea`
  - Verificà chì u furmatu `XLIFF` hè disattivatu
  - Verificà chì u furmatu `XLIFF files (Okapi)` hè attivatu
  - Verificà l’ozzioni di u furmatu `XLIFF files (Okapi)` :  
    ⚫ `Use the default filter settings (okf_xliff)`  
    ⚪ `Use the following filter parameter file:`
    - [x] `Include the name of the translation unit in comments`
    - [ ] `Show and protect entries with translate='no' (if not set: they are not extracted)`
    - [x] `Protect entries with state='final' (if not set: they can be edited)`

## Traduzzione in lingua corsa

- Lancià l’appiecazione _OmegaT_ è apre u prughjettu _Thunderbird for Android_ per traducelu

## Preparazione di i schedarii dopu a traduzzione

### Estensione .strings
Ci vole à appruntà __solu__ i schedarii cù l’estensione `.strings` chì si trovanu in u cartulare `target` di u prughjettu _VLC_ in _OmegaT_.
- Lancià _Notepad++_
- Apre tutti i schedarii cù l’estensione `.strings`
- Eseguisce a macro di cunversione `Cunversione OmegaT(.strings)-VLC(.strings)` installata pocu fà
- Arregistrà u schedariu cù u nome d’origine : `tb-android-_xxxxxxxx_.strings`

✔️ Ùn ci hè alcunu approntu à fà à l’altri furmati di schedariu di lingua corsa

## Incaricamentu di i schedarii di lingua corsa
- Tutti in schedarii tradutti in lingua corsa da _OmegaT_ si trovanu in u cartulare `target`
- Per ogni schedariu, ci vole à impiegà _Weblate_ cù l’ozzione `Téleverser un fichier` per rinfrescà u schedariu traduttu
