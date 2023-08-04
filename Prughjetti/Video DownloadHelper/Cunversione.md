# Prucedura di cunversione di i schedarii di traduzzione _Video DownloadHelper_

Eccu una prucedura di cunversione di u schedariu di traduzzione _Video DownloadHelper_ per ch’ellu sia accettatu da  __OmegaT__, attrezzu di traduzzione assistita da l’urdinatore.

## Scopu di a prucedura

Per disgrazia, i schedarii di traduzzione `.json` di _Video DownloadHelper_ ùn ponu micca esse tradutti direttamente da _OmegaT_ è ci vole à trasfurmà u furmatu di u so cuntenutu. Eccu una prucedura macro chì si pò caricà è impiegà in _Notepad++_ per fà sta trasfurmazione.  

A) Esempiu di linee in u schedariu `message.json` d’origine :
```
    "save_as": {
        "message": "Save as…"
    },
       "cancel": {
        "message": "Cancel"
       },
       "default": {
        "message": "Default"
       },
	"file_ready": {
		"message": "\"$ARG1$\" is now ready",
		"placeholders": {
			"arg1": {
				"content": "$1"
			}
		}
	},
```
Eccu e listesse linee dopu à trasfurmazione cù a prucedura `Cunversione VDH(.json)-OmegaT(.json)` :
```
    "save_as": "Save as…",
    "cancel": "Cancel",
    "default": "Default",
    "file_ready": "\"$ARG1$\" is now ready",
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
        <Macro name="Cunversione VDH(.json)-OmegaT(.json)" Ctrl="no" Alt="no" Shift="no" Key="0">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per caccià e linee chì cuntenenu [argn] è [content] nant'à a linea chì seguiteghja" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="^\s+&quot;(arg1|arg2|arg3|arg4|arg5|arg6|arg7|arg8|arg9)&quot;(:|\s*:)\s+{\n\s+&quot;content&quot;(:|\s*:)\s+&quot;(.*)&quot;\n\s+(}|},)\n" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per caccià e linee chì cuntenenu [placeholders]" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam=",$\n\s+&quot;placeholders&quot;:\s*{\n\s+}" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per trasfurmà e linee chì cuntenenu [message]" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="{$\n\s+&quot;message&quot;:\s+&quot;(.*)&quot;\n\s+}" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="&quot;\1&quot;" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Cumanda nurmale per caccià tutte e linee viote" />
            <Action type="2" message="0" wParam="42055" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per impiegà u listessu numeru di spazii à u principiu di tutte e linee" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="^\s+&quot;(.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="    &quot;\1" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
```
- Tandu a nova prucedura - `Cunversione VDH(.json)-OmegaT(.json)` - hè dispunibule in _Notepad++_.
- Di sicuru, si pò sceglie __un altru nome di prucedura__.  

Per a vostra infurmazione, ci hè parechje istruzzioni `message="2172"` in ste prucedure chì cuntenenu un cummentu per spiegà ciò chì si face dentru. Ùn si pò micca impiegà i cummenti classichi di u XML perchè quelli cummenti sò autumaticamente squassati quandu ci hè una mudificazione di u schedariu `shortcuts.xml` da _Notepad++_, per indettu per arregistrà una nova prucedura macro arricurdata.

## Impiegu di a prucedura

- Lancià _Notepad++_
- Apre u schedariu di traduzzione ch’ellu ci vole à cunvertisce
- Sceglie `Macro`, eppò `Eseguisce una macro parechje volte…`
- Selezziunà u nome di a prucedura à impiegà : `Cunversione VDH(.json)-OmegaT(.json)`
- Cliccu nant’à `Eseguisce 1 volta`
- Appughjà nant’à u buttone `Eseguisce`
- Arregistrà u schedariu trasfurmatu cù un nome sfarente, per indettu : `omegat_message.json`
- Cupià stu schedariu in u cartulare `/source/` di u prughjettu __Video DownloadHelper__ in _OmegaT_.

#### Liami di navigazione nant’à stu situ
- [Rivene à a lista di i membri di stu prughjettu](./)
- [Rivene à a lista di tutti i prughjetti](../)
- [Rivene à a lista di tutti i prugrammi](../../../../#readme)
