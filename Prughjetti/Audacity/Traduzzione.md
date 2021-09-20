# A traduzzione in lingua corsa d’_Audacity_

## Distribuzione
- A prima traduzzione in corsu hè stata distribuita cù a versione 3.0.0 di marzu di u 2021
- L’installazione di u prugramma, chì impiega _Inno Setup_, si pò fà in lingua corsa
- Una [cronolugia di tutte e mudificazioni](https://github.com/audacity/audacity/commits/master/locale/co.po) si trova nant’à GitHub

## Traduttore
- Patriccollu di Santa Maria è Sichè

## Pagina ufficiale di u situ web nant’à a traduzzione
- https://www.audacityteam.org/community/translators/

## Ciò ch’ella ci vole per traduce
- Richiestu
  - Un iscrizzione à una lista di distribuzione di messaghju
  - Un prugramma per traduce - è esse capace di mudificà - i schedarii _gettext_ cù l’estensioni `.po` o `.pot`, per indettu : _Poedit_ o _OmegaT_
- Ozzionale
  - Un contu _Transifex_
  - _Notepad++_, prugramma per mudificà un testu

## I schedarii di lingua à traduce

U dipositu di tutta a fonte d’_Audacity_ si trova nant’à GitHub :  
   https://github.com/audacity/audacity  

I schedarii di tutte e lingue tradutte si trovanu in u cartulare [/locale/.](https://github.com/audacity/audacity/tree/master/locale)

- U furmatu di i schedarii : `.po`
- A fonte d’origine : [audacity.pot](https://github.com/audacity/audacity/blob/master/locale/audacity.pot)
- U schedariu di lingua corsa : [co.po](https://github.com/audacity/audacity/blob/master/locale/co.po)

Ci hè dinù un altru locu - ind’è [_Transifex_](https://www.transifex.com/klyok/audacity/language/co/) - induve si pò truvà parechje versione di u schedariu di lingua corsa :
- `Audacity master (development version, updated daily)` hè a versione di sviluppu, quella chì pò cambià à ogni mumentu è chì diventerà a prossima versione
- `Audacity master (string freeze version)` hè una copia di a versione attuale
- Un altra versione, cum’è, per indettu, `Audacity release-3.0.3`

## Cumu sapè quandu ci hè qualcosa di novu à traduce ?
Ci vole à abbunassi à sta lista di distribuzione di messaghju : [audacity-translation mailing list](https://lists.sourceforge.net/lists/listinfo/audacity-translation)  

Quandu ci hè una nova versione cù nove catene à traduce, a squadra d’_Audacity_ manda un messaghju - una o duie settimane nanzu a data d’esciuta prevista - à tutti i traduttori chì sò iscritti nant’à a lista di distribuzione.

- In stu casu, [i schedarii di lingue nant’à _GitHub_](https://github.com/audacity/audacity/blob/master/locale/) cuntenenu tutti :
  - l’anziane catene dighjà tradutte (ghjè a maiò parte)
  - e nove catene a traduce
- Di più, [per e lingue amministrate nant’à _Transifex_](https://www.transifex.com/klyok/audacity/dashboard/), cum’è a lingua corsa, a versione attuale hè uguale à a versione di sviluppu.  

Ma pocu à pocu, trà duie versione d’_Audacity_, a versione di sviluppu cambia. S’è vo avete un contu _Transifex_, ci hè una nutificazione mandata à ogni cambiamentu. È cusì, manu manu, ghjè pussibule di traduce e catene chì seranu in a prossima versione, invece d’aspettà u messaghju di cambiamentu di versione da a squadra d’_Audacity_. Di sta manera, a traduzzione di e nove catene si face pianu pianu è quandu s’affaca a nova versione, u vostru schedariu di lingua hè guasi prontu.

## Cumu fà a traduzzione ?
Officialmente, _Audacity_ ùn prupone alcuna appiecazione - lucale o nant’à u Web - per fà a traduzzione. Ma si pò quantunque impiegà _Transifex_ per traduce. St’appiecazione in linea hè capace, grazia à a so memoria di traduzzione, di truvà e catene uguale o simile è vi e prupone per aiutavvi à traduce.

### In linea
- Si pò impiegà stu metoda quandu ci hè __poca affare à traduce__.
- A traduzzione si face direttamente in linea nant’à u situ _Transifex_ :  
  https://www.transifex.com/klyok/audacity/language/co/
- Ci vole à selezziunà una risorsa à traduce : `Audacity master (development)` o `Audacity master`
- Cliccà nant’à u buttone `Traduire`
- St’azzione currisponde à st’indirizzi :
  - `Audacity master (development version, updated daily)` https://www.transifex.com/klyok/audacity/translate/#co/audacity-master-development
  - `Audacity master (string freeze version)` https://www.transifex.com/klyok/audacity/translate/#co/audacity-master
- In a parte à manca di l’appiecazione, e catene - tradutte o micca - sò affissate in l’ordine alfabeticu ma si pò vede trè categurie : `Toutes`, `Non traduites` è `Non révisées`
- Cliccà nant’à a categuria `Non traduites` per fighjà solu e catene chì fermanu à traduce.
- L’appiecazione _Transifex_, grazia à a so memoria di traduzzione, hè capace di truvà e catene uguale o simile è di pruponele (fighjendu e _Suggestions_) per aiutavvi à traduce.

### In lucale
- Stu metoda hè piuttostu ricumandatu quandu ci hè __assai catene à traduce__.
- U scopu hè d’estrae u schedariu di traduzzione, di traducelu cù un’appiecazione lucale eppò di ricaricà u schedariu traduttu in lingua corsa.
- A traduzzione si pò fà cù l’appiecazioni _Poedit_ o _OmegaT_ chì sò capace treminduie, grazia à a so memoria di traduzzione, di truvà e catene uguale o simile è di vi e prupone per aiutavvi à traduce.
- A memoria di traduzzione di _Poedit_ hè nutrita da e traduzzioni di schedarii solu di furmatu `.po` invece chì quella d’_OmegaT_ hè più maiò perchè ella cresce da e traduzzioni di schedarii di tutti i furmati.
- Dunque _Poedit_ serà piuttostu impiegatu per cumpletà a traduzzione d’un schedariu `.po` dighjà principiata è _OmegaT_ serà ricumandatu per fà a traduzzione sana d’un schedariu `.po` o di qualchì altru furmatu.
- Per impiegà _OmegaT_, seguitate l’[istruzzioni per l’adopru di l’appiecazione _OmegaT_](OmegaT.md).
- Osinnò per cumpletà una traduzzione cù _Poedit_, ci vole à impiegà _Transifex_ per espurtà direttamente u schedariu di lingua corsa :
  - `Audacity master (development version, updated daily)` https://www.transifex.com/klyok/audacity/audacity-master-development/co/download/for_translation/
  - `Audacity master (string freeze version)` https://www.transifex.com/klyok/audacity/audacity-master/co/download/for_translation/
  - `Audacity release-3.0.3)` https://www.transifex.com/klyok/audacity/audacity-release-303/co/download/for_translation/
- Lancià _Poedit_ è apre u schedariu per traducelu eppò arregistrallu.
- Dopu a traduzzione, hè ricumandatu d’impiegà _Transifex_ cù l’ozzione `Téleverser un fichier` per rinfrescà u schedariu di traduzzione.

## Istruzzioni per piglià in contu u novu schedariu in lingua corsa

Quandu u vostru schedariu di lingua corsa hè prontu, ci vole à mandà u schedariu in furmatu `.po` in pezza aghjunta à a lista di distribuzione d’_Audacity_.  

Di regula, ghjè _James Crook_ chì hè incaricatu di piglià in contu tutti i schedarii di lingua è di mudificà a basa d’Audacity. Per tuttu ciò chì tocca à _Transifex_, ci vole à cuntattà _Thomas De Rocker_. Si pò truvà i so indirizzi à tremindui in l’[archivii di i messaghji di a lista di distribuzione d’_Audacity_](https://sourceforge.net/p/audacity/mailman/audacity-translation/).
