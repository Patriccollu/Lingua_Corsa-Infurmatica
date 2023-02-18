# Istruzzioni per impiegà _OmegaT_ per a traduzzione di _Notepad++ _

Per fà una traduzzione, l'appiecazione _OmegaT_ hà bisognu di schedarii di fonte cù una lingua sfarente di quella di destinazione. Di regula, a lingua di fonte hè l’inglese è quella di destinazione hè u corsu. D’altronde tutte e memorie di traduzzione pruviste nant’à stu situ sò in u sensu da l’inglese ver di u corsu.

Eccu l’istruzzioni per scaricà l’ultima versione di u schedariu di traduzzione è appruntallu per un trattamentu cù l’appiecazione _OmegaT_.

## Scaricamentu di u schedariu à traduce

### L’interfaccia di _Notepad++_
- Si pò scaricà u schedariu __in lingua inglese__ da quì :  
  https://github.com/notepad-plus-plus/notepad-plus-plus/blob/master/PowerEditor/installer/nativeLang/english.xml

- Eccu u cartulare chì cuntene tutti i schedarii di lingua :  
  https://github.com/notepad-plus-plus/notepad-plus-plus/tree/master/PowerEditor/installer/nativeLang

- S’ella hè bisognu, si pò scaricà u schedariu in __lingua corsa__ da quì :  
  https://github.com/notepad-plus-plus/notepad-plus-plus/blob/master/PowerEditor/installer/nativeLang/corsican.xml

### U so cumpunente _wingup_
- Si pò scaricà u schedariu __in lingua inglese__ da quì :  
  https://github.com/notepad-plus-plus/wingup/blob/master/src/translations/english.xml

- Eccu u cartulare chì cuntene tutti i schedarii di lingua :  
  https://github.com/notepad-plus-plus/wingup/tree/master/src/translations

- S’ella hè bisognu, si pò scaricà u schedariu in __lingua corsa__ da quì :  
  https://github.com/notepad-plus-plus/wingup/blob/master/src/translations/corsican.xml

## Preparazione di u schedariu nanzu a traduzzione

Per disgrazia, u furmatu `.xml` di i schedarii di lingua di _Notepad++_ ùn sò micca ricunnisciuti da _OmegaT_, nè cù u so filtru d’origine, nè cù quelli di u pachettu _Okapi_. Dunque, ci vole à appruntallu via una prucedura di cunversione.  
  
In primu locu, ci vole à installà duie prucedure di cunversione. Per sapene di più, seguitate l’[istruzzioni per cunvertisce un schedariu di lingua](Cunversione.md) per ch’ellu sia accettatu da _OmegaT_.  

- Eppò lancià _Notepad++_
- Apre u schedariu `english.xml`
- Eseguisce a prucedura installata appostu chì si chjama :
  - `Cunversione Notepad(.xml)-OmegaT(.lng)` per _Notepad++_
  - `Cunversione Notepad_wingup(.xml)-OmegaT(.lng)` per u so cumpunente _wingup_
- Arregistrà u schedariu cù u nome `english.lng`

## Copia di u schedariu di lingua inglese

- Cupià o dispiazzà stu schedariu in u cartulare `source` di u prughjettu _Notepad++ _ in _OmegaT_

## Ozzione o preferenze particulare à definisce in OmegaT

- Lancià l’appiecazione _OmegaT_
- Sceglie `Ozzioni` eppò `Filtri di schedariu…`
  - Verificà chì u furmatu `XLIFF` hè disattivatu
  - Verificà chì u furmatu `Testu chjave=valore` hè attivatu

## Traduzzione in lingua corsa

- Lancià l’appiecazione _OmegaT_ è apre u prughjettu _Notepad++ _ per traducelu

## Preparazione di i schedarii dopu a traduzzione

⛔ Per disgrazia, ùn ci hè alcuna prucedura, à st’ora, per trasfurmà u cuntenutu di u schedariu da u furmatu `.lng` à u furmatu `.xml` d’origine

## Incaricamentu di u schedariu di lingua corsa

- Per fà st’operazione, seguitate [l’istruzzioni chì si trovanu à quellu capitulu](Traduzzione.md#istruzzioni-per-pigli%C3%A0-in-contu-u-novu-schedariu-di-lingua-corsa)
