# A traduzzione in lingua corsa di _Notepad++_

## Distribuzione
- A prima traduzzione in corsu hè stata distribuita cù a version 6.9.2 di settembre di u 2016
- U stallatore NSIS hè statu distribuitu cù a versione 7.3.3 di maghju di u 2017
- Una [cronolugia di tutte e dumande di mudificazione](https://github.com/notepad-plus-plus/notepad-plus-plus/pulls?utf8=%E2%9C%93&q=is%3Apr+corsican) si trova nant’à GitHub
- Una [cronolugia di tutte e mudificazioni](https://github.com/notepad-plus-plus/notepad-plus-plus/commits/master/PowerEditor/installer/nativeLang/corsican.xml) si trova nant’à GitHub

## Traduttore
- Patriccollu di Santa Maria è Sichè

## Pagina di u situ Web ufficiale nant’à a traduzzione
- https://npp-user-manual.org/docs/binary-translation/

## Ciò ch’ella ci vole per traduce
- Richiestu
  - Un contu nant’à _GitHub_
- Ozzionale
  - _Notepad++_, prugramma per mudificà un testu, paragunà duie versioni di testu, o trasfurmà u cuntenutu cù una prucedura pre-arregistrata
  - _OmegaT_, prugramma per traduce i schedarii cù l’estensioni `.lng`
 
## I schedarii di lingua à traduce

U dipositu di tutta a fonte di Notepad++ si trova nant’à _GitHub_ :  
   https://github.com/notepad-plus-plus/notepad-plus-plus  
   https://github.com/notepad-plus-plus/wingup
   
### L’interfaccia di _Notepad++_

I schedarii di lingua si trovanu in u cartulare [/nativeLang/.](https://github.com/notepad-plus-plus/notepad-plus-plus/tree/master/PowerEditor/installer/nativeLang)
  
- U furmatu di i schedarii : `xml`
- A fonte d’origine : [english.xml](https://github.com/notepad-plus-plus/notepad-plus-plus/blob/master/PowerEditor/installer/nativeLang/english.xml)
- U schedariu di lingua corsa : [corsican.xml](https://github.com/notepad-plus-plus/notepad-plus-plus/blob/master/PowerEditor/installer/nativeLang/corsican.xml)

### U so cumpunente _wingup_

_wingup_ hè u cumpunentu di _Notepad++_ chì s’incaricheghja e messe à livellu di u prugramma.

I schedarii di lingua di _wingup_ si trovanu in un altru [cartulare specificu](https://github.com/notepad-plus-plus/wingup/tree/master/src/translations)

- A fonte d’origine : [english.xml](https://github.com/notepad-plus-plus/wingup/blob/master/src/translations/english.xml)
- U schedariu di lingua corsa : [corsican.xml](https://github.com/notepad-plus-plus/wingup/blob/master/src/translations/corsican.xml)

## Cumu sapè quandu ci hè qualcosa di novu à traduce ?

Trà duie versioni, a squadra di _Notepad++_ pò mudificà e catene di fonte nant’à _GitHub_ aghjunghjendu catene nove, mudifichendu o squassendu catene anziane. Quandu st’operazione si face, ùn hè micca pussibule di riceve autumaticamente un messaghju elettronicu, cum’è per indettu, via un’iscrizzione à una lista di distribuzione.  

Ci hè una funzione in GitHub per cunnosce tutte e mudificazioni fatte (commits) nant’à a fonte d’origine :  
https://github.com/notepad-plus-plus/notepad-plus-plus/commits/master/PowerEditor/installer/nativeLang/english.xml
  
Un cliccu nant’à ogni mudificazione vi permette di fighjà tutte e sfarenze trà duie versioni : e linee squassate, cambiate o aghjunte. Ma qu’ella operazione hè manuale.
  
Per furtuna, ci hè un’altra funzione in _GitHub_ chì permette d’ingenerà un flussu di nutizie `Atom` secondu l’attività di _GitHub_, per indettu quand’un schedariu hè mudificatu. È si pò riceve un avvertimentu in _Thunderbird_ quand’un tale flussu hè ingeneratu.  

Per sapene di più, fighjate l’istruzzioni per [impiegà un flussu di _GitHub_ è riceve l’infurmazione nant’à _Thunderbird_](../../Flussu%20di%20nutizie.md).

### I flussi _Atom_

Eccu i flussi à cuttighjà ch’ella ci vole à definisce in _Thunderbird_ grazia à un abbunamentu :  
- https://github.com/notepad-plus-plus/notepad-plus-plus/commits/master/PowerEditor/installer/nativeLang/english.xml.atom
- https://github.com/notepad-plus-plus/wingup/commits/master/src/translations/english.xml.atom
- https://github.com/notepad-plus-plus/notepad-plus-plus/tags.atom

U primu è u secondu liame permettenu di sapè quandu ci hè una mudificazione di u schedariu di e catene inglese à traduce. L’ultimu liame ghjove à esse infurmatu quandu ci hè una versione nova di _Notepad++_.  

## Cumu fà a traduzzione ?

- _Notepad++_ ùn prupone alcuna appiecazione - nè lucale, nè nant’à u Web - per fà a traduzzione

- Per fà què, hè ricummandatu d’impiegà __OmegaT__ perchè hè capace di mudificà u furmatu di schedariu `.lng`. Per sapene di più, seguitate l’[istruzzioni per l’adopru di l’appiecazione _OmegaT_](OmegaT.md)

## Istruzzioni per piglià in contu u novu schedariu di lingua corsa

Quandu u vostru schedariu di lingua corsa hè prontu nant’à u vostru urdinatore, ci vole à impiegà _GitHub_ per pigliallu in contu, vole si dì dumandà a mudificazione di a versione attuale di u schedariu di destinazione per ch’ella sia rimpiazzata da a vostra versione lucale.  

- Andà nant’à u [situ ufficiale di Notepad++](https://github.com/notepad-plus-plus/notepad-plus-plus) o quellu di [u so cumpunente _wingup_](https://github.com/notepad-plus-plus/wingup)

- Cliccà nant’à u buttone `Go to file` è scrive « _corsican.xml_ » per circà stu schedariu

- Cliccà nant’à a linea `PowerEditor/installer/nativeLang/corsican.xml` per fighjà a versione attuale

- Cliccà nant’à l’icona di a mina, quella chì si trova tuttu insù à dirittu, trà l’icona di u screnu è quella di l’empiilozzu. Si pò fighjà un cummentu chì dice « _Edit the file in your fork of this project_ ». Vole si dì chì a mudificazione si ferà in lucale, in una copia di u dipositu Notepad++ chì si chjamerà `u_mo_nome_github/notepad-plus-plus`

- D’altronde, ci hè u messaghju dicendu : _You’re making changes in a project you don’t have write access to. Submitting a change will write it to a new branch in your fork u_mo_nome_github/notepad-plus-plus, so you can send a pull request._

- In a sessione di mudificazione « _Edit file_ » chì s’apre, rimpiazzà a versione attuale da a vostra versione lucale di u schedariu di lingua corsa

- Verificà e mudificazioni grazia à l’unghjetta « _Preview changes_ ». S’ellu ci hè qualcosa à cambià, si pò sempre mudificalla via l’unghjetta « _Edit file_ »

- Quandu u schedariu hè prontu, ci vole à andà tuttu inghjò. Sottu u paragrafu _Propose changes_ scrivite un cummentu per spiegà perchè u schedariu hè mudificatu. Per indettu : `Update Corsican translation for Notepad++ 7.9.6`

- Cliccà nant’à u buttone « _Propose changes_ » per acccettà e mudificazioni direttamente ver di una nova ghjamba lucale. Da bona regula, a ghjamba principale (o maestra) si chjama _Master_ è l’altre, impiegate per i cambiamenti sò chjamate autumaticamente `patch-1, …, patch-n`

- Una funzione « _Comparing changes_ » vi prupone di paragunà a versione attuale :  
  `base repository: notepad-plus-plus/notepad-plus-plus/` `base: master`  
cù a vostra versione creata pocu fà :  
  `head repository: u_mo_nome_github/notepad-plus-plus/` `compare: patch-1`  
  _✔️ Able to merge. These branches can be automatically merged._  

  Ci hè un buttone verde `Create pull request` ma __ùn ci vole micca à fà què__ subitu !

- Avà, ci vole à rinuminà sta ghjamba creata pocu fà perchè Notepad++ richiede __una nova ghjamba per ogni mudificazione__. U nome ricumandatu hè `NPP_aaaammgg` induve _aaaa_=l’annu, _mm_=u mese è _gg_=u ghjornu), per indettu `NPP_20210328`

- Andà à u vostru dipositu lucale nant’à GitHub : `https://github.com/u_mo_nome_github/notepad-plus-plus`

- Cliccà nant’à u buttone cù u numeru di e ghjambe chì si trova trà u buttone `Master` è u numeru d’etichette (`tags`)

- Cliccà nant’à l’icona di a mina, in pettu à u nome di a nova ghjamba, per indettu `patch-1`, per cambiallu

- Rimpiazzà u nome attuale da `NPP_aaaammgg` è cliccà nant’à u buttone `Rename branch`

- Andà à l’unghjetta « _Code_ » per vede l’ultimu cambiamentu. Ci hè un messaghju dicendu :  
  `NPP_aaaammgg had recent pushes less than a minute ago`

- Appughjà nant’à u buttone verde `Compare & pull request`

- Avà, ghjè a funzione « _Open a pull request_ » chì torna vi prupone di paragunà a versione attuale :  
  `base repository: notepad-plus-plus/notepad-plus-plus/` `base: master`  
  cù a vostra versione creata pocu fà :  
  `head repository: u_mo_nome_github/notepad-plus-plus/` `compare: NPP_aaaammgg`  
  _✔️ Able to merge. These branches can be automatically merged._  

- L’azzione _Pull Request_ hè una dumanda à a squadra Notepad++ per accettà a nova versione cù e vostre mudificazioni. Un titulu per sta dumanda hè prupostu ; ghjè quellu dighjà scrittu per spiegà i cambiamenti : `Update Corsican translation for Notepad++ 7.9.6`  
  Si pò cambià u titulu.

- Ci vole à aghjunghje un cummentu. Fighjate a [cronolugia di e dumande scorse](https://github.com/notepad-plus-plus/notepad-plus-plus/pulls?utf8=%E2%9C%93&q=is%3Apr+corsican) per sapene di più

- Quandu a vostra dumanda - titulu è cummentu - hè pronta, cliccà nant’à u buttone `Create pull request`

- Una nova dumanda hè stata creata per appruntà una fusione :  
  `1 commit into notepad-plus-plus:master from u_mo_nome_github:NPP_aaaammgg`

- Ci vole à aspettà chì sta dumanda sia trattata da a squadra Notepad++. Si pò [seguitalla in a lista di tutte e dumande aperte.](https://github.com/notepad-plus-plus/notepad-plus-plus/pulls) Què pò piglià parechji ghjorni, o ancu settimane

- Fin’tantu chì a vostra dumanda ùn hè stata ancu trattata, s’ella hè bisognu, ci hè pussibule di fà d’altre mudificazioni :
  - Andà nant’à a vostra dumanda cù `https://github.com/notepad-plus-plus/notepad-plus-plus/pull/nnnn/commits`  
  _induve_ nnnn _hè u numeru di a vostra dumanda_
  - Cliccà nant’à a mudificazione a più recente (s’ella ci n’hè più d’una) per fighjà e vostre mudificazioni fatte pocu fà
  - Cliccà nant’à u segnu `...` tuttu à dirittu nant’à a linea `PowerEditor/installer/nativeLang/corsican.xml`
  - Sceglie l’ozzione `Edit file`
  - Mudificà u schedariu di lingua corsa
  - Quandu u schedariu hè prontu, ci vole à andà tuttu inghjò. Sottu à u paragrafu _Commit changes_ scrivite un cummentu per spiegà perchè u schedariu hè statu mudificatu. Per indettu : `Update Corsican translation for Notepad++ 7.9.6`
  - Cliccà nant’à u buttone « _Commit changes_ » per acccettà e mudificazioni direttamente ver di a vostra ghjamba lucale `NPP_aaaammgg`
  - Si pò vede un paragone di e sfarenze trà a versione attuale è a vostra ultima versione :  
  `u_mo_nome_github wants to merge 2 commits into notepad-plus-plus:master from u_mo_nome_github:NPP_aaaammgg`
  - Cliccà nant’à `Conversation` per fighjà a cronolugia di a vostra dumanda
  - Si pò aghjunghje un cummentu, per indettu per spiegà chì st'ultima mudificazione era per traduce una mudificazione recente di u schedariu di fonte in inglese
  - Tandu si facenu parechji cuntrolli in _GitHub_ grazia à a funzione _appveyor_ è si pò vede cù un circulu ghjallu chì serà rimpiazzatu cù u segnu ✔️ quandu i cuntrolli seranu compii
- Quandu sta dumanda hè stata pigliata in contu da Don, u sviluppatore di Notepad++, si pò squassà a vostra ghjamba lucale `NPP_aaaammgg`

#### Liami di navigazione nant’à stu situ
- [Rivene à a lista di i membri di stu prughjettu](./)
- [Rivene à a lista di tutti i prughjetti](../)
- [Rivene à a lista di tutti i prugrammi](../../../../#readme)
