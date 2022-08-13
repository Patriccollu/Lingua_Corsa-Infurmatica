# Istruzzioni per impiegà _OmegaT_ per a traduzzione d’_HandBrake_

Per fà una traduzzione, l'appiecazione _OmegaT_ hà bisognu di schedarii di fonte cù una lingua sfarente di quella di destinazione. Di regula, a lingua di fonte hè l’inglese è quella di destinazione hè u corsu. D’altronde tutte e memorie di traduzzione pruviste nant’à stu situ sò in u sensu da l’inglese ver di u corsu.

Eccu l’istruzzioni per scaricà l’ultima versione di i schedarii di traduzzione è appruntalli per un trattamentu cù l’appiecazione _OmegaT_.

## Scaricamentu di i schedarii à traduce

- Eccu i liami per scaricà i schedarii in lingua inglese da _Transifex_ :
  - [Windows](https://www.transifex.com/HandBrakeProject/WinUI/language/en/)
  - [Mac](https://www.transifex.com/HandBrakeProject/mac-ui/language/en/)
  - [Linux](https://www.transifex.com/HandBrakeProject/linux-ui/language/en/)
- Per ogni risorsa :
  - Fà un cliccu nant’à u so nome per affissà tutte l’ozzioni
  - Sceglie l’ozzione `Télecharger le fichier pour le traduire`

- D’una manera alternativa, solu per Windows è Linux, si pò dinù scaricà i schedarii da _GitHub_ :
  - Windows : [Resources.resx](https://github.com/HandBrake/HandBrake/blob/master/win/CS/HandBrakeWPF/Properties/Resources.resx) è [ResourcesTooltips.resx](https://github.com/HandBrake/HandBrake/blob/master/win/CS/HandBrakeWPF/Properties/ResourcesTooltips.resx)
  - Linux : [ghb.pot](https://github.com/HandBrake/HandBrake/tree/master/gtk/po/ghb.pot)
  - Fà un cliccu drittu nant’à u buttone « _Raw_ » chì si trova à dritta, accant’à l’icone di u screnu, di a mina è di a curbella
  - Sceglie l’ozzione « _Arregistrà a sibula di a leia sottu…_ »

## Preparazione di i schedarii nanzu a traduzzione

### Estensione .resx

✔️ Ùn ci hè alcunu approntu à fà à i schedarii di stu furmatu

### Estensione .po
U schedariu `.po` scaricatu si chjama `for_translation_linux-ui_ghbpot_en.po`. Ghjè una versione in lingua inglese, vole si dì chì e catene di fonte è quelle di traduzzione sò treminduie in lingua inglese. Eccu l’istruzzioni per fane una versione in inglese impieghevule da _Omegat_.

- Lancià _Poedit_
- Sceglie l’ozzione `Schedariu` > `Apre…` o selezziunà l’azzione `Navigazione` nant’à u screnu di benvenuta
- Selezziunà u schedariu `.po` scaricatu
- Ci hè un messaghju dicendu : `A lingua di a traduzzione hè listessa chì quella d’origine`
- Cliccà nant’à u buttone `Currege a lingua`
- Indicà l’infurmazioni richieste in a finestra :
  - `Nome è versione di prughjettu`
  - `Squadra di traduzzione`
  - `Lingua` > __co__
  - `Forme plurale` > `Impiegà un espressione predefinita` > __nplurals=2; plural=(n > 1);__
- Cliccà nant’à u buttone `Vai`
- Selezziunà tutte e catene cù a cumanda `Ctrl-A` o cù l’ozzione `Mudificà` > `Tuttu selezziunà`
- Viutà u cuntenutu di e catene cù a cumanda `Ctrl-K` o cù l’ozzione `Mudificà` > `Viutà a traduzzione`
- Arregistrà u schedariu cù u nome : `for_omegat_linux-ui_ghbpot_en.po`

### Estensione .pot
S’ellu hè bisognu, eccu una manera di creà un schedariu `.po` viotu impieghendu u mudellu di schedariu di traduzzione in inglese (.POT)

- Lancià _Poedit_
- Sceglie l’ozzione `Schedariu` > `Novu da un schedariu POT/PO…` o slezziunà l’azzione `Creà nova…` nant’à u screnu di benvenuta
- Selezziunà u schedariu `ghb.pot` scaricatu
- In a finestra chì richiede a lingua di traduzzione, scrive `co`
- Tandu, sceglie l’ozzione `Catalogu` eppò `Pruprietà…`
- Indicà l’infurmazioni richieste :
  - `Nome è versione di u prughjettu`
  - `Squadra di traduzzione`
  - `Forme plurale` > `Impiegà un espressione predefinita` > __nplurals=2; plural=(n > 1);__
- Arregistrà u schedariu cù u nome : `for_omegat_linux-ui_ghbpot_en.po`

Sta manera alternativa pò dinù esse impiegata cusì per trasfurmà un altru schedariu di lingua - qualchissia a so lingua di destinazione, per indettu `fr.po` - in un novu schedariu viotu.

### Estensione .xliff
U schedariu `.xlf` scaricatu si chjama `for_translation_mac-ui_enxliff_en.xlf`. Ghjè una versione in lingua inglese, ma solu e catene di fonte sò in lingua inglese. Eccu l’istruzzioni per fane una versione in inglese impieghevule da _Omegat_.

- Lancià _Poedit_
- Sceglie l’ozzione `Schedariu` > `Apre…` o selezziunà l’azzione `Navigazione` nant’à u screnu di benvenuta
- Selezziunà u schedariu `.xlf` scaricatu
- Ci hè un messaghju dicendu : `A lingua di a traduzzione hè listessa chì quella d’origine`
- Cliccà nant’à u buttone `Currege a lingua`
- In a finestra chì richiede a lingua di traduzzione, scrive `co` è cliccà nant’à `Vai`
- Arregistrà u schedariu cù u nome : `for_omegat_mac-ui_enxliff_en.xlf`

## Copia di i schedarii di lingua inglese

- Cupià o dispiazzà i schedarii appruntati in u cartulare `source` di u prughjettu _HandBrake_ in _OmegaT_.

## Ozzione o preferenze particulare à definisce in OmegaT

- Lancià l’appiecazione _OmegaT_
- Sceglie `Ozzioni` eppò `Filtri di schedariu…`
  - Verificà chì u furmatu `XLIFF` hè disattivatu. 
  - Verificà chì u furmatu `ResX` hè attivatu. 
  - Verificà chì u furmatu `PO` hè attivatu.  
  - Verificà l’ozzioni di u furmatu `PO` :  
    - [x] `Permette e traduzzioni viote in i schedarii tradutti`
    - [ ] `Permette a traduzzione di i segmenti d’origine vioti`
    - [x] `Ignurà l’intestatura di i schedarii PO`
    - [ ] `Rimpiazzà autumaticamente « {nplurals=INTEGER; &plural=EXPRESSION;} » in l’intestatura`  
	      `Furmatu :` ⚫ `Classicu`   ⚪ `Monolinguale`
  - Verificà chì u furmatu `XLIFF files (Okapi)` hè attivatu.  
  - Verificà l’ozzioni di u furmatu `XLIFF files (Okapi)` :  
    ⚫ `Use the default filter settings (okf_xliff)`  
    ⚪ `Use the following filter parameter file:`
    - [x] `Include the name of the translation unit in comments`
    - [ ] `Show and protect entries with translate='no' (if not set: they are not extracted)`
    - [x] `Protect entries with state='final' (if not set: they can be edited)`

## Traduzzione in lingua corsa

- Lancià l’appiecazione _OmegaT_ è apre stu prughjettu per traducelu

## Preparazione di i schedarii dopu a traduzzione

✔️ Ùn ci hè alcunu approntu à fà à u schedariu di lingua corsa

## Incaricamentu di i schedarii di lingua corsa

Per què, ci vole à impiegà l’ozzione `Téleverser un fichier` di _Transifex_ per rinfrescà u schedariu di traduzzione.
