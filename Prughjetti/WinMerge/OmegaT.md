# Istruzzioni per impiegà _OmegaT_ per a traduzzione di _WinMerge_

Per fà una traduzzione, l'appiecazione _OmegaT_ hà bisognu di schedarii di fonte cù una lingua sfarente di quella di destinazione. Di regula, a lingua di fonte hè l’inglese è quella di destinazione hè u corsu. D’altronde tutte e memorie di traduzzione pruviste nant’à stu situ sò in u sensu da l’inglese ver di u corsu.

Eccu l’istruzzioni per scaricà l’ultima versione di i schedarii di traduzzione è appruntalli per un trattamentu cù l’appiecazione _OmegaT_.

## Scaricamentu di i schedarii à traduce

Si pò scaricà i schedarii __in lingua inglese__ da quì :  
- [per l’interfaccia](https://github.com/WinMerge/winmerge/blob/master/Translations/WinMerge/English.pot)
- [per u _Shell_](https://github.com/WinMerge/winmerge/blob/master/Translations/ShellExtension/English.pot)
- [per u stalladore](https://github.com/WinMerge/winmerge/blob/master/Translations/InnoSetup/English.isl)
- [per u schedariu _ReadMe_](https://github.com/WinMerge/winmerge/blob/master/Docs/Users/ReadMe.txt)
- [per u situ web](https://github.com/WinMerge/website/blob/master/po/en-US.pot)

S’ella hè bisognu, eccu l'indirizzi per scaricà i schedarii in __lingua corsa__ :  
- [per l’interfaccia](https://github.com/WinMerge/winmerge/tree/master/Translations/WinMerge/Corsican.po)
- [per u _Shell_](https://github.com/WinMerge/winmerge/tree/master/Translations/ShellExtension/Corsican.po)
- [per u stalladore](https://github.com/WinMerge/winmerge/tree/master/Translations/InnoSetup/Corsican.isl)
- [per u schedariu _ReadMe_](https://github.com/WinMerge/winmerge/blob/master/Translations/Docs/Readme/ReadMe-Corsican.txt)
- [per u situ web](https://github.com/WinMerge/website/tree/master/po/co.po)

## Preparazione di i schedarii nanzu a traduzzione

- Ci vole à appruntà i schedarii cù l’estensioni : `.po` è `.pot`
- Ùn ci hè nunda à fà per l’estensioni `.isl` è `.txt`

### Estensione .po
- Lancià _Poedit_
- Sceglie l’ozzione `Schedariu` > `Apre…` o selezziunà l’azzione `Navigazione` nant’à u screnu di benvenuta
- Selezziunà u schedariu `.po` scaricatu
- Selezziunà tutte e catene cù a cumanda `Ctrl-A` o cù l’ozzione `Mudificà` > `Tuttu selezziunà`
- Viutà u cuntenutu di e catene cù a cumanda `Ctrl-K` o cù l’ozzione `Mudificà` > `Viutà a traduzzione`
- Arregistrà u schedariu cù u nome : `for_omegat_winmerge_en.po`

### Estensione .pot
- Lancià _Poedit_
- Sceglie l’ozzione `Schedariu` > `Apre…` o selezziunà l’azzione `Navigazione` nant’à u screnu di benvenuta
- Selezziunà u schedariu `.pot` scaricatu
- Cliccà nant’à u buttone `Creà una nova traduzzione`
- Nant’à a finestra chì s’affissa, indicà : `lingua di traduzzione` > __co__ è chjodela
- Cliccà nant’ l’ozzione `Traduzzione` > `Pruprietà`
- Nant’à a finestra di chì s’affissa, indicà l’infurmazioni richieste :
  - `Nome è versione di u prughjettu`
  - `Squadra di traduzzione`
   - `Forme plurale` > `Impiegà un espressione predefinita` > __nplurals=2; plural=(n > 1);__
- Chjode a finestra cù u buttone `Vai`
- Arregistrà u schedariu cù u nome : `for_omegat_winmerge_en.po`

## Copia di i schedarii di lingua inglese

- Cupià o dispiazzà sti schedarii in u cartulare `source` di u prughjettu _WinMerge_ in _OmegaT_.

## Ozzione o preferenze particulare à definisce in OmegaT

- Lancià l’appiecazione _OmegaT_
- Sceglie `Ozzioni` eppò `Filtri di schedariu…`
  - Verificà chì u furmatu `Testu` hè attivatu. 
  - Verificà l’ozzione di u furmatu `Testu` : 
          `Taglià u testu d’origine per fà paragrafi :`  
    - [x] `À ogni linea`
  - Verificà chì u furmatu `Testu chjave=valore` hè attivatu
  - Verificà chì u furmatu `PO` hè attivatu. 
  - Verificà l’ozzioni di u furmatu `PO` :  
    - [x] `Permette e traduzzioni viote in i schedarii tradutti`
    - [ ] `Permette a traduzzione di i segmenti d’origine vioti`
    - [x] `Ignurà l’intestatura di i schedarii PO`
    - [ ] `Rimpiazzà autumaticamente « {nplurals=INTEGER; &plural=EXPRESSION;} » in l’intestatura`  
	      `Furmatu :` ⚫ `Classicu`   ⚪ `Monolinguale`

## Traduzzione in lingua corsa

- Lancià l’appiecazione _OmegaT_ è apre u prughjettu _WinMerge_ per traducelu.

## Preparazione di i schedarii dopu a traduzzione

✔️ Ùn ci hè alcunu approntu à fà à i schedarii di lingua corsa.

## Incaricamentu di i schedarii di lingua corsa
- Tutti in schedarii tradutti in lingua corsa da _OmegaT_ si trovanu in u cartulare `target`
- Per ogni schedariu mudificatu, ci vole à seguità l’[istruzzioni per piglià in contu u novu schedariu di lingua corsa](Traduzzione.md#istruzzioni-per-pigli%C3%A0-in-contu-u-novu-schedariu-di-lingua-corsa)
