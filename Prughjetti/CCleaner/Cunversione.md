# Prucedura di cunversione di i schedarii di traduzzione _CCleaner_

Eccu parechje prucedure di cunversione di i schedarii di traduzzione _CCleaner_ per ch’elli sianu accettati da  __OmegaT__, attrezzu di traduzzione assistita da l’urdinatore.

## Scopu di e prucedure

Per disgrazia, i schedarii di traduzzione `.nsh` è `.rc` di _CCleaner_ ùn ponu micca esse tradutti direttamente da _OmegaT_ è ci vole à trasfurmà u furmatu di u so cuntenutu. Eccu parechje prucedure macro chì si pò caricà è impiegà in _Notepad++_ per fà ste trasfurmazioni.  

A) Esempiu di linee in u schedariu d’origine `lang_en.nsh` :
```
LangString ADVANCED_OPTIONS_SUBTITLE ${LANG_ENGLISH} "Select any advanced options"
LangString ADVANCED_OPTIONS_TITLE ${LANG_ENGLISH} "Advanced Options"
```
Eccu e listesse linee dopu à trasfurmazione cù a prucedura `Cunversione_CCleaner_NSH-OmegaT` :
```
LangString_ADVANCED_OPTIONS_SUBTITLE_${LANG_ENGLISH}=Select any advanced options
LangString_ADVANCED_OPTIONS_TITLE_${LANG_ENGLISH}=Advanced Options
```
In più di què, ci hè una prucedura chì face a trasfurmazione à l’arritrosa : `Cunversione_OmegaT-CCleaner_NSH`.  

B) Esempiu di linee in u schedariu d’origine `res_en.rc` :
```
100,	"1033"	/* Automated Language ID */
8,	"CCleaner Homepage"
9,	"Uninstall CCleaner"
102,	"Click here to visit the CCleaner website at www.ccleaner.com/ccleaner"
```
Eccu e listesse linee dopu à trasfurmazione cù a prucedura `Cunversione_CCleaner_RC-OmegaT` :
```
100=1033
8=CCleaner Homepage
9=Uninstall CCleaner
102=Click here to visit the CCleaner website at www.ccleaner.com/ccleaner
```
Per i dui schedarii, ste linee ponu esse arregistrate in un schedariu cù l’estensione `.lng` chì hè un furmatu cunnisciutu da OmegaT.

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
        <Macro name="Cunversione_CCleaner_NSH-OmegaT" Ctrl="no" Alt="no" Shift="no" Key="0">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Mudificazione > Operazioni nant’à u spaziu > Ammuzzà i spazii di fine di linea" />
            <Action type="2" message="0" wParam="42024" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Rimpiazzamentu nurmale di {LangString } da {LangString_}" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="LangString " />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="LangString_" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Rimpiazzamentu nurmale di { ${LANG_ENGLISH} "} da {_${LANG_ENGLISH}=}" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam=' ${LANG_ENGLISH} &quot;' />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="_${LANG_ENGLISH}=" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Rimpiazzamentu allungatu di {"\n} da {\n}" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='&quot;&#x000D;&#x000A;' />
            <Action type="3" message="1625" wParam="0" lParam="1" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\n" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
        <Macro name="Cunversione_CCleaner_RC-OmegaT" Ctrl="no" Alt="no" Shift="no" Key="0">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per squassà tuttu ciò chì si trova trà { /*} è {*/}" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam=" /\*([^*]|[\r\n]|(\*+([^*/]|[\r\n])))*\*+/" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per squassà tuttu ciò chì si trova trà {\t/*} è {*/}" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="&#x0009;/\*([^*]|[\r\n]|(\*+([^*/]|[\r\n])))*\*+/" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Mudificazione > Operazioni nant’à u spaziu > Ammuzzà i spazii di fine di linea" />
            <Action type="2" message="0" wParam="42024" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Rimpiazzamentu allungatu di {"\n} da {\n}" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='&quot;&#x000D;&#x000A;' />
            <Action type="3" message="1625" wParam="0" lParam="1" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\n" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Rimpiazzamentu nurmale di {, 	"} da {=}" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam=', &#x0009;&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="=" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Rimpiazzamentu nurmale di {,	"} da {=}" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam=',&#x0009;&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="=" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Rimpiazzamentu nurmale di {,    "} da {=}" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam=',    &quot;' />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="=" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Rimpiazzamentu nurmale di {,   "} da {=}" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam=',   &quot;' />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="=" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Rimpiazzamentu nurmale di {,  "} da {=}" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam=',  &quot;' />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="=" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Rimpiazzamentu nurmale di {	"} da {=}" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='&#x0009;&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="=" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Marcà è indettà tutte e linee chì cuntenenu u segnu uguale (=)" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="=" />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="784" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1615" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Ricerca > Indetta > Arritrusà l’indette" />
            <Action type="2" message="0" wParam="43050" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Squassà tutte e marche" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1633" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Ricerca > Indetta > Caccià e linee indettate" />
            <Action type="2" message="0" wParam="43021" lParam="0" sParam="" />
        </Macro>
        <Macro name="Cunversione_OmegaT-CCleaner_NSH" Ctrl="no" Alt="no" Shift="no" Key="0">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Rimpiazzamentu nurmale di {LangString } da {LangString_}" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="LangString_" />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="LangString " />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Rimpiazzamentu nurmale di { ${LANG_ENGLISH} "} da {_${LANG_ENGLISH}=}" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="_${LANG_ENGLISH}=" />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam=' ${LANG_ENGLISH} &quot;' />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per aghjunghje un segnu {"} à a fine di tutte e line chì principianu da {LangString }" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="^(LangString .*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam='\1&quot;' />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
```
- Tandu e nove prucedure sò dispunibule in _Notepad++_.  
 
    Di sicuru, si pò sceglie __un altru nome di prucedura__.

## Impiegu di e prucedure

- Lancià _Notepad++_

- Apre u schedariu di traduzzione ch’ellu ci vole à cunvertisce

- Sceglie `Macro`, eppò `Eseguisce una macro parechje volte…`

- Selezziunà u nome di a prucedura à impiegà

- Cliccu nant’à `Eseguisce 1 volta`

- Appughjà nant’à u buttone `Eseguisce`

- Arregistrà u schedariu trasfurmatu cù l’estensione `.lng`
 
- Cupià stu schedariu in u cartulare `/source/` di u prughjettu __CCleaner__ in _OmegaT_.

#### Liami di navigazione nant’à stu situ
- [Rivene à a lista di i membri di stu prughjettu](./)
- [Rivene à a lista di tutti i prughjetti](../)
- [Rivene à a lista di tutti i prugrammi](../../../../#readme)
