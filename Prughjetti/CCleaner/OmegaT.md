# Istruzzioni per impiegà _OmegaT_ per a traduzzione di _CCleaner_

Per fà una traduzzione, l'appiecazione _OmegaT_ hà bisognu di schedarii di fonte cù una lingua sfarente di quella di destinazione. Di regula, a lingua di fonte hè l’inglese è quella di destinazione hè u corsu. D’altronde tutte e memorie di traduzzione pruviste nant’à stu situ sò in u sensu da l’inglese ver di u corsu.

Eccu l’istruzzioni per scaricà l’ultima versione di i schedarii di traduzzione è appruntalli per un trattamentu cù l’appiecazione _OmegaT_.

## Scaricamentu di i schedarii à traduce

- Si pò scaricà i schedarii __in lingua corsa__ da quì :  
  https://crowdin.com/project/avast-ccleaner/co#

- À st’ora, ci hè trè schedarii :
  - `res_uk_recuva.rc` Aghjuntu per _Recuva_
  - `lang_uk.nsh` Stalladore NSIS
  - `res_uk.rc` Interfaccia di _CCleaner_
  
- Per ogni schedariu, ci vole à cliccà nant’à l’icona chì riprisenta trè punti è sceglie un’azzione :
  - `Download` per scaricà un schedariu in u so furmatu d’origine
  - `Export in XLIFF` per scaricà un schedariu cù u furmatu `.xliff` (**RICUMANDATU**)

- S’ella hè bisognu, si pò scaricà un schedariu `.zip` chì cuntene i trè schedarii in __lingua inglese__ da quì :  
  https://crowdin.com/backend/download/project/avast-ccleaner/enp.zip

- Si pò scaricà dinù [un altru schedariu compressu](https://crowdin.com/backend/download/project/avast-ccleaner.zip) chì cuntene i trè schedarii **per ogni lingua**

## Preparazione di i schedarii nanzu a traduzzione

- Hè **ricumandatu** di scaricà i schedarii in u furmatu `.xliff` perchè l’approntu hè più faciule
- À st’ora, _OmegaT_ ùn pò micca traduce direttamente i schedarii cù l’estensioni `.nsh` è `.rc`
- Ma, per furtuna, si pò [installà è impiegà e prucedure di cunversione](Cunversione.md) per trasfurmà u so cuntenutu

### Estensione .xliff
- Lancià _Poedit_
- Sceglie l’ozzione `Schedariu` > `Apre…` o selezziunà l’azzione `Navigazione` nant’à u screnu di benvenuta
- Selezziunà u schedariu `.xliff` scaricatu pocu fà
- Verificà chì a lingua di destinazione sia `co` o `co_FR`
- Selezziunà tutte e catene cù a cumanda `Ctrl-A` o cù l’ozzione `Mudificà` > `Tuttu selezziunà`
- Viutà u cuntenutu di tutte ste catene cù a cumanda `Ctrl-K` o cù l’ozzione `Mudificà` > `Viutà a traduzzione`
- Arregistrà u schedariu cù u listessu nome

### Estensione .nsh
- Lancià _Notepad++_
- Apre u schedariu `lang_uk.nsh` scaricatu pocu fà
- Eseguisce a macro installata appostu chì si chjama `Cunversione_CCleaner_NSH-OmegaT`
- Arregistrà u schedariu cù u nome `lang_uk.nsh.lng`

### Estensione .rc
- Lancià _Notepad++_
- Apre u schedariu `res_uk.rc` o `res_uk_recuva.rc` scaricatu pocu fà
- Eseguisce a macro installata appostu chì si chjama `Cunversione_CCleaner_RC-OmegaT`
- Arregistrà u schedariu cù u nome `res_uk.rc.lng` o `res_uk_recuva.rc.lng`

## Copia di i schedarii di lingua inglese

- Cupià o dispiazzà sti schedarii in u cartulare `source` di u prughjettu _CCleaner_ in _OmegaT_

## Ozzione o preferenze particulare à definisce in OmegaT

- Lancià l’appiecazione _OmegaT_
- Sceglie `Ozzioni` eppò `Filtri di schedariu…`
  - Verificà l’ozzioni di u furmatu `XLIFF files (Okapi)` :  
    ⚫ `Use the default filter settings (okf_xliff)`  
    ⚪ `Use the following filter parameter file:`
    - [x] `Include the name of the translation unit in comments`
    - [ ] `Show and protect entries with translate='no' (if not set: they are not extracted)`
    - [x] `Protect entries with state='final' (if not set: they can be edited)`

## Traduzzione in lingua corsa

- Lancià l’appiecazione _OmegaT_ è apre stu prughjettu per traducelu

## Preparazione di i schedarii dopu a traduzzione

- Tutti in schedarii tradutti in lingua corsa da _OmegaT_ si trovanu in u cartulare `target` di u prughjettu _CCleaner_

### Estensione .xliff

✔️ Ùn ci nisunu approntu à fà per i schedarii cù l’estensione `.xliff`

### Estensione .nsh
- Lancià _Notepad++_
- Apre u schedariu `lang_uk.nsh.lng` chì si trova in u cartulare `target` di u prughjettu _CCleaner_
- Eseguisce a macro installata appostu chì si chjama `Cunversione_OmegaT-CCleaner_NSH`
- Arregistrà u schedariu cù u nome `lang_uk.nsh`

### Estensione .rc
- Lancià _Notepad++_
- Apre u schedariu `res_uk.rc.lng` o `res_uk_recuva.rc.lng` chì si trovanu in u cartulare `target` di u prughjettu _CCleaner_
- Eseguisce a macro installata appostu chì si chjama `Cunversione_OmegaT-CCleaner_RC`
- Arregistrà u schedariu cù u nome `res_uk.rc` o `res_uk_recuva.rc`

## Incaricamentu di i schedarii di lingua corsa
- Per ogni schedariu traduttu è appruntatu, ci vole à impiegà _Crowdin_ via l’azzione `File` > `Upload Translations…` per rinfrescallu
