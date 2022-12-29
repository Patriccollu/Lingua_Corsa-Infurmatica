# Prucedura di cunversione di i schedarii di traduzzione _Mozilla VPN_

In fatti, fine à u mezu di u 2021, era pussibule di traduce direttamente da _OmegaT_ i schedarii `.xliff` di _Mozilla VPN_. Ma à st’epica, anu cambiatu u so furmatu è avà, ùn hè più pussibule.  

Eccu duie prucedure di cunversione di sti schedarii `.xliff` per ch’elli sianu accettati da  __OmegaT__, attrezzu di traduzzione assistita da l’urdinatore.  

I schedarii di traduzzione cù u furmatu `.ftl` ùn sò micca cuncernati da sta trasfurmazione.

## Scopu di e prucedure

Perchè i schedarii di traduzzione `.xliff` di _Mozilla VPN_ ùn ponu più esse tradutti direttamente da _OmegaT_, ci vole à trasfurmà u furmatu di u so cuntenutu.  

Eccu a prima prucedura macro chì si pò caricà è impiegà in _Notepad++_ per fà sta trasfurmazione : `Cunversione Mozilla VPN(XLIFF)-OmegaT(XLIFF)`

A) Esempiu di linee in u schedariu d’origine `mozillavpn.xliff` :
```
<?xml version='1.0' encoding='UTF-8'?>
<xliff xmlns="urn:oasis:names:tc:xliff:document:1.2" version="1.2">
  <file original="../../nebula/ui/components/VPNAboutUs.qml" datatype="plaintext" source-language="en" target-language="en-US">
    <body>
      <trans-unit id="vpn.aboutUs.privacyNotice2">
        <source>Privacy notice</source>
      </trans-unit>
      <trans-unit id="vpn.aboutUs.releaseVersion2">
        <note annotates="source" from="developer">Refers to the installed version. For example: "Release Version: 1.23"</note>
        <source>Release version</source>
      </trans-unit>
...[]...
      <trans-unit id="vpn.settings.aboutUs">
        <source>About us</source>
      </trans-unit>
    </body>
  </file>
```
B1) Eccu e listesse linee dopu a trasfurmazione cù a prucedura `Cunversione Mozilla VPN(XLIFF)-OmegaT(XLIFF)` :
```
<?xml version='1.0' encoding='UTF-8'?>
<xliff xmlns="urn:oasis:names:tc:xliff:document:1.2" version="1.2">
  <file original="../../nebula/ui/components/VPNAboutUs.qml" datatype="plaintext" source-language="en" target-language="en-US">
    <body>
      <trans-unit id="vpn.aboutUs.privacyNotice2">
        <source>Privacy notice</source>
        <target xml:lang="co">Privacy notice</target>
      </trans-unit>
      <trans-unit id="vpn.aboutUs.releaseVersion2">
        <note annotates="source" from="developer">Refers to the installed version. For example: "Release Version: 1.23"</note>
        <source>Release version</source>
        <target xml:lang="co">Release version</target>
      </trans-unit>
...[]...
      <trans-unit id="vpn.settings.aboutUs">
        <source>About us</source>
        <target xml:lang="co">About us</target>
      </trans-unit>
    </body>
  </file>
```
S’ella hè bisognu, ci hè dinù una seconda prucedura di cunversione chì si chjama `Cunversione Mozilla VPN(XLIFF)-OmegaT(TXT)` per trasfurmà un schedariu `.xliff` in furmatu testu simplice. In stu casu, l’estensione di u schedariu trasfurmatu serà `.txt`.  

B2) Eccu e listesse linee dopu à trasfurmazione cù a prucedura `Cunversione Mozilla VPN(XLIFF)-OmegaT(TXT)` :
```
Privacy notice
Release version
...[]...
About us
```

## Installazione di e prucedure

