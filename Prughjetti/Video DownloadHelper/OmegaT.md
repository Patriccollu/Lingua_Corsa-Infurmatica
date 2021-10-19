# Istruzzioni per impiegà _OmegaT_ per a traduzzione di _Video DownloadHelper_

Per fà una traduzzione, l'appiecazione _OmegaT_ hà bisognu di schedarii di fonte cù una lingua sfarente di quella di destinazione. Di regula, a lingua di fonte hè l’inglese è quella di destinazione hè u corsu. D’altronde tutte e memorie di traduzzione pruviste nant’à stu situ sò in u sensu da l’inglese ver di u corsu.

Eccu l’istruzzioni per scaricà l’ultima versione di u schedariu di traduzzione è appruntallu per un trattamentu cù l’appiecazione _OmegaT_.

## Scaricamentu di u schedariu à traduce

- Ci sò duie manere di scaricà u schedariu à traduce :
 1. Da u prugramma d’installazione in versione beta, impieghendu una prucedura di cunversione cù _Notepad++_
 2- Da a versione installata nant’à u vostru navigatore, senza installà alcuna prucedura di cunversione

### Da u prugramma d’installazione in versione beta
- Si pò scaricà l’ultima versione di u prugramma d’installazione in versione beta da quì :  
  https://www.downloadhelper.net/firefox/betas
- Cliccà nant’à u buttone `Install beta version vv.rr.mmm` induve `vv.rr.mmm` riprisente u numeru di versione, per indettu : `7.6.1a1`
- U prugramma scaricatu hè un schedariu cumpressu chì si chjama `video_downloadhelper-vv.rr.mmm-an+fx.xpi`
- Si pò impiegà u prugramma _7-Zip_ per apre stu schedariu cumpressu è estrae i schedarii chì si trovanu dentru
- U schedariu __in lingua inglese__ si chjama `messages.json` è si trova in u cartulare `\_locales\en_US\`
- Lancià _Notepad++_
- Apre u schedariu `messages.json`
- Seguitate l’[istruzzioni per installà una prucedura di cunversione specifica](Cunversione.md)
- Eseguisce a prucedura installata appostu per fà sta cunversione
- Arregistrà u schedariu cù u nome : `omegat_messages.json`

- S’ella hè bisognu, ci hè dinù un schedariu in __lingua corsa__ chì si chjama `messages.json` è chì si trova in u cartulare `\_locales\co\`

### Da a versione installata nant’à u vostru navigatore
- Lancià _Video DownloadHelper_ __in lingua inglese__ è espurtà u schedariu di sta manera
- Fà un cliccu dirittu nant’à l’icona di l’interfaccia
- Sceglie : `Preferences` > `Plus…` > `Traduction`
- Fà un cliccu nant’à u buttone `Export`

## Copia di u schedariu di lingua inglese

- Cupià o dispiazzà u schedariu à traduce in u cartulare `source` di u prughjettu _Video DownloadHelper_ in _OmegaT_.

## Ozzione o preferenze particulare à definisce in OmegaT

- Lancià l’appiecazione _OmegaT_
- Sceglie `Ozzioni` eppò `Filtri di schedariu…`
  - Verificà chì u furmatu `JSON files (Okapi)` hè attivatu. 
  - Verificà l’ozzioni di u furmatu `JSON files (Okapi)` :  
    ⚫ `Use the default filter settings (okf_json)`  
    ⚪ `Use the following filter parameter file:`
    - [x] `Include the name of the translation unit in comments`

## Traduzzione in lingua corsa

- Lancià l’appiecazione _OmegaT_ è apre u prughjettu _Video DownloadHelper_ per traducelu.

## Preparazione di i schedarii dopu a traduzzione

✔️ Ùn ci hè alcunu approntu à fà à u schedariu di lingua corsa.

## Incaricamentu di i schedarii di lingua corsa
- Tutti i schedarii tradutti in lingua corsa da _OmegaT_ si trovanu in u cartulare `target` di u prughjettu
- Quandu u schedariu di lingua corsa hè prontu, ci vole à fà un postu nant’à u [foru di traduzzione di _Video DownloadHelper_](https://groups.google.com/g/video-downloadhelper-internationalization) è mette u schedariu `message.json` in pezza aghjunta.
