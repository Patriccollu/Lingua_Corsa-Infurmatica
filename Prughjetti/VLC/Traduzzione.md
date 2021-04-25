# A traduzzione in lingua corsa di _VLC Media Player_

## Distribuzione
### VLC for Windows
- A prima traduzzione in corsu hè stata distribuita cù a versione 3.0.0 di marzu di u 2021
- L’installazione di u prugramma, chì impiega _NSIS_, si pò fà in lingua corsa
- Una cronolugia di e mudificazioni si trova à st’indirizzu :
https://code.videolan.org/videolan/vlc/-/commits/master/po/co.po
### VLC for iOS
- A prima traduzzione in corsu hè stata distribuita cù a versione 3.1.3 d’uttobre di u 2018
- Una cronolugia di e mudificazioni si trova à st’indirizzi :
  - https://code.videolan.org/videolan/vlc-ios/-/commits/master/Apple-TV/Settings.bundle/co.lproj/Root.strings
  - https://code.videolan.org/videolan/vlc-ios/-/commits/master/Resources/Settings.bundle/co.lproj/Root.strings
  - https://code.videolan.org/videolan/vlc-ios/-/commits/master/Resources/co.lproj/InfoPlist.strings
  - https://code.videolan.org/videolan/vlc-ios/-/commits/master/Resources/co.lproj/Localizable.strings
### VLC for Android
- A prima traduzzione in corsu hè stata distribuita cù a versione 3.0.11 di maghju di u 2018
- Una cronolugia di e mudificazioni si trova à st’indirizzi :
  - https://code.videolan.org/videolan/vlc-android/-/commits/master/medialibrary/res/values-co/strings.xml
  - https://code.videolan.org/videolan/vlc-android/-/commits/master/application/resources/src/main/res/values-co/strings.xml

## Traduttori
- Patriccollu di Santa Maria è Sichè, Ghjuvan Pasquinu Castellani

## Pagina ufficiale di u situ web nant’à a traduzzione
- https://www.videolan.org/developers/i18n/

## Ciò ch’ella ci vole per traduce
- Richiestu
  - Un contu _Transifex_
- Ricumandatu
  - _OmegaT_, prugramma per traduce i schedarii cù l’estensioni `.po`, `.strings`, `.txt`, `.xlf` o `.xml`
  - _Poedit_, prugramma per mudificà i schedarii _gettext_ cù l’estensioni `.po`
  - _Notepad++_, prugramma per mudificà un testu è paragunà duie versioni d’un testu
- Ozzionale
  - Un iscrizzione à una lista di distribuzione di messaghju

## I schedarii di lingua à traduce

- U furmatu di i schedarii : `.po`, `.strings`, `.ts`, `.txt`, `.xhtml`, `.xlf` o `.xml`

- Tutti i schedarii di lingua - per ogni lingua dispunibule in _VLC_ - si trovanu nant’à [_Transifex_](https://www.transifex.com/yaron/vlc-trans/languages/).

- Quelli per a lingua corsa si trovanu quì :  
  https://www.transifex.com/yaron/vlc-trans/language/co/

## Cumu sapè quandu ci hè qualcosa di novu à traduce ?
Trà duie versioni, a squadra di _VLC_ mudificheghja e catene di fonte nant’à _Transifex_ aghjunghjendu catene nove, mudifichendu catene anziane, o ancu aghjughjendu un novu schedariu.  Quand’ella casca, ci hè una [nutificazione nant’à _Transifex_](https://www.transifex.com/notices/list/).

Ci hè dinù una [lista di tute e nutizie nant’à stu listessu situ](https://www.transifex.com/yaron/vlc-trans/announcements/).

## Cumu fà a traduzzione ?
- I traduttori devenu impiegà _Transifex_ ma a traduzzione si pò fà di parechje manere :
  - sia in linea, a traduzzione si face direttamente nant’à _Transifex_
  - sia in lucale nant’à u vostru urdinatore perchè _Transifex_ prupone funzioni per espurtà è impurtà i schedarii
  - in stu casu, a traduzzione si pò fà cù l’appiecazione _OmegaT_ chì hè capace, grazia à a so memoria di traduzzione, nutrita da e vostre traduzzioni, di truvà e catene uguale o simile è vi e prupone per aiutavvi à traduce.

### In linea
- Si pò impiegà stu metoda quandu ci hè __poca affare à traduce__.
- A traduzzione si face direttamente in linea nant’à u situ _Transifex_ :  
  https://www.transifex.com/yaron/vlc-trans/language/co/
- Ci vole à selezziunà una di e 18 risorse à traduce :
```
ANDROID android
TXT android (store, full description, 4000 max.)
TXT android (store, short description, 80 max.)
STRINGS iOS
STRINGS iOS (fastlane - keyword)
STRINGS iOS (fastlane - title)
STRINGS iOS (infoplist)
STRINGS iOS (settings)
PO VideoLAN.org - website
PO VLC 2.2 (outdated, won't be updated)
PO VLC 3.0
STRINGS VLC 3.0 (extra strings for macOS)
DESKTOP vlc.desktop
ANDROID VLC: NSIS installer
QT vlmc (not released soon)
XHTML VLSub (might be rewritten in JavaScript, not needing anymore)
TXT WinRT (store description)
XLIFF WinRT (xlf)
```
- Cliccà nant’à u buttone `Traduire`
- E catene - tradutte o micca - sò affissate in l’ordine alfabeticu ma si pò vede trè categurie : `Toutes`, `Non traduites` è `Non révisées`
- Cliccà nant’à a categuria `Non traduites` per fighjà solu e catene chì fermanu à traduce
- L’appiecazione _Transifex_, grazia à a so memoria di traduzzione, hè capace di truvà e catene uguale o simile è di pruponele (fighjendu e _Suggestions_) per aiutavvi à traduce.

### In lucale
- Stu metoda hè piuttostu ricumandatu quandu ci hè __assai catene à traduce__.
- U scopu hè d’estrae u schedariu di traduzzione, di traducelu cù un’appiecazione lucale eppò di ricaricà u schedariu traduttu in lingua corsa.
- A traduzzione si pò fà cù l’appiecazioni _OmegaT_ (per tutti i furmati) o _Poedit_ (solu per i schedarii `.po`) chì sò capace treminduie, grazia à a so memoria di traduzzione, di truvà e catene uguale o simile è di vi e prupone per aiutavvi à traduce.
- Per impiegà _OmegaT_, seguitate l’[istruzzioni per l’adopru di l’appiecazione _OmegaT_](OmegaT.md).
- Dopu a traduzzione, hè ricumandatu d’impiegà _Transifex_ cù l’ozzione `Téleverser un fichier` per rinfrescà u schedariu di traduzzione.

## Istruzzioni per piglià in contu u novu schedariu in lingua corsa

Quandu i schedarii di lingua corsa sò stati rinfrescati nant’à _Transifex_, ùn ci hè più nunda à fà.
