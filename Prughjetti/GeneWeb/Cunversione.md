# Prucedura di cunversione di schedariu di traduzzione GeneWeb

Eccu una prucedura di cunversione di u schedariu di traduzzione GeneWeb per ch’ellu sia accettatu da  __OmegaT__, attrezzu di traduzzione assistita da l’urdinatore.

## Scopu di a prucedura

- Per disgrazia, u schedariu di traduzzione di GeneWeb hè unicu è cuntene tutte e lingue !
  
Esempiu di linee di u schedariu `lexicon.txt` :
```
    a nephew/a niece
af: 'n broerskind/'n susterskind///broers- en susterskinders
bg: племенник/племенница/племенници/племеннички/племенници и племеннички
br: un niz/un nizez/nized/nizezed/nized ha nizezed
ca: un nebot/una neboda/nebots/nebodes/nebots i nebodes
co: un nipote/una nipote/nipoti/nipoti/nipoti
de: ein:d:+em Neffe:d:+n/eine:d:+r Nichte/Neffen/Nichten/Neffen und Nichten
en: a nephew/a niece/nephews/nieces/nephews and nieces
es: un sobrino/a sobrina/sobrinos/sobrinas/sobrinos y sobrinas
et: venna- või õepoeg:g:--ja/venna- või õetütar:g:--re///venna- ja õelapsed
fi: veljen- tai sisarenpoika:g:---jan/veljen- tai sisarentytär:g:---tären///sisarusten lapset
fr: un neveu/une nièce/neveux/nièces/neveux et nièces
```
- Dunque ùn pò micca esse traduttu direttamente da OmegaT è ci vole à trasfurmà u furmatu di u so cuntenutu.

- Eccu una prucedura macro - `Cunversione GeneWeb(.txt)-OmegaT(.txt)` - chì si pò caricà è impiegà in _Notepad++_ per fà quella trasfurmazione :
  - squassà tutti i tituli
  - cunservà e linee cù e catene in inglese, quelle chì principianu cù `en: ` 
  - squassà e traduzzioni di tutte l’altre linee 
  - squassà u prefissu `en: `
  
Eccu e listesse linee dopu à trasfurmazione :
```
a nephew/a niece/nephews/nieces/nephews and nieces
```
- Ste linee devenu esse arregistrate in un schedariu cù l’estensione `.txt` chì hè un furmatu cunnisciutu da OmegaT.

## Installazione di a prucedura

- Apre u cartulare di Notepad++ induve si trova u schedariu `shortcuts.xml` perchè ghjè quellu chì cuntene tutte e vostre prucedure persunalizate. Da bona regula, stu cartulare si trova in `C:\Users\xxxxxxxx\AppData\Roaming\Notepad++` (induve _xxxxxxxx_ hè u vostru nome d’utilizatore).  

    Per apre stu cartulare d’una manera più faciule, ci vole à fà una ricerca Windows cù sta catena : `%APPDATA%\Notepad++`

- In u cartulare chì s’apre, sciglite u schedariu `shortcuts.xml` è apritelu cù Notepad++.

- Dentru u schedariu, dopu l’istruzzione `<Macros>`, ci hè unu o parechji gruppi d’istruzzioni chì s’assumiglianu à què :
```
	<Macro name=".......">
	   ...
	   ...
	   ...
	</Macro>
```
- Basta à aghjunghje tutte st’istruzzioni __nanzu__ a linea `</Macros>` chì indicheghja a fine di tutte e prucedure macro.
```
        <Macro name="Cunversione GeneWeb(.txt)-OmegaT(.txt)" Ctrl="no" Alt="no" Shift="no" Key="0">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Marcà tutte e linee chì principianu cù |^en: |" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="^en: " />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="784" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1615" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Cumanda nurmale per caccià tutte e linee senza marca" />
            <Action type="2" message="0" wParam="43051" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Rimpiazzamentu allungatu di |^en: | da nunda" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="^en: " />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Cumanda nurmale per viutà e marche di tutte e linee indettate" />
            <Action type="2" message="0" wParam="43008" lParam="0" sParam="" />
        </Macro>
```
- Tandu a nova prucedura - `Cunversione GeneWeb(.txt)-OmegaT(.txt)` - hè dispunibule in Notepad++.
- Di sicuru, si pò sceglie __un altru nome di prucedura__.  

Per a vostra infurmazione, ci hè parechje istruzzioni `message="2172"` in ste prucedure chì cuntenenu un cummentu per spiegà ciò chì si face dentru. Ùn si pò micca impiegà i cummenti classichi di u XML perchè quelli cummenti sò autumaticamente squassati quandu ci hè una mudificazione di u schedariu `shortcuts.xml` da _Notepad++_, per indettu per arregistrà una nova prucedura macro arricurdata.

## Impiegu di a prucedura

- Scaricà l’ultima mudificazione di u schedariu `lexicon.txt` chì si trova nant’à u [dipositu _GitHub_](https://github.com/geneweb/geneweb/blob/master/hd/lang/lexicon.txt)
    - Fà un cliccu dirittu nant’à u buttone « _Raw_ » chì si trova à diritta, accant’à l’icone di u screnu, di a mina è di a curbella
    - Sceglie l’ozzione « _Arregistrà a sibula di a leia sottu…_ »
    - Arregistrà u schedariu cù u listessu nome
	
- Lancià Notepad++
- Apre u schedariu `lexicon.txt` scaricatu pocu fà
- Sceglie `Macro`, eppò `Eseguisce una macro parechje volte…`
- Selezziunà `Cunversione GeneWeb(.txt)-OmegaT(.txt)`
- Cliccu nant’à `Eseguisce 1 volta`
- Appughjà nant’à u buttone `Eseguisce`
- Arregistrà u schedariu cù u nome `omegat_lexicon.txt`
 - Cupià stu schedariu in u cartulare `/source/` di u prughjettu __GeneWeb__ in _OmegaT_.

#### Liami di navigazione nant’à stu situ
- [Rivene à a lista di i membri di stu prughjettu](./)
- [Rivene à a lista di tutti i prughjetti](../)
- [Rivene à a lista di tutti i prugrammi](../../../../#readme)
