# Istruzzioni per impiegà _OmegaT_ per a traduzzione di _PDFCreator_

Per fà una traduzzione, l'appiecazione _OmegaT_ hà bisognu di schedarii di fonte cù una lingua sfarente di quella di destinazione. Di regula, a lingua di fonte hè l’inglese è quella di destinazione hè u corsu. D’altronde tutte e memorie di traduzzione pruviste nant’à stu situ sò in u sensu da l’inglese ver di u corsu.

Eccu l’istruzzioni per scaricà l’ultima versione di i schedarii di traduzzione è appruntalli per un trattamentu cù l’appiecazione _OmegaT_.

## Scaricamentu di i schedarii à traduce

- Si pò scaricà i schedarii da sta lista di prughjetti :  
  https://translate.pdfforge.org/languages/co_FR/  

- Per ogni prughjettu, ci vole à selezziunà un cumpunente nant’à a lista di i cumpunenti di u prughjettu
- Tandu, per ogni cumpunente, ci vole à selezziunallu, è cliccà nant’à `Fichiers` eppò `Télécharger le fichier de traduction d’origine (Fichier PO Gettext)`.

- Osinnò eccu l'indirizzi per scaricà direttamente tutti i schedarii di lingua :  

  - `Messages` https://translate.pdfforge.org/download/pdfcreator/messages/co_FR/
  - `Setup` https://translate.pdfforge.org/download/pdfcreator/setup/co_FR/
  - `Frontend` https://translate.pdfforge.org/download/pdfcreator-online/frontend/co_FR/

## Preparazione di i schedarii nanzu a traduzzione

I schedarii scaricati sò in lingua corsa, vole si dì ch’elli cuntenenu tutte e catene in lingua inglese è e so traduzzioni in lingua corsa. Eccu l’istruzzioni per fane una __versione di fonte in lingua inglese__.

- Lancià _Poedit_
- Sceglie l’ozzione `Schedariu` > `Apre…` o selezziunà l’azzione `Navigazione` nant’à u screnu di benvenuta
- Selezziunà u schedariu `.po` scaricatu
- Selezziunà tutte e catene cù a cumanda `Ctrl-A` o cù l’ozzione `Mudificà` > `Tuttu selezziunà`
- Viutà u cuntenutu di e catene cù a cumanda `Ctrl-K` o cù l’ozzione `Mudificà` > `Viutà a traduzzione`
- Arregistrà u schedariu cù u so nome :
  - `pdfcreator-messages-co_FR.po`
  - `pdfcreator-setup-co_FR.po`
  - `pdfcreator-online-frontend-co_FR.po`

## Copia di i schedarii di lingua inglese

- Cupià o dispiazzà sti schedarii in u cartulare `source` di u prughjettu _PDFCreator_ in _OmegaT_.

## Ozzione o preferenze particulare à definisce in OmegaT

- Lancià l’appiecazione _OmegaT_
- Sceglie `Ozzioni` eppò `Filtri di schedariu…`
  - Verificà l’ozzioni di u furmatu `PO` :  
    - [x] `Permette e traduzzioni viote in i schedarii tradutti`
    - [ ] `Permette a traduzzione di i segmenti d’origine vioti`
    - [x] `Ignurà l’intestatura di i schedarii PO`
    - [ ] `Rimpiazzà autumaticamente « {nplurals=INTEGER; &plural=EXPRESSION;} » in l’intestatura`  
	      `Furmatu :` ⚫ `Classicu`   ⚪ `Monolinguale`

## Traduzzione in lingua corsa

- Lancià l’appiecazione _OmegaT_ è apre stu prughjettu per traducelu.

## Preparazione di i schedarii dopu a traduzzione

✔️ Ùn ci hè alcunu approntu à fà à u schedariu di lingua corsa.

## Incaricamentu di i schedarii di lingua corsa

Dopu a traduzzione, ci vole à impiegà _pdfforge translate_ cù l’ozzione `Fichiers` eppò `Téleverser la traduction` per rinfrescà i schedarii di traduzzione cù quelli schedarii tradutti da _OmegaT_ chì si trovanu in u cartulare `target` di u prughjettu _PDFCreator_ :  
- `pdfcreator-messages-co_FR.po`
- `pdfcreator-setup-co_FR.po`
- `pdfcreator-online-frontend-co_FR.po`
