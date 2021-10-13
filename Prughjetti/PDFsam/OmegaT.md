# Istruzzioni per impiegà _OmegaT_ per a traduzzione di _PDFsam_

Per fà una traduzzione, l'appiecazione _OmegaT_ hà bisognu di schedarii di fonte cù una lingua sfarente di quella di destinazione. Di regula, a lingua di fonte hè l’inglese è quella di destinazione hè u corsu. D’altronde tutte e memorie di traduzzione pruviste nant’à stu situ sò in u sensu da l’inglese ver di u corsu.

Eccu l’istruzzioni per scaricà l’ultima versione di i schedarii di traduzzione è appruntalli per un trattamentu cù l’appiecazione _OmegaT_.

## Scaricamentu di u schedariu à traduce

- Si pò scaricà u schedariu __in lingua corsa__ da quì :  
  https://translations.launchpad.net/pdfsam/pdfsam-v3/+pots/pdfsam/co/+translate
- St’azzione currisponde à st’indirizzu :  
  https://translations.launchpad.net/pdfsam/pdfsam-v3/+pots/pdfsam/co/+export

## Preparazione di u schedariu nanzu a traduzzione

- Lancià _Poedit_
- Sceglie l’ozzione `Schedariu` > `Apre…` o selezziunà l’azzione `Navigazione` nant’à u screnu di benvenuta
- Selezziunà u schedariu `.po` scaricatu
- Selezziunà tutte e catene cù a cumanda `Ctrl-A` o cù l’ozzione `Mudificà` > `Tuttu selezziunà`
- Viutà u cuntenutu di e catene cù a cumanda `Ctrl-K` o cù l’ozzione `Mudificà` > `Viutà a traduzzione`
- Arregistrà u schedariu cù u listessu nome : `omegat_PDFsam-en.po`

## Copia di u schedariu di lingua inglese

- Cupià o dispiazzà stu schedariu in u cartulare `source` di u prughjettu _PDFsam_ in _OmegaT_.

## Ozzione o preferenze particulare à definisce in OmegaT

- Lancià l’appiecazione _OmegaT_
- Sceglie `Ozzioni` eppò `Filtri di schedariu…`
  - Verificà chì u furmatu `PO` hè attivatu. 
  - Verificà l’ozzioni di u furmatu `PO` :  
    - [x] `Permette e traduzzioni viote in i schedarii tradutti`
    - [ ] `Permette a traduzzione di i segmenti d’origine vioti`
    - [x] `Ignurà l’intestatura di i schedarii PO`
    - [ ] `Rimpiazzà autumaticamente « {nplurals=INTEGER; &plural=EXPRESSION;} » in l’intestatura`  
	      `Furmatu :` ⚫ `Classicu`   ⚪ `Monolinguale`

## Traduzzione in lingua corsa

- Lancià l’appiecazione _OmegaT_ è apre u prughjettu _PDFsam_ per traducelu.

## Preparazione di u schedariu dopu a traduzzione

✔️ Ùn ci hè alcunu approntu à fà à u schedariu di lingua corsa.

## Incaricamentu di u schedariu di lingua corsa
- U schedariu traduttu in lingua corsa da _OmegaT_ si trova in u cartulare `target`
- Ci vole à impiegà _Launchpad_ per impurtacci u schedariu di traduzzione traduttu cù l’azzione `Upload translation`
