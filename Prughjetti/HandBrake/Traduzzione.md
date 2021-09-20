# A traduzzione in lingua corsa d’_HandBrake_

## Distribuzione
- A prima traduzzione in corsu hè stata distribuita per _Windows_ cù a versione 1.4.0 di lugliu di u 2021, è cù a versione 1.5.0 per _Linux_ è _MacOS_.
- L’installazione di u prugramma, nant’à _Windows_, chì impiega _NSIS_, si pò fà in lingua corsa
- Una cronolugia di tutte e mudificazioni si trova nant’à GitHub
  - Per Windows :
    - [Resources.resx](https://github.com/HandBrake/HandBrake/commits/master/win/CS/HandBrakeWPF/Properties/Resources.co.resx)
    - [ResourcesTooltips.resx](https://github.com/HandBrake/HandBrake/commits/master/win/CS/HandBrakeWPF/Properties/ResourcesTooltips.co.resx)
  - Per Linux :
    - [Resources.resx](https://github.com/HandBrake/HandBrake/commits/master/gtk/po/co.po)

## Traduttore
- Patriccollu di Santa Maria è Sichè

## Pagina ufficiale di u situ web nant’à a cuntribuzione è a traduzzione
- https://handbrake.fr/docs/en/latest/contributing/contribute.html

## Ciò ch’ella ci vole per traduce
- Richiestu
  - Un contu _Transifex_
  - Una dumanda nant’à _Transifex_ per participà à a traduzzione d’_HandBrake_
- Ricumandatu
  - _OmegaT_, prugramma per traduce i schedarii cù l’estensioni `.po`, `.resx` è `.xliff`
- Ozzionale
  - _Poedit_, prugramma per traduce i schedarii cù l’estensioni `.po` è `.xliff`
  - _Notepad++_, prugramma per mudificà un testu, paragunà duie versioni di testu, o trasfurmà u cuntenutu cù una prucedura pre-arregistrata

## I schedarii di lingua à traduce

- U furmatu di i schedarii di lingua hè sfarente secondu à u sistema :
  - `.po` per Linux
  - `.resx` per Windows
  - `.xliff` per Mac

### Situ officiale di traduzzione

- Tutti i schedarii di lingua - per ogni lingua dispunibule in _HandBrake_ - si trovanu nant’à _Transifex_ :
  - [Windows](https://www.transifex.com/HandBrakeProject/WinUI/languages/)
  - [Mac](https://www.transifex.com/HandBrakeProject/mac-ui/languages/)
  - [Linux](https://www.transifex.com/HandBrakeProject/linux-ui/languages/)

- Quelli per a lingua corsa si trovanu quì :  
  https://www.transifex.com/HandBrakeProject/dashboard/all_projects/co/  

- U dipositu di tutta a fonte d’_HandBrake_ si trova nant’à _GitHub_ :  
  https://github.com/HandBrake/HandBrake

### Situ di sviluppu

Secondu à u sistema, i schedarii di tutte e lingue tradutte si trovanu nant’à _GitHub_ :
- [Cartulare per Windows](https://github.com/HandBrake/HandBrake/tree/master/win/CS/HandBrakeWPF/Properties)
- [Cartulare per Mac](https://github.com/HandBrake/HandBrake/tree/master/macosx)
- [Cartulare per Linux](https://github.com/HandBrake/HandBrake/tree/master/gtk/po)

## Cumu sapè quandu ci hè qualcosa di novu à traduce ?

Quandu s’appronta una nova versione, a squadra d’_HandBrake_ mudificheghja e catene di fonte nant’à _Transifex_ aghjunghjendu catene nove o mudifichendu catene anziane. È quandu st’operazione si face, si riceve una nutificazione nant’à _Transifex_.  

## Cumu fà a traduzzione ?
Officialmente, _HandBrake_ prupone l’appiecazione _Transifex_ nant’à u Web per fà a traduzzione. Ma si pò quantunque impiegane un’altra in lucale per traduce.

### In linea
- Si pò impiegà stu metoda quandu ci hè __poca affare à traduce__.
- U scopu hè di cumpletà a traduzzione di i schedarii di lingua corsa
- A traduzzione si face direttamente in linea nant’à u situ _Transifex_ :
  - [Windows](https://www.transifex.com/HandBrakeProject/WinUI/language/co/)
  - [Mac](https://www.transifex.com/HandBrakeProject/mac-ui/language/co/)
  - [Linux](https://www.transifex.com/HandBrakeProject/linux-ui/language/co/)
- Per ogni sistema, ci vole à selezziunà una o duie risorse à traduce :
  - Windows : `Resources.resx` è `ResourcesTooltips.resx`
  - Mac : `en.xliff`
  - Linux : `ghb.pot`
- Per ogni schedariu, cliccà nant’à u buttone `Traduire`
- St’azzione currisponde à st’indirizzi :
  - Windows : [Resources.resx](https://www.transifex.com/HandBrakeProject/WinUI/translate/#co/resourcesresx) è [ResourcesTooltips.resx](https://www.transifex.com/HandBrakeProject/WinUI/translate/#co/resourcestooltipsresx)
  - Mac : [en.xliff](https://www.transifex.com/HandBrakeProject/mac-ui/translate/#co/enxliff)
  - Linux : [ghb.pot](https://www.transifex.com/HandBrakeProject/linux-ui/translate/#co/ghbpot)
- In a parte à manca di l’appiecazione, e catene - tradutte o micca - sò affissate in l’ordine alfabeticu ma si pò vede trè categurie : `Toutes`, `Non traduites` è `Non révisées`
- Cliccà nant’à a categuria `Non traduites` per fighjà solu e catene chì fermanu à traduce.
- L’appiecazione _Transifex_, grazia à a so memoria di traduzzione, hè capace di truvà e catene uguale o simile è di pruponele (fighjendu e _Suggestions_) per aiutavvi à traduce.

### In lucale
- Stu metoda hè piuttostu ricumandatu quandu ci hè __assai catene à traduce__.
- U scopu hè d’estrae i schedarii di traduzzione, di traduceli cù un’appiecazione lucale eppò di ricaricà i schedarii tradutti in lingua corsa.
- Secondu à l’estensione di schedariu, a traduzzione si pò fà cù l’appiecazioni _OmegaT_ o _Poedit_ chì sò capace treminduie, grazia à a so memoria di traduzzione, di truvà e catene uguale o simile è di vi e prupone per aiutavvi à traduce.
- A memoria di traduzzione di _Poedit_ hè nutrita da e traduzzioni di schedarii solu di furmatu `.po` o `.xliff` invece chì quella d’_OmegaT_ hè più maiò perchè ella cresce da e traduzzioni di schedarii di tutti i furmati.
- Dunque _Poedit_ serà piuttostu impiegatu per cumpletà a traduzzione d’un schedariu `.po` o `.xliff` dighjà principiata è _OmegaT_ serà ricumandatu per fà a traduzzione sana d’un schedariu di qualchì altru furmatu.
- Per disgrazia, e risorse Windows sò di furmatu `.resx` è dunque ùn ponu micca esse mudificate da _Poedit_. Per quelle risorse, ci vole à impiegà _OmegaT_.
- Per impiegà _OmegaT_, seguitate l’[istruzzioni per l’adopru di l’appiecazione _OmegaT_](OmegaT.md).
- Osinnò per cumpletà una traduzzione cù _Poedit_, ci vole à impiegà _Transifex_ per espurtà direttamente u schedariu di lingua corsa :
  - `en.xliff` https://www.transifex.com/HandBrakeProject/mac-ui/enxliff/co/download/for_translation/
  - `ghb.pot` https://www.transifex.com/HandBrakeProject/linux-ui/ghbpot/co/download/for_translation/
- Lancià _Poedit_ è apre u schedariu per traducelu eppò arregistrallu
- Dopu a traduzzione, hè ricumandatu d’impiegà _Transifex_ cù l’ozzione `Téleverser un fichier` per rinfrescà u schedariu di traduzzione.

## Istruzzioni per piglià in contu u novu schedariu in lingua corsa

Quandu i schedarii di lingua corsa sò stati rinfrescati nant’à _Transifex_, ùn ci hè più nunda à fà.
