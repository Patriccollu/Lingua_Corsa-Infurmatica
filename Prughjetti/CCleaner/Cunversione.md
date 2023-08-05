# Prucedura di cunversione di i schedarii di traduzzione _CCleaner_

Eccu parechje prucedure di cunversione di i schedarii di traduzzione _CCleaner_ per ch’elli sianu accettati da  __OmegaT__, attrezzu di traduzzione assistita da l’urdinatore.

## Scopu di e prucedure

Per disgrazia, i schedarii di traduzzione `.nsh` è `.rc` di _CCleaner_ ùn ponu micca esse tradutti direttamente da _OmegaT_ è ci vole à trasfurmà u furmatu di u so cuntenutu. Eccu quattru prucedure macro chì si pò caricà è impiegà in _Notepad++_ per fà ste trasfurmazioni :
1. `Cunversione CCleaner(.nsh)-OmegaT(.lng)` per trasfurmà u cuntenutu di u schedariu `lang_en.nsh` da u so furmatu d’origine à u furmatu `.lng`
2. `Cunversione CCleaner(.rc)-OmegaT(.isl)` per trasfurmà u cuntenutu di u schedariu `res_en.rc` o `res_uk_recuva.rc` da u so furmatu d’origine à u furmatu `.isl`
3. `Cunversione OmegaT(.lng)-CCleaner(.nsh)` per trasfurmà u cuntenutu di u schedariu `lang_en.nsh.lng` da u furmatu cunnisciutu da _OmegaT_, à u so furmatu `.nsh` d’origine
4. `Cunversione OmegaT(.isl)-CCleaner(.rc)` per trasfurmà u cuntenutu di u schedariu `res_en.rc.isl` o `res_uk_recuva.rc.isl` da u furmatu cunnisciutu da _OmegaT_, à u so furmatu `.rc` d’origine

A) Esempiu di linee in u schedariu d’origine `lang_en.nsh` :
```
LangString ADVANCED_OPTIONS_SUBTITLE ${LANG_ENGLISH} "Select any advanced options"
LangString ADVANCED_OPTIONS_TITLE ${LANG_ENGLISH} "Advanced Options"
```
Eccu e listesse linee dopu à trasfurmazione cù a prucedura `Cunversione CCleaner(.nsh)-OmegaT(.lng)` :
```
LangString_ADVANCED_OPTIONS_SUBTITLE_${LANG_ENGLISH}=Select any advanced options
LangString_ADVANCED_OPTIONS_TITLE_${LANG_ENGLISH}=Advanced Options
```
In più di què, ci hè una prucedura chì face a trasfurmazione à l’arritrosa : `Cunversione OmegaT(.lng)-CCleaner(.nsh)`.  

B) Esempiu di linee in u schedariu d’origine `res_en.rc` o `res_uk_recuva.rc`  :
```
STRINGTABLE
BEGIN
100,	"1033"	/* Automated Language ID */
8,	"CCleaner Homepage"
9,	"Uninstall CCleaner"
102,	"Click here to visit the CCleaner website at www.ccleaner.com/ccleaner"
```
Eccu e listesse linee dopu à trasfurmazione cù a prucedura `Cunversione CCleaner(.rc)-OmegaT(.isl)` :
```
;STRINGTABLE
;BEGIN
100=1033
8=CCleaner Homepage
9=Uninstall CCleaner
102=Click here to visit the CCleaner website at www.ccleaner.com/ccleaner
```
In più di què, ci hè una prucedura chì face a trasfurmazione à l’arritrosa : `Cunversione OmegaT(.isl)-CCleaner(.rc)`.  

