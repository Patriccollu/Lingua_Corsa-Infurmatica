# Istruzzioni per impiegà _OmegaT_ per a traduzzione d’_Audacity_

Per fà una traduzzione, l'appiecazione _OmegaT_ hà bisognu di schedarii di fonte cù una lingua sfarente di quella di destinazione. Di regula, a lingua di fonte hè l’inglese è quella di destinazione hè u corsu. D’altronde tutte e memorie di traduzzione pruviste nant’à stu situ sò in u sensu da l’inglese ver di u corsu.

Eccu l’istruzzioni per scaricà l’ultima versione di i schedarii di traduzzione è appruntalli per un trattamentu cù l’appiecazione _OmegaT_.

## Scaricamentu di u schedariu à traduce

- Si pò scaricà a __versione attuale__ da dui lochi :
  - Nant’à [_GitHub_](https://github.com/audacity/audacity/blob/master/locale/co.po) si chjama `co.po`
    - Fà un cliccu drittu nant’à u buttone « _Raw_ » chì si trova à dritta, accant’à l’icone di u screnu, di a mina è di a curbella
    - Sceglie l’ozzione « _Arregistrà a sibula di a leia sottu…_ »
  - Nant’à [_Transifex_](https://www.transifex.com/klyok/audacity/audacity/co/download/for_translation/) si chjama `for_translation_audacity_audacity_co.po`
- A __versione di sviluppu__ si trova solu nant’à [_Transifex_](https://www.transifex.com/klyok/audacity/audacity-development/co/download/for_translation/) è si chjama `for_translation_audacity_audacity-development_co.po`

## Preparazione di u schedariu nanzu a traduzzione

U schedariu `.po` scaricatu hè una versione in lingua corsa, vole si dì ch’ellu cuntene tutte e catene in lingua inglese è e so traduzzioni in lingua corsa. Eccu l’istruzzioni per fane una __versione di fonte in lingua inglese__.

- Lancià _Poedit_
- Sceglie l’ozzione `Schedariu` > `Apre…` o selezziunà l’azzione `Navigazione` nant’à u screnu di benvenuta
- Selezziunà u schedariu `.po` scaricatu
- Selezziunà tutte e catene cù a cumanda `Ctrl-A` o cù l’ozzione `Mudificà` > `Tuttu selezziunà`
- Viutà u cuntenutu di e catene cù a cumanda `Ctrl-K` o cù l’ozzione `Mudificà` > `Viutà a traduzzione`
- Arregistrà u schedariu cù u nome : `Audacity.po`

Ci hè dinù una __manera alternativa__ di creà un schedariu `.po` viotu impieghendu u mudellu di schedariu di traduzzione in inglese (.POT)

- Scaricà u [mudellu di schedariu di traduzzione in inglese](https://github.com/audacity/audacity/blob/master/locale/audacity.pot) `audacity.pot`
  - Fà un cliccu drittu nant’à u buttone « _Raw_ » chì si trova à dritta, accant’à l’icone di u screnu, di a mina è di a curbella
  - Sceglie l’ozzione « _Arregistrà a sibula di a leia sottu…_ »
- Lancià _Poedit_
- Sceglie l’ozzione `Schedariu` > `Novu da un schedariu POT/PO…` o slezziunà l’azzione `Creà nova…` nant’à u screnu di benvenuta
- Selezziunà u schedariu `.pot` scaricatu
- In a finestra chì richiede a lingua di traduzzione, scrive `co`
- Tandu, sceglie l’ozzione `Catalogu` eppò `Pruprietà…`
- Indicà l’infurmazioni richieste :
  - `Nome è versione di u prughjettu`
  - `Squadra di traduzzione`
  - `Forme plurale` > `Impiegà un espressione predefinita` > __nplurals=2; plural=(n > 1);__
- Arregistrà u schedariu cù u nome : `Audacity.po`
  
## Copia di u schedariu di lingua inglese

- Cupià o dispiazzà stu schedariu `Audacity.po` in u cartulare `source` di u prughjettu _Audacity_ in _OmegaT_.

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

## Preparazione di i schedarii nanzu a traduzzione

✔️ Ùn ci hè alcunu approntu à fà à u schedariu di lingua corsa.

## Incaricamentu di i schedarii di lingua corsa

Ci vole à mandà u vostru schedariu di lingua corsa da un messaghju elettronicu perchè ùn ci hè alcuna azzione in linea per incaricallu. [Cliccà quì per sapene di più nant’à st’azzione](Traduzzione.md#istruzzioni-per-pigli%C3%A0-in-contu-u-novu-schedariu-in-lingua-corsa).  

Cum’è u corsu hè una di e lingue d’_Audacity_ amministrate nant’à _Transifex_, hè ricumandatu di rinfrescalla nant’à st’appiecazione cù l’ozzione `Téleverser un fichier`.
