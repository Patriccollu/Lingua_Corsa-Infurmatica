# Istruzzioni per impiegà _OmegaT_ per a traduzzione di _paint.net_

Per fà una traduzzione, l'appiecazione _OmegaT_ hà bisognu di schedarii di fonte cù una lingua sfarente di quella di destinazione. Di regula, a lingua di fonte hè l’inglese è quella di destinazione hè u corsu. D’altronde tutte e memorie di traduzzione pruviste nant’à stu situ sò in u sensu da l’inglese ver di u corsu.

Eccu l’istruzzioni per scaricà l’ultima versione di u schedariu di traduzzione è appruntallu per un trattamentu cù l’appiecazione _OmegaT_.

## Scaricamentu di u schedariu à traduce

- U schedariu di lingua inglese si trova in quellu sottucartulare d’installazione di _paint.net_ :  
`C:\Program Files\paint.net\resx`

- Si pò scaricà u schedariu __in lingua corsa__ da quì :  
  https://crowdin.com/project/paintdotnet/co#

- Ci vole à cliccà nant’à l’icona chì riprisenta trè punti è sceglie un’azzione :
  - `Download` per scaricà un schedariu in u so furmatu `.resx` d’origine
  - `Download in XLIFF` per scaricà un schedariu cù u furmatu `.xliff` (**RICUMANDATU**)

- Ci vole à sapè ch’ellu si pò scaricà dinù [un schedariu compressu](https://crowdin.com/backend/download/project/paintdotnet.zip) chì cuntene u schedariu per ogni lingua è chì seria ghjuvevule per paragunà a traduzzione trà parechje lingue.

- Fate casu chì si pò accede à tutti sti liami nant’à _Crowdin_ solu s’è vo site cunnessi à u vostru contu _Crowdin_.

## Preparazione di u schedariu nanzu a traduzzione
Secondu u schedariu scaricatu, l’approntu hè più o menu faciule :
- Cù u schedariu `PaintDotNet.Strings.3.resx` scaricatu da u sottucartulare d’installazione di _paint.net_, ùn ci hè alcunu approntu
- Cù u schedariu `PaintDotNet.Strings.3.co.xliff` scaricatu da _Crowdin_ cù l’azzione `Download in XLIFF`, l’approntu hè faciule è l’istruzzioni si trovanu in u paragrafu chì seguita

### Estensione .xliff
- Lancià _Poedit_
- Sceglie l’ozzione `Schedariu` > `Apre…` o selezziunà l’azzione `Navigazione` nant’à u screnu di benvenuta
- Selezziunà u schedariu `.liff` scaricatu
- Verificà chì a lingua di destinazione sia `co` o `co_FR`
- Selezziunà tutte e catene cù a cumanda `Ctrl-A` o cù l’ozzione `Mudificà` > `Tuttu selezziunà`
- Viutà u cuntenutu di tutte ste catene cù a cumanda `Ctrl-K` o cù l’ozzione `Mudificà` > `Viutà a traduzzione`
- Arregistrà u schedariu cù u listessu nome

### Estensione .resx
- Ùn ci hè alcunu approntu s’è u schedariu `PaintDotNet.Strings.3.resx` hè statu scaricatu da u sottucartulare d’installazione di _paint.net_ perchè e catene sò tutte in lingua inglese
- Ma s’è u schedariu `PaintDotNet.Strings.3.co.resx` hè statu scaricatu da _Crowdin_ cù l’azzione `Download`, l’approntu ùn hè micca pussibule perchè e catene sò solu in lingua corsa

## Copia di u schedariu di lingua inglese

- Cupià o dispiazzà u schedariu approntatu - di furmatu `.resx` o `.xliff` - in u cartulare `source` di u prughjettu _paint.net_ in _OmegaT_.

## Ozzione o preferenze particulare à definisce in OmegaT

- Lancià l’appiecazione _OmegaT_
- Sceglie `Ozzioni` eppò `Filtri di schedariu…`
  - Verificà chì u furmatu `ResX` hè attivatu. 
  - Verificà chì u furmatu `XLIFF` hè disattivatu. 
  - Verificà chì u furmatu `XLIFF files (Okapi)` hè attivatu.  
  - Verificà l’ozzioni di u furmatu `XLIFF files (Okapi)` :  
    ⚫ `Use the default filter settings (okf_xliff)`  
    ⚪ `Use the following filter parameter file:`
    - [x] `Include the name of the translation unit in comments`
    - [ ] `Show and protect entries with translate='no' (if not set: they are not extracted)`
    - [x] `Protect entries with state='final' (if not set: they can be edited)`

## Traduzzione in lingua corsa

- Lancià l’appiecazione _OmegaT_ è apre stu prughjettu per traducelu.

## Preparazione di u schedariu dopu a traduzzione

Ùn ci hè nisunu approntu à fà à i schedarii.

## Incaricamentu di i schedarii di lingua corsa
- U schedariu traduttu in lingua corsa da _OmegaT_ si trova in u cartulare `target` di u prughjettu _paint.net_
- Ci vole à impiegà _Crowdin_ cù l’azzione `File` > `Upload Translations…` per rinfrescallu
