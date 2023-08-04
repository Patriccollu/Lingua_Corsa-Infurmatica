# Istruzzioni per impiegà _OmegaT_ per a traduzzione di _VLC Media Player_

Per fà una traduzzione, l'appiecazione _OmegaT_ hà bisognu di schedarii di fonte cù una lingua sfarente di quella di destinazione. Di regula, a lingua di fonte hè l’inglese è quella di destinazione hè u corsu. D’altronde tutte e memorie di traduzzione pruviste nant’à stu situ sò in u sensu da l’inglese ver di u corsu.

Eccu l’istruzzioni per scaricà l’ultima versione di i schedarii di traduzzione è appruntalli per un trattamentu cù l’appiecazione _OmegaT_.

## Scaricamentu di i schedarii à traduce

- Si pò scaricà i schedarii __in lingua inglese__ da quì :  
  https://www.transifex.com/yaron/vlc-trans/language/en/

- Eccu l'indirizzi per scaricà tutti i schedarii di lingua :  

	https://www.transifex.com/yaron/vlc-trans/android/en/download/for_translation/  
	https://www.transifex.com/yaron/vlc-trans/android-store-fulldescription/en/download/for_translation/  
	https://www.transifex.com/yaron/vlc-trans/android-store-shortdescription/en/download/for_translation/  
	https://www.transifex.com/yaron/vlc-trans/ios/en/download/for_translation/  
	https://www.transifex.com/yaron/vlc-trans/ios-fastlane-keyword/en/download/for_translation/  
	https://www.transifex.com/yaron/vlc-trans/ios-fastlane-title/en/download/for_translation/  
	https://www.transifex.com/yaron/vlc-trans/ios-infoplist/en/download/for_translation/  
	https://www.transifex.com/yaron/vlc-trans/ios-settings/en/download/for_translation/  
	https://www.transifex.com/yaron/vlc-trans/vlc_website/en/download/for_translation/  
	https://www.transifex.com/yaron/vlc-trans/vlc-22/en/download/for_translation/  
	https://www.transifex.com/yaron/vlc-trans/vlc-30/en/download/for_translation/  
	https://www.transifex.com/yaron/vlc-trans/vlc-30-extra-strings-for-macos/en/download/for_translation/  
	https://www.transifex.com/yaron/vlc-trans/vlc-desktop/en/download/for_translation/  
	https://www.transifex.com/yaron/vlc-trans/vlc-installer/en/download/for_translation/  
	https://www.transifex.com/yaron/vlc-trans/vlmc/en/download/for_translation/  
	https://www.transifex.com/yaron/vlc-trans/vlsub/en/download/for_translation/  
	https://www.transifex.com/yaron/vlc-trans/winrt-store-description/en/download/for_translation/  
	https://www.transifex.com/yaron/vlc-trans/winrt-xlf/en/download/for_translation/  

- S’ella hè bisognu, si pò scaricà i schedarii in __lingua corsa__ da quì :  
  https://www.transifex.com/yaron/vlc-trans/language/co/

- Tutti i schedarii scaricati anu un nome chì principià cù `for_translation_vlc-trans_xxxxx-yyyyy_en.`

## Preparazione di i schedarii nanzu a traduzzione
- Ùn ci hè nunda à fà à i schedarii cù l’estensioni `.txt` è `.xml`
- Ci vole à appruntà i schedarii cù l’estensioni : `.po`, `.strings`, è `.xlf`
- À st’ora, _OmegaT_ ùn pò micca traduce i schedarii cù l’estensioni `.desktop`, `.ts` è `.xhtml`

### Estensione .po
U schedariu `.po` scaricatu hè una versione in lingua inglese, vole si dì chì e catene di fonte è quelle di traduzzione sò treminduie in lingua inglese. Eccu l’istruzzioni per fane una versione in inglese impieghevule da _Omegat_.

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
- Arregistrà u schedariu cù u nome : `for_omegat_vlc-trans_xxxxx-yyyyy_en.po`

### Estensione .strings
- Lancià _Notepad++_
- Installà e prucedure di cunversione cum’è indicatu in [st’istruzzioni detagliate](Cunversione.md)
- Apre __tutti i schedarii__ cù l’estensione : `.strings`
- Sceglie `Macro`, eppò `Eseguisce una macro parechje volte…`
- Selezziunà u nome di a prucedura à impiegà : `Cunversione VLC(.strings)-OmegaT(.strings)`
- Cliccu nant’à `Eseguisce 1 volta`
- Appughjà nant’à u buttone `Eseguisce`
- Quandu s’impiegherà sta prucedura, viderete 3 volte u messaghju quì sottu è ci vulerà à risponde OK :  
  `Vulete rimpiazzà tutte l’occurrenze in tutti i schedarii aperti ?`
- Fate casu chì a cunversione si face in __tutti i schedarii__ cù l’estensione `.strings` aperti in una sessione di _Notepad++_. S’ellu hè bisognu, si pò apre una seconda sessione _Notepad++_
- Arregistrà u schedariu cù u nome : `for_omegat_vlc-trans_xxxxx-yyyyy_en.strings`

### Estensione .xlf
- Lancià _Poedit_
- Sceglie l’ozzione `Schedariu` > `Apre…` o selezziunà l’azzione `Navigazione` nant’à u screnu di benvenuta
- Selezziunà u schedariu `.xlf` scaricatu
- Cliccà nant’à u buttone `Definisce a lingua`
- In a finestra chì richiede a lingua di traduzzione, scrive `co`
- Arregistrà u schedariu cù u nome : `for_omegat_vlc-trans_xxxxx-yyyyy_en.xlf`

## Copia di i schedarii di lingua inglese

- Cupià o dispiazzà i schedarii appruntati in u cartulare `source` di u prughjettu _VLC_ in _OmegaT_.

## Ozzione o preferenze particulare à definisce in OmegaT

- Lancià l’appiecazione _OmegaT_
- Sceglie `Ozzioni` eppò `Filtri di schedariu…`
  - Verificà chì u furmatu `XLIFF` hè disattivatu. 
  - Verificà chì u furmatu `Testu` hè attivatu.  
  - Verificà l’ozzione di u furmatu `Testu` : 
          `Taglià u testu d’origine per fà paragrafi :`  
    - [x] `À ogni linea`
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

- Lancià l’appiecazione _OmegaT_ è apre stu prughjettu per traducelu.

## Preparazione di i schedarii dopu a traduzzione
Ci vole à appruntà __solu__ i schedarii cù l’estensione `.strings` chì si trovanu in u cartulare `target` di u prughjettu _VLC_ in _OmegaT_.
- Lancià _Notepad++_
- Apre tutti i schedarii cù l’estensione `.strings`
- Eseguisce a macro di cunversione `Cunversione OmegaT(.strings)-VLC(.strings)` installata pocu fà
- Fate casu chì a cunversione si face in tutti i schedarii cù l’estensione `.strings` aperti in a sessione di _Notepad++_
- Arregistrà u schedariu cù u listessu nome : `for_omegat_vlc-trans_xxxxx-yyyyy_en.strings`

## Incaricamentu di i schedarii di lingua corsa
- Tutti in schedarii tradutti in lingua corsa da _OmegaT_ si trovanu in u cartulare `target`
- Per ogni schedariu, ci vole à impiegà _Transifex_ cù l’ozzione `Téleverser un fichier` per rinfrescà u schedariu traduttu