Per i dui furmati `.nsh` è `.rc`, ste linee ponu esse arregistrate in un schedariu cù l’estensioni `.lng` o `.isl` chì sò dui furmati cunnisciuti da OmegaT.

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
        <Macro name="Cunversione CCleaner(.nsh)-OmegaT(.lng)" Ctrl="no" Alt="no" Shift="no" Key="0" FolderName="Cunversioni CCleaner">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per trasfurmà tutte e line da u furmatu NSH à u furmatu LNG" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='LangString (.*) \${LANG_ENGLISH} &quot;(.*)&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="LangString_\1_\${LANG_ENGLISH}=\2" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
        <Macro name="Cunversione OmegaT(.lng)-CCleaner(.nsh)" Ctrl="no" Alt="no" Shift="no" Key="0" FolderName="Cunversioni CCleaner">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per trasfurmà tutte e line da u furmatu LNG à u furmatu NSH" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="LangString_(.*)_\${LANG_ENGLISH}=(.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam='LangString \1 \${LANG_ENGLISH} &quot;\2&quot;' />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
        <Macro name="Cunversione CCleaner(.rc)-OmegaT(.isl)" Ctrl="no" Alt="no" Shift="no" Key="0" FolderName="Cunversioni CCleaner">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per caccià i cummenti chì seguiteghjanu i caratteri // piazzati dopu à un spaziu o una tabulazione" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="(.*)[ |\t]//(.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\1" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per caccià i cummenti chì si trovanu trà i caratteri /* è */" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="/\*([^*]|[\r\n]|(\*+([^*/]|[\r\n])))*\*+/" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Cumanda nurmale per ammuzzà tutti i spazii di fine di linea" />
            <Action type="2" message="0" wParam="42024" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam='Rimpiazzamentu nurmale di |""| da |&#x00C2;&#x00A7;&#x00C2;&#x00A7;|' />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='&quot;&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="&#x00C2;&#x00A7;&#x00C2;&#x00A7;" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per trasfurmà e linee in u furmatu variabile=catena" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='(\d{6}|\d{5}|\d{4}|\d{3}|\d{2}|\d{1})(.*)&quot;(.*)&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\1=\3" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam='Rimpiazzamentu nurmale di |&#x00C2;&#x00A7;&#x00C2;&#x00A7;| da |"|' />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="&#x00C2;&#x00A7;&#x00C2;&#x00A7;" />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam='&quot;' />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per aghjunghje u segnu ; à tutte e linee" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="(.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam=";\1" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per caccià u segnu ; nant'à e linee chì cuntenenu u segnu uguale" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam=";(.*)=(.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\1=\2" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
        <Macro name="Cunversione OmegaT(.isl)-CCleaner(.rc)" Ctrl="no" Alt="no" Shift="no" Key="0" FolderName="Cunversioni CCleaner">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per trasfurmà tutte e line da u furmatu LNG à u furmatu RC" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="(.*)=(.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam='\1,\t&quot;\2&quot;' />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per caccià u segnu ; nant'à e linee chì principanu da stu segnu" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="^;(.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\1" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
```
- Tandu e prucedure nove sò dispunibule in _Notepad++_.
- Di sicuru, si pò sceglie __d’altri nomi__ di prucedura.  

Per a vostra infurmazione, ci hè parechje istruzzioni `message="2172"` in ste prucedure chì cuntenenu un cummentu per spiegà ciò chì si face dentru. Ùn si pò micca impiegà i cummenti classichi di u XML perchè quelli cummenti sò autumaticamente squassati quandu ci hè una mudificazione di u schedariu `shortcuts.xml` da _Notepad++_, per indettu per arregistrà una nova prucedura macro arricurdata.

## Impiegu di e prucedure

- Per fà a cunversione d’un schedariu da u so furmatu d’origine versu u furmatu `.lng` cunnisciutu da OmegaT, [seguitate st’istruzzioni](./OmegaT.md#preparazione-di-i-schedarii-nanzu-a-traduzzione).
- Per fà a cunversione d’un schedariu da u furmatu `.lng` cunnisciutu da OmegaT versu u so furmatu d’origine, [seguitate st’istruzzioni](./OmegaT.md#preparazione-di-i-schedarii-dopu-a-traduzzione).

#### Liami di navigazione nant’à stu situ
- [Rivene à a lista di i membri di stu prughjettu](./)
- [Rivene à a lista di tutti i prughjetti](../)
- [Rivene à a lista di tutti i prugrammi](../../../../#readme)
