# A traduzzione in lingua corsa di Notepad++

## Distribuzione
 - A prima traduzzione in corsu hè stata distribuita cù a version 6.9.2 di settembre di u 2016
 - U stallatore NSIS hè statu distribuitu cù a versione 7.3.3 di maghju di u 2017
 - Una [cronolugia di tutte e dumande di mudificazione](https://github.com/notepad-plus-plus/notepad-plus-plus/pulls?utf8=%E2%9C%93&q=is%3Apr+corsican) si trova nant’à GitHub
## Traduttore
 - Patriccollu di Santa Maria è Sichè

## Pagina di u situ Web ufficiale nant’à a traduzzione
 - https://npp-user-manual.org/docs/binary-translation/

## I schedarii di lingua à traduce

U dipositu di tutta a fonte di Notepad++ si trova nant’à GitHub :  
   https://github.com/notepad-plus-plus/notepad-plus-plus

I schedarii di lingua si trovanu in u cartulare [/nativeLang/.](https://github.com/notepad-plus-plus/notepad-plus-plus/tree/master/PowerEditor/installer/nativeLang)

- A fonte d’origine : [english.xml](https://github.com/notepad-plus-plus/notepad-plus-plus/blob/master/PowerEditor/installer/nativeLang/english.xml)
- U schedariu di destinazione : [corsican.xml](https://github.com/notepad-plus-plus/notepad-plus-plus/blob/master/PowerEditor/installer/nativeLang/corsican.xml)
- U furmatu di i schedarii : `xml`

## Cumu sapè quandu ci hè qualcosa di novu à traduce ?
Per disgrazia, ùn hè micca pussibule di riceve un messaghju quandu ci hè qualcosa di novu à traduce, per indettu cù un’iscrizzione à una lista di distribuzione.  

Ma ci hè una funzione in GitHub per cunnosce tutte e mudificazioni (commits) fatte nant’à a fonte d’origine :  
https://github.com/notepad-plus-plus/notepad-plus-plus/commits/master/PowerEditor/installer/nativeLang/english.xml
  
Un cliccu nant’à ogni mudificazione vi permette di fighjà tutte e sfarenze trà duie versioni : e linee squassate, cambiate o aghjunte.

## Cumu fà a traduzzione ?
- Notepad++ ùn prupone alcuna appiecazione - lucale o nant’à u Web - per fà a traduzzione.
- Pudete impiegà __OmegaT__ per fà què. Per sapene di più, seguitate l’[istruzzioni per cunvertisce un schedariu di lingua](https://github.com/Patriccollu/Lingua_Corsa-Infurmatica/blob/master/Prughjetti/Notepad%2B%2B/Cunversione.md) per ch’ellu sia accettatu da  __OmegaT__.  

Quandu u vostru schedariu di lingua corsa hè prontu nant’à u vostru urdinatore, ci vole à impiegà GitHub per pigliallu in contu, vole si dì dumandà a mudificazione di a versione attuale di u schedariu di destinazione per ch’ella sia rimpiazzata da a vostra versione lucale.

## Istruzzioni per piglià in contu u novu schedariu di lingua corsa

- Andà nant’à u [situ ufficiale di Notepad++](https://github.com/notepad-plus-plus/notepad-plus-plus)

- Cliccà nant’à u buttone « _Go to file_ » è scrive `corsican.xml` per circà stu schedariu.

- Cliccà nant’à a linea `PowerEditor/installer/nativeLang/corsican.xml` per fighjà a versione attuale.

- Cliccà nant’à l’icona di a mina, quella chì si trova tuttu insù à dirittu, trà l’icona di u screnu è quella di l’empiilozzu. Si pò fighjà un cummentu chì dice « _Edit the file in your fork of this project_ ». Vole si dì chì a mudificazione si ferà in lucale, in una copia di u dipositu Notepad++ chì si chjamerà `u_mo_nome_github/notepad-plus-plus`

- In a sessione di mudificazione « _Edit file_ » chì s’apre, rimpiazzà a versione attuale da a vostra versione lucale di u schedariu di lingua corsa.

- Verificà e mudificazioni grazia à l’unghjetta « _Preview changes_ ». S’ellu ci hè qualcosa à cambià, si pò sempre mudificalla via l’unghjetta « _Edit file_ ».

- Quandu u schedariu hè prontu, scrive un cummentu cum’è, per indettu : `Update Corsican translation for Notepad++ 7.9.3`

- Cliccà nant’à u buttone « _Commit changes_ » per acccettà e mudificazioni direttamente ver di una nova ghjamba lucale. Da bona regula, a ghjamba principale (o maestra) si chjama _Master_ è l’altre, impiegate per i cambiamenti sò chjamate autumaticamente `patch_1, …, patch_n`

- Avà, ci vole à rinuminà sta ghjamba creata pocu fà perchè Notepadd++ richiede __una nova ghjamba per ogni mudificazione__. U nome ricumandatu hè `NPP_aaaammgg` induve _aaaa_=l’annu, _mm_=u mese è _gg_=u ghjornu), per indettu `NPP_20210327`

- Andà à l’unghjetta « _Code_ » di u vostru dipositu lucale. Da bona regula, u nome di a nova ghjamba hè affissatu. Cliccà nant’à u buttone cù u numeru di e ghjambe chì si trova trà u nome di a nova ghjamba è u numeru d’etichette (_tags_).

- Cliccà nant’à l’icona di a mina, in pettu à u nome di a nova ghjamba per cambiallu.

- Rimpiazzà u nome attuale da `NPP_aaaammgg`

- Andà à l’unghjetta « _Code_ » per vede l’ultimu cambiamentu. Appughjà nant’à u buttone verde « _Compare & pull request_ »

- St’azzione - __Pull Request__ - hà da appruntà una fusione : `1 commit into notepad-plus-plus:master from u_mo_nome_github:NPP_aaaammgg`

- Ci vole à aspettà chì sta dumanda sia trattata da Don, u sviluppatore di Notepadd++. Què pò piglià un parechji ghjorni.

- Quandu sta dumanda hè stata pigliata in contu, si pò squassà a ghjamba lucale `NPP_aaaammgg`
