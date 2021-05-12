# Istruzzioni per impiegà _OmegaT_ per a traduzzione di _Poedit_

Per fà una traduzzione, l'appiecazione _OmegaT_ hà bisognu di schedarii di fonte cù una lingua sfarente di quella di destinazione. Di regula, a lingua di fonte hè l’inglese è quella di destinazione hè u corsu. D’altronde tutte e memorie di traduzzione pruviste nant’à stu situ sò in u sensu da l’inglese ver di u corsu.

Eccu l’istruzzioni per scaricà l’ultima versione di i schedarii di traduzzione è appruntalli per un trattamentu cù l’appiecazione _OmegaT_.

## Scaricamentu di i schedarii à traduce

À st'ora, ci hè 7 schedarii, di furmatu sfarente, chì cuntenenu a traduzzione di _Poedit_ per e piattaforme Mac, Linux è Windows. I furmati di schedariu sò : `.strings`, `.po`, `.rc`, `.csv` è `.xliff`.  

Si pò scaricà a versione attuale da [_Crowdin_](https://crowdin.com/project/poedit/co#). Per ogni schedariu :
- Selezziunà un schedariu cù un cliccu nant’à u so nome
- Cliccà nant’à l’icona cù trè tratti orizuntale - ciò chì si chjama u listinu « _hamburger_ » - accant’à CORSICAN insù è à manca
- In a rubrica `File`, sceglie `Download`
- Arregistrà u schedariu in un cartulare timpurariu

Nota : Per u schedariu `MainToolbar.xliff` a prucedura hè un pocu sfarente :
- Selezziunà u schedariu cù un cliccu nant’à u nome `Mac toolbar (duplicates with normal file)`
- Cliccà nant’à l’icona cù trè tratti orizuntale - ciò chì si chjama u listinu « _hamburger_ » - accant’à CORSICAN insù è à manca
- In a rubrica `File`, sceglie `Download in XLIFF`
- Arregistrà u schedariu in un cartulare timpurariu

## Preparazione di u schedariu nanzu a traduzzione

- Ci vole à appruntà i schedarii cù l’estensioni : `.po` è `.xliff`
- Ùn ci hè nunda à fà per l’estensioni `.csv`, `.rc` è `.strings`

### Estensioni .po è xliff
I schedarii scaricati sò una versione in lingua corsa, vole si dì ch’elli cuntenenu tutte e catene in lingua inglese è ancu e so traduzzioni in lingua corsa. Eccu l’istruzzioni per fane una versione di fonte in lingua inglese.

- Lancià _Poedit_
- Sceglie l’ozzione `Schedariu` > `Apre…` o selezziunà l’azzione `Navigazione` nant’à u screnu di benvenuta
- Selezziunà u schedariu `.po` o `.xliff` scaricatu
- Selezziunà tutte e catene cù a cumanda `Ctrl-A` o cù l’ozzione `Mudificà` > `Tuttu selezziunà`
- Viutà u cuntenutu di e catene cù a cumanda `Ctrl-K` o cù l’ozzione `Mudificà` > `Viutà a traduzzione`
- Arregistrà u schedariu cù u listessu nome

## Copia di u schedariu di lingua inglese

- Cupià o dispiazzà sti schedarii in u cartulare `source` di u prughjettu _Poedit_ in _OmegaT_.

## Ozzione o preferenze particulare à definisce in OmegaT

- Lancià l’appiecazione _OmegaT_
- Sceglie `Ozzioni` eppò `Filtri di schedariu…`
  - Verificà l’ozzioni di u furmatu `PO` :  
    - [x] `Permette e traduzzioni viote in i schedarii tradutti`
    - [ ] `Permette a traduzzione di i segmenti d’origine vioti`
    - [x] `Ignurà l’intestatura di i schedarii PO`
    - [ ] `Rimpiazzà autumaticamente « {nplurals=INTEGER; &plural=EXPRESSION;} » in l’intestatura`  
	      `Furmatu :` ⚫ `Classicu`   ⚪ `Monolinguale`
  - Verificà l’ozzioni di u furmatu `XLIFF files (Okapi)` :  
    ⚫ `Use the default filter settings (okf_xliff)`  
    ⚪ `Use the following filter parameter file:`
    - [x] `Include the name of the translation unit in comments`
    - [ ] `Show and protect entries with translate='no' (if not set: they are not extracted)`
    - [x] `Protect entries with state='final' (if not set: they can be edited)`

## Traduzzione in lingua corsa

- Lancià l’appiecazione _OmegaT_ è apre stu prughjettu per traducelu.

## Preparazione di i schedarii dopu a traduzzione

✔️ Ùn ci hè alcunu approntu à fà à i schedarii di lingua corsa.

## Incaricamentu di i schedarii di lingua corsa

- Tutti in schedarii tradutti in lingua corsa da _OmegaT_ si trovanu in u cartulare `target`
- Per ogni schedariu, ci vole à impiegà _Crowdin_ cù l’ozzione `File` > `Upload Translations…` per rinfrescà u schedariu traduttu
