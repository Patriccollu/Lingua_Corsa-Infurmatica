# Prucedura di cunversione di i schedarii di traduzzione _VLC_

Eccu duie prucedure di cunversione di i schedarii di traduzzione _VLC_ per ch’elli sianu accettati da  __OmegaT__, attrezzu di traduzzione assistita da l’urdinatore.

## Scopu di e prucedure

Per disgrazia, i schedarii di traduzzione `.strings` di _VLC_ ùn ponu micca esse tradutti direttamente da _OmegaT_ è ci vole à trasfurmà u furmatu di u so cuntenutu. Eccu duie prucedure macro chì si pò caricà è impiegà in _Notepad++_ per fà sta trasfurmazione :
1. `Cunversione VLC(.strings)-OmegaT(.strings)` per trasfurmà u cuntenutu di i schedarii `.strings` da u so furmatu d’origine ver di un furmatu cunnisciutu da _OmegaT_
2. `Cunversione OmegaT(.strings)-VLC(.strings)` per fà a trasfurmazione à l’arritrosa, vole si dì trasfurmà u cuntenutu di i schedarii `.strings` da u furmatu cunnisciutu da _OmegaT_ ver di u so furmatu d’origine

Esempiu di linee in un schedariu `.strings` d’origine :
```
"CHOOSE_AUDIO_TRACK" = "Choose Audio Track";
// 1st comment
"CHOOSE_SUBTITLE_TRACK" = "Choose Subtitle Track"; /* 2nd comment */
"UNKNOWN_TRACK_TYPE" = "Unknown track type"; // 3rd comment
```
Eccu e listesse linee dopu à trasfurmazione cù a prucedura `Cunversione VLC.STRINGS-OmegaT` :
```
"CHOOSE_AUDIO_TRACK" =Choose Audio Track

"CHOOSE_SUBTITLE_TRACK" =Choose Subtitle Track
"UNKNOWN_TRACK_TYPE" =Unknown track type
```
A seconda prucedura rimette u schedariu à u so furmatu d’origine, senza i cummenti chì sò stati cacciati.
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
        <Macro name="Cunversione VLC(.strings)-OmegaT(.strings)" Ctrl="no" Alt="no" Shift="no" Key="0" FolderName="Cunversioni VLC">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per caccià i cummenti chì si trovanu daretu i caratteri // in tutti i schedarii" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="^//(.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1635" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per caccià i cummenti chì si trovanu trà i caratteri /* è */ in tutti i schedarii" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="/\*([^*]|[\r\n]|(\*+([^*/]|[\r\n])))*\*+/" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1635" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per trasfurmà u restu di a linea in tutti i schedarii" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="&quot;(.*)&quot;\s*=\s*&quot;(.*)&quot;\s*;(.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="&quot;\1&quot; = \2" />
            <Action type="3" message="1702" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1635" sParam="" />
        </Macro>
        <Macro name="Cunversione OmegaT(.strings)-VLC(.strings)" Ctrl="no" Alt="no" Shift="no" Key="0" FolderName="Cunversioni VLC">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per trasfurmà u restu di a linea in tutti i schedarii" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="&quot;(.*)&quot;\s*=\s*(.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="&quot;\1&quot; = &quot;\2&quot;;" />
            <Action type="3" message="1702" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1635" sParam="" />
        </Macro>
```
- Tandu e duie prucedure nove sò dispunibule in _Notepad++_.
- Di sicuru, si pò sceglie __un altru nome di prucedura__.  

Per a vostra infurmazione, ci hè parechje istruzzioni `message="2172"` in ste prucedure chì cuntenenu un cummentu per spiegà ciò chì si face dentru. Ùn si pò micca impiegà i cummenti classichi di u XML perchè quelli cummenti sò autumaticamente squassati quandu ci hè una mudificazione di u schedariu `shortcuts.xml` da _Notepad++_, per indettu per arregistrà una nova prucedura macro arricurdata.

## Impiegu di e prucedure

Fighjate l’istruzzioni detagliate per sapè quand’ellu ci vole à impiegà ste duie prucedure :
1. [A prima prucedura](OmegaT.md#estensione-strings) `Cunversione VLC(.strings)-OmegaT(.strings)` per trasfurmà u cuntenutu di i schedarii `.strings` da u so furmatu d’origine ver di un furmatu cunnisciutu da _OmegaT_
2. [A seconda prucedura](OmegaT.md#preparazione-di-i-schedarii-dopu-a-traduzzione)`Cunversione OmegaT(.strings)-VLC(.strings)` per fà a trasfurmazione à l’arritrosa, vole si dì trasfurmà u cuntenutu di i schedarii `.strings` da u furmatu cunnisciutu da _OmegaT_ ver di u so furmatu d’origine, per ch’ella sia

#### Liami di navigazione nant’à stu situ
- [Rivene à a lista di i membri di stu prughjettu](./)
- [Rivene à a lista di tutti i prughjetti](../)
- [Rivene à a lista di tutti i prugrammi](../../../../#readme)