- Apre u cartulare di _Notepad++_ induve si trova u schedariu `shortcuts.xml` perchè ghjè quellu chì cuntene tutte e vostre prucedure persunalizate. Da bona regula, stu cartulare si trova in `C:\Users\xxxxxxxx\AppData\Roaming\Notepad++` (induve _xxxxxxxx_ hè u vostru nome d’utilizatore).  

    Per apre stu cartulare d’una manera più faciule, ci vole à fà una ricerca Windows cù sta catena : `%APPDATA%\Notepad++`

- In u cartulare chì s’apre, sciglite u schedariu `shortcuts.xml` è apritelu cù _Notepad++_

- Dentru u schedariu, dopu l’istruzzione `<Macros>`, ci hè unu o parechji gruppi d’istruzzioni chì s’assumiglianu à què :
```
	<Macro name=".......">
	   ...
	   ...
	   ...
	</Macro>
```
- Basta à aghjunghje tutte st’istruzzioni __nanzu__ a linea `</Macros>` chì indicheghja a fine di tutte e prucedure macro
```
        <Macro name="Cunversione Mozilla VPN(XLIFF)-OmegaT(XLIFF)" Ctrl="no" Alt="no" Shift="no" Key="0">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam='Espressione regulare per aghjunghje una linea <target> dopu à ogni linea <source>' />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='(.*)<source>(.*)</source>' />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam='\1<source>\2</source>\n\1<target xml:lang="co">\2</target>' />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam='Rimpiazzamentu nurmale di e catene [target-language="en-US"] da [target-language="co"]' />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam='target-language="en-US"' />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam='target-language="co"' />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
        <Macro name="Cunversione Mozilla VPN(XLIFF)-OmegaT(TXT)" Ctrl="no" Alt="no" Shift="no" Key="0">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Marca e indetta e linee cuntenendu |<source>|" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="&lt;source&gt;" />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="784" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1615" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Marca e indetta e linee cuntenendu |</source>|" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="&lt;/source&gt;" />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="784" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1615" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Caccia e linee senza marca" />
            <Action type="2" message="0" wParam="43051" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Rimpiazzamentu nurmale di |<source>| da ||" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="&lt;source&gt;" />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Rimpiazzamentu nurmale di |</source>| da ||" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="&lt;/source&gt;" />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Viura tutte l'indette" />
            <Action type="2" message="0" wParam="42042" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Ammuzza i spazii di principiu di linea" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="16" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1633" sParam="" />
        </Macro>
```
- Tandu e prucedure nove sò dispunibule in _Notepad++_
- Di sicuru, si pò sceglie __un altru nome__ di prucedura  

Per a vostra infurmazione, ci hè parechje istruzzioni `message="2172"` in ste prucedure chì cuntenenu un cummentu per spiegà ciò chì si face dentru. Ùn si pò micca impiegà i cummenti classichi di u XML perchè quelli cummenti sò autumaticamente squassati quandu ci hè una mudificazione di u schedariu `shortcuts.xml` da _Notepad++_, per indettu per arregistrà una nova prucedura macro arricurdata.

## Impiegu di a prucedura

- Lancià _Notepad++_
- Apre u schedariu di traduzzione ch’ellu ci vole à cunvertisce
- Sceglie `Macro`, eppò `Eseguisce una macro parechje volte…`
- Selezziunà u nome di a prucedura à impiegà
- Cliccu nant’à `Eseguisce 1 volta`
- Appughjà nant’à u buttone `Eseguisce`
- Arregistrà u schedariu trasfurmatu cù l’estensione `.xliff` o `.txt` secondu à a prucedura impiegata
- Cupià stu schedariu in u cartulare `/source/` di u prughjettu __Mozilla VPN__ in _OmegaT_

#### Liami di navigazione nant’à stu situ
- [Rivene à a lista di i membri di stu prughjettu](./)
- [Rivene à a lista di tutti i prughjetti](../)
- [Rivene à a lista di tutti i prugrammi](../../../../#readme)
