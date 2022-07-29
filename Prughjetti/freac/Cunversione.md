# Prucedura di cunversione di i schedarii di traduzzione _fre:ac_

Eccu una prucedura di cunversione di u schedariu di traduzzione _fre:ac_ per ch’ellu sia accettatu da  __OmegaT__, attrezzu di traduzzione assistita da l’urdinatore.

## Scopu di a prucedura

Per disgrazia, certi schedarii di traduzzione `.xml` di _fre:ac_ ùn ponu micca esse tradutti direttamente da _OmegaT_ è ci vole à trasfurmà u furmatu di u so cuntenutu. Eccu una prucedura macro chì si pò caricà è impiegà in _Notepad++_ per fà sta trasfurmazione.  

Secondu à u cartulare induve si trovanu sti schedarii, a prucedura di cunversione hè richiesta o nò.  

- I schedarii chì si trovanu in quelli sottucartulari anu bisognu di trasfurmazione, vole si dì chì a prucedura di cunversione hè richiesta nanzu di traduceli cù _OmegaT_ :
  - https://github.com/enzo1982/freac/tree/master/i18n/freac/
  - https://github.com/enzo1982/freac/tree/master/i18n/setup/
  - https://github.com/enzo1982/freac/tree/master/i18n/tips
  - https://github.com/enzo1982/freac/tree/master/i18n/updater
  - Esempiu di linee in un schedariu chì hà bisognu di trasfurmazione :
```
    <entry id="100" string="OK"/>
    <entry id="101" string="Cancel"/>
    <entry id="102" string="Close"/>
```
- I schedarii chì si trovanu in sti sottucartulari `crowdin` ùn anu bisognu di trasfurmazione, vole si dì ch’elli ponu esse tradutti direttamente da _OmegaT_ senza impiegà a prucedura di cunversione :
  - https://github.com/enzo1982/freac/tree/master/i18n/freac/crowdin
  - https://github.com/enzo1982/freac/tree/master/i18n/setup/crowdin
  - https://github.com/enzo1982/freac/tree/master/i18n/tips/crowdin
  - https://github.com/enzo1982/freac/tree/master/i18n/updater/crowdin
  - Esempiu di linee in un schedariu chì pò esse traduttu direttamente da _OmegaT_ :
```
    <entry id="100" string="OK">OK</entry>
    <entry id="101" string="Cancel">Cancel</entry>
    <entry id="102" string="Close">Close</entry>
```
## Installazione di a prucedura

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
        <Macro name="Cunversione freac.XML-OmegaT" Ctrl="no" Alt="no" Shift="no" Key="0">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per mudificà e catene chì cuntenenu entry è string" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='(.*)<entry id="(.*)" string="(.*)"\/>' />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam='\1<entry id="\2" string="\3">\3</entry>' />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
```
- Tandu a nova prucedura - `Cunversione freac.XML-OmegaT` - hè dispunibule in _Notepad++_.
- Di sicuru, si pò sceglie __un altru nome di prucedura__.  

Per a vostra infurmazione, l’istruzzione `message="2172"` in sta prucedure cuntene un cummentu per spiegà ciò chì si face dentru. Ùn si pò micca impiegà i cummenti classichi di u XML perchè quelli cummenti sò autumaticamente squassati quandu ci hè una mudificazione di u schedariu `shortcuts.xml` da _Notepad++_, per indettu per arregistrà una nova prucedura macro arricurdata.

## Impiegu di a prucedura

- Lancià _Notepad++_
- Apre u schedariu di traduzzione ch’ellu ci vole à cunvertisce
- Sceglie `Macro`, eppò `Eseguisce una macro parechje volte…`
- Selezziunà u nome di a prucedura à impiegà : `Cunversione freac.XML-OmegaT`
- Cliccu nant’à `Eseguisce 1 volta`
- Appughjà nant’à u buttone `Eseguisce`
- Arregistrà u schedariu trasfurmatu cù l’estensione `.xml`
- Cupià stu schedariu in u cartulare `/source/` di u prughjettu __freac__ in _OmegaT_.

#### Liami di navigazione nant’à stu situ
- [Rivene à a lista di i membri di stu prughjettu](./)
- [Rivene à a lista di tutti i prughjetti](../)
- [Rivene à a lista di tutti i prugrammi](../../../../#readme)
