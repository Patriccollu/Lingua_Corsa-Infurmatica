# Prucedura di cunversione di i schedarii di traduzzione _Mp3tag_

Eccu duie prucedure di cunversione di i schedarii di traduzzione _Mp3tag_ per ch’elli sianu accettati da  __OmegaT__, attrezzu di traduzzione assistita da l’urdinatore.

## Scopu di e prucedure

- Per disgrazia, i schedarii di traduzzione `.lng` di _Mp3tag_ ùn ponu micca esse tradutti direttamente da _OmegaT_, bench’ellu cunnosci st’estensione è ci vole à trasfurmà un pocu u furmatu di u so cuntenutu.
- Eccu duie prucedure macro chì si pò caricà è impiegà in _Notepad++_ per fà ste trasfurmazioni :
1. `Cunversione Mp3tag(.lng)-OmegaT(.lng)`  
   Per trasfurmà u cuntenutu di u schedariu `English.lng` da u so furmatu d’origine ver di u furmatu `.lng` accettatu da  _OmegaT_
2. `Cunversione OmegaT(.lng)-Mp3tag(.lng)`  
   Per trasfurmà u cuntenutu di u schedariu `English.lng` da u furmatu cunnisciutu da _OmegaT_, ver di u so furmatu d’origine

#### Esempiu di linee in u schedariu d’origine :

```
_M_STR_PRESETS &Presets
_M_STR_PREVIEW Preview
_M_STR_PROPERTIES {1} Properties
_M_STR_QUICK &Quick
_M_STR_RECURSE Subdirectories
_M_STR_REST Rest
_M_STR_SAVE_NOT < no association >
```

#### Eccu e listesse linee dopu à a trasfurmazione cù a prima prucedura` :

```
_M_STR_PRESETS=&Presets
_M_STR_PREVIEW=Preview
_M_STR_PROPERTIES={1} Properties
_M_STR_QUICK=&Quick
_M_STR_RECURSE=Subdirectories
_M_STR_REST=Rest
_M_STR_SAVE_NOT=< no association >
```

- Ghjè a seconda prucedura chì face a trasfurmazione à l’arritrosa : `Cunversione OmegaT(.lng)-Mp3tag(.lng)`
- U schedariu trasfurmatu pò esse arregistratu cù a listessa estensione `.lng`

## Installazione di e prucedure

- Apre u cartulare di _Notepad++_ induve si trova u schedariu `shortcuts.xml` perchè ghjè quellu chì cuntene tutte e vostre prucedure persunalizate. Da bona regula, stu cartulare si trova in `C:\Users\xxxxxxxx\AppData\Roaming\Notepad++` (induve _xxxxxxxx_ hè u vostru nome d’utilizatore).  

    Per apre stu cartulare d’una manera più faciule, ci vole à fà una ricerca Windows cù sta catena : `%APPDATA%\Notepad++`

- In u cartulare chì s’apre, sciglite u schedariu `shortcuts.xml` è apritelu cù _Notepad++_.

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
        <Macro name="Cunversione Mp3tag(.lng)-OmegaT(.lng)" Ctrl="no" Alt="no" Shift="no" Key="0" FolderName="Cunversioni Mp3tag">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per rimpiazzà solu a prima occurenza d'un spaziu da un segnu uguale nant'à ogni linea" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam=" (.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="=$1" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
        <Macro name="Cunversione OmegaT(.lng)-Mp3tag(.lng)" Ctrl="no" Alt="no" Shift="no" Key="0" FolderName="Cunversioni Mp3tag">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per rimpiazzà solu a prima occurenza d'un segnu uguale da un spaziu nant'à ogni linea" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="=(.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam=" $1" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
```
- Tandu e nove prucedure sò dispunibule in _Notepad++_.
- Di sicuru, si pò sceglie __d’altri nomi__ di prucedura.  

Per a vostra infurmazione, ci hè parechje istruzzioni `message="2172"` in ste prucedure chì cuntenenu un cummentu per spiegà ciò chì si face dentru. Ùn si pò micca impiegà i cummenti classichi di u XML perchè quelli cummenti sò autumaticamente squassati quandu ci hè una mudificazione di u schedariu `shortcuts.xml` da _Notepad++_, per indettu per arregistrà una nova prucedura macro arricurdata.

## Impiegu di e prucedure

- Lancià _Notepad++_
- Apre u schedariu di traduzzione ch’ellu ci vole à cunvertisce
- Sceglie `Macro`, eppò `Eseguisce una macro parechje volte…`
- Selezziunà u nome di a prucedura à impiegà
- Cliccu nant’à `Eseguisce 1 volta`
- Appughjà nant’à u buttone `Eseguisce`
- Arregistrà u schedariu trasfurmatu cù l’estensione `.lng`

#### Liami di navigazione nant’à stu situ
- [Rivene à a lista di i membri di stu prughjettu](./)
- [Rivene à a lista di tutti i prughjetti](../)
- [Rivene à a lista di tutti i prugrammi](../../../../#readme)
