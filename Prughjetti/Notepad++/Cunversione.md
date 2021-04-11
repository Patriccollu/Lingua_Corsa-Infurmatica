# Prucedura di cunversione di schedariu di traduzzione Notepad++

Eccu una prucedura di cunversione di schedariu di traduzzione Notepad++ per ch’ellu sia accettatu da  __OmegaT__, attrezzu di traduzzione assistita da l’urdinatore.

## Scopu di a prucedura

Per disgrazia, un schedariu di traduzzione `.xml` di Notepad++ - cum’è __english.xml__ - ùn pò micca esse traduttu direttamente da OmegaT è ci vole à trasfurmà u furmatu di u so cuntenutu. Eccu una prucedura macro - `Cunversione_Notepad-OmegaT` - chì si pò caricà è impiegà in Notepad++ per fà sta trasfurmazione.  

Esempiu di linee in u schedariu d’origine :
```
                    <Item id="21224" name="Open:"/>
            <replace-in-files-progress-title value="Replace In Files progress..."/>
```
Eccu e listesse linee dopu à trasfurmazione :
```
	21224=Open:
	replace-in-files-progress-title=Replace In Files progress...
```
Ste linee ponu esse arregistrate in un schedariu cù l’estensione `.lng` chì hè un furmatu cunnisciutu da OmegaT.

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
        <Macro name="Cunversione_Notepad-OmegaT" Ctrl="no" Alt="no" Shift="no" Key="0">
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='&lt;Item id=&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="1" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='&lt;Item menuId=&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="1" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='&lt;Item subMenuId=&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="1" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='&lt;Item idName=&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="1" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='&quot;    name=&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="1" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="=" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='&quot;   name=&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="1" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="=" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='&quot;  name=&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="1" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="=" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='&quot; name=&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="1" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="=" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam=' name=&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="1" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="=" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam=' title=&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="1" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="=" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam=' value=&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="1" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="=" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='&lt;Item CMID=&quot;' />
            <Action type="3" message="1625" wParam="0" lParam="1" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="CMID_" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='&quot;/&gt;' />
            <Action type="3" message="1625" wParam="0" lParam="1" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='&quot;&gt;' />
            <Action type="3" message="1625" wParam="0" lParam="1" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="&lt;" />
            <Action type="3" message="1625" wParam="0" lParam="1" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2013" wParam="0" lParam="0" sParam="" />
            <Action type="2" message="0" wParam="42043" lParam="0" sParam="" />
        </Macro>
```
- Tandu a nova prucedura - `Cunversione_Notepad-OmegaT` - hè dispunibule in Notepad++.  
 
    Di sicuru, si pò sceglie __un altru nome di prucedura__.

## Impiegu di a prucedura

- Lancià Notepad++

- Apre un schedariu di traduzzione ch’ellu ci vole à cunvertisce, per indettu : `english.xml`

- Sceglie `Macro`, eppò `Eseguisce una macro parechje volte…`

- Selezziunà `Cunversione_Notepad-OmegaT`

- Cliccu nant’à `Eseguisce 1 volta`

- Appughjà nant’à u buttone `Eseguisce`

- Arregistrà u schedariu trasfurmatu cù l’estensione `.lng`
 
- Cupià stu schedariu in u cartulare `/source/` di u prughjettu __Notepad++__ in _OmegaT_.

#### Liami di navigazione nant’à stu situ
- [Rivene à a lista di i membri di stu prughjettu](./)
- [Rivene à a lista di tutti i prughjetti](../)
- [Rivene à a lista di tutti i prugrammi](../../../../#readme)
