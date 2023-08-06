# Prucedure di cunversione di u schedarii di traduzzione _VeraCrypt_

Quandu u schedariu di traduzzione `.xml` di _VeraCrypt_ ùn pò micca esse traduttu direttamente da _OmegaT_, ci vole à trasfurmà u furmatu di u so cuntenutu. Stu tipu di trasfurmazione si pò fà grazia à una prucedura ch’ella si pò caricà è impiegà in _Notepad++_.

## Scopu di e prucedure

Ci hè parechje prucedure dispunibule per fà a cunversione di u schedariu di traduzzione _VeraCrypt_ è trasfurmà u so furmatu d’origine `.xml` in un altru furmatu `.isl` o`.lng`.

Eccu un esempiu di linee chì si trovanu in u schedariu `Language.xml` d’origine :
```
    <entry lang="en" key="IDCANCEL">Cancel</entry>
    <entry lang="en" key="IDC_ALL_USERS">Install &amp;for all users</entry>
    <entry lang="en" key="IDC_BROWSE">Bro&amp;wse...</entry>
    <entry lang="en" key="IDC_DESKTOP_ICON">Add VeraCrypt icon to &amp;desktop</entry>
    <entry lang="en" key="IDC_DONATE">Donate now...</entry>
```
Eccu e listesse linee dopu à una trasfurmazione cù e prucedure `Cunversione VeraCrypt(.xml)-OmegaT(.isl)` o `Cunversione VeraCrypt(.xml)-OmegaT(.lng)` :
```
IDCANCEL=Cancel
IDC_ALL_USERS=Install &for all users
IDC_BROWSE=Bro&wse...
IDC_DESKTOP_ICON=Add VeraCrypt icon to &desktop
IDC_DONATE=Donate now...
```
A sfarenza trà ste duie prucedure hè chì a prima - impieghendu u furmatu `.isl` - permette a trasfurmazione in l’altru sensu grazia à una terza prucedura : `Cunversione OmegaT(.isl)-VeraCrypt(.xml)`.

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
        <Macro name="Cunversione VeraCrypt(.xml)-OmegaT(.isl)" Ctrl="no" Alt="no" Shift="no" Key="0" FolderName="Cunversioni VeraCrypt">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per aghjunghje un caratteru speziale davanti à tutte e linee" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="^" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam=";" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per trasfurmà e linee |entry|" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="^;(.*)\s+key=&quot;(.*)&quot;&gt;(.*)&lt;/entry&gt;" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\2=\3" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Cumanda nurmale per rimpiazzà u segnu di u è cummerciale in tutte e catene" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="&amp;amp;" />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="&amp;" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
        <Macro name="Cunversione OmegaT(.isl)-VeraCrypt(.xml)" Ctrl="no" Alt="no" Shift="no" Key="0" FolderName="Cunversioni VeraCrypt">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per aghjunghje un secondu caratteru speziale davanti à tutte e linee" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="^" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="§" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per trasfurmà e linee sfarente di |entry|" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="^§;(.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\1" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per trasfurmà e linee |entry|" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="^§(.*)=(.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\t&lt;entry lang=&quot;co&quot; key=&quot;\1&quot;&gt;\2&lt;/entry&gt;" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Cumanda nurmale per rimpiazzà u segnu di u è cummerciale in tutte e catene" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="&amp;" />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="&amp;amp;" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
        <Macro name="Cunversione VeraCrypt(.xml)-OmegaT(.lng)" Ctrl="no" Alt="no" Shift="no" Key="0" FolderName="Cunversioni VeraCrypt">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per caccià i cummenti, ancu s'elli si trovanu nant'à parechje linee" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="&amp;lt;!--.*?--&amp;gt;" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per indettà tutte e linee |entry|" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="^\s+&lt;entry\s+(.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="784" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1615" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Cumanda nurmale per caccià tutte e linee senza indetta" />
            <Action type="2" message="0" wParam="43051" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Cumanda nurmale per viutà e marche di tutte e linee indettate" />
            <Action type="2" message="0" wParam="43008" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Cumanda nurmale per rimpiazzà u segnu di u è cummerciale in tutte e catene" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="&amp;amp;" />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="&amp;" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per trasfurmà e linee |entry|" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="(.*)\s+key=&quot;(.*)&quot;&gt;(.*)&lt;/entry&gt;" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\2=\3" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
```
- Tandu e prucedure nove sò dispunibule in _Notepad++_.
- Di sicuru, si pò sceglie __un altru nome per ogni prucedura__.  

Per a vostra infurmazione, ci hè parechje istruzzioni `message="2172"` in ste prucedure chì cuntenenu un cummentu per spiegà ciò chì si face dentru. Ùn si pò micca impiegà i cummenti classichi di u XML perchè quelli cummenti sò autumaticamente squassati quandu ci hè una mudificazione di u schedariu `shortcuts.xml` da _Notepad++_, per indettu per arregistrà una nova prucedura macro arricurdata.

## Impiegu di a prucedura

- Lancià _Notepad++_
- Apre u schedariu di traduzzione ch’ellu ci vole à cunvertisce
- Sceglie `Macro`, eppò `Eseguisce una macro parechje volte…`
- Selezziunà u nome di a prucedura à impiegà, per indettu : `Cunversione VeraCrypt(.xml)-OmegaT(.isl)`
- Cliccu nant’à `Eseguisce 1 volta`
- Appughjà nant’à u buttone `Eseguisce`
- Arregistrà u schedariu trasfurmatu cù un nome sfarente, per indettu : `Language.omegat.isl`
- Cupià stu schedariu in u cartulare `/source/` di u prughjettu __VeraCrypt__ in _OmegaT_.

#### Liami di navigazione nant’à stu situ
- [Rivene à a lista di i membri di stu prughjettu](./)
- [Rivene à a lista di tutti i prughjetti](../)
- [Rivene à a lista di tutti i prugrammi](../../../../#readme)
