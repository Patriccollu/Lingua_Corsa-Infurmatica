# Prucedure di cunversione di schedariu di traduzzione di _SumatraPDF_

Eccu parechje prucedure di cunversione di u schedariu di traduzzione di _SumatraPDF_ per ch’ellu sia accettatu da __OmegaT__, attrezzu di traduzzione assistita da l’urdinatore.  

Ste prucedure devenu esse caricate è impiegate in _Notepad++_ per fà a trasfurmazione. Ogni prucedura eseguisce un inseme di cumande per trasfurmà u cuntenutu di u schedariu apertu in _Notepad++_.

## Scopu di e prucedure

- Per disgrazia, u schedariu di traduzzione di _SumatraPDF_ ùn pò micca esse traduttu direttamente da _OmegaT_, dunque ci vole à trasfurmà u so cuntenutu cù una prucedura autumatica installata nant’à _Notepad++_.

- Ci hè dui lochi induve si pò truvà e catene in inglese chì sò à traduce, di furmatu sfarente, è mischiate cù d’altre infurmazioni :
  - nant’à una [pagina di u situ di traduzzione _apptranslator.org_](https://www.apptranslator.org/app/SumatraPDF/co)
  - nant’à un [schedariu di u situ di sviluppu _GitHub_](https://github.com/sumatrapdfreader/sumatrapdf/blob/master/src/docs/translations.txt)

- In più di què, u furmatu di l’infurmazione à traduce hè sfarente secondu à u locu induve vo avete scaricatu e catene, ma ancu di grazia ci hè una prucedura per ogni furmatu.

### Furmatu di l’infurmazione da u situ di traduzzione _apptranslator.org

```
Home : SumatraPDF : Corsican translations Not logged in. Log in with Twitter
0 untranslated out of 341 total strings
Progress:
100%

&About Add a translation... • see on Google Translate
About SumatraPDF Add a translation... • see on Google Translate
&Actual Size\tCtrl+1 => &Dimensione attuale\tCtrl+1 Edit • see on Google Translate
Add Favorite => Aghjunghje à i favuriti Edit • see on Google Translate 
```

- Una prima prucedura macro - `Cunversione SumatraPDF.APP-OmegaT` - ghjova à cunservà tutte e linee in inglese, quelle chì sò dighjà tradutte è quelle chì sò à traduce. Eccu u detagliu di quella trasfurmazione :
  - identificà solu e linee chì cuntenenu `see on Google Translate`
  - squassà tutte l’altre linee
  - caccià e linee viote
  - squassà l’identificazione nant’à e linee
  - rimpiazzà `Add a translation...` da `=>`
  - cunservà solu a parte à manca di u segnu `=>` è caccià u restu

Eccu e listesse linee dopu à trasfurmazione :
```
&About
About SumatraPDF
&Actual Size\tCtrl+1
Add Favorite
```
- Una seconda prucedura macro - `Cunversione SumatraPDF.APPn-OmegaT` - ghjova à cunservà solu e linee in inglese chì sò nove, è dunque à traduce. Eccu u detagliu di quella trasfurmazione :
  - identificà solu e linee chì cuntenenu `Add a translation...`
  - squassà tutte l’altre linee
  - caccià e linee viote
  - squassà l’identificazione nant’à e linee

Eccu e listesse linee dopu à trasfurmazione :
```
&About
About SumatraPDF
```
### Furmatu di l’infurmazione da u situ di sviluppu _GitHub_

Esempiu di linee di u schedariu `translations.txt` :
```
:&About
af:&Omtrent
am:&Ծրագրի մասին
ar:حول& 
br:Sobre
ca-xv:&Quant a...
ca:&Quant a...
cn:关于(&A)...
co:&Apprupositu
cy:&Ynghylch...
fr:&À propos
fy-nl:&Oer
it:Info progr&amma
… … …
:&Actual Size\tCtrl+1
af:&Gewone Grootte\tCtrl+1
am:Իրական &չափը\tCtrl+1
ar:الحجم &الحقيقي\tCtrl+1
az:&Faktiki ölçü\tCtrl+1
… … …
```

- Una terza prucedura macro - `Cunversione SumatraPDF.TXT-OmegaT` - ghjova à cunservà tutte e linee in inglese, quelle chì sò dighjà tradutte è quelle chì sò à traduce. Eccu u detagliu di quella trasfurmazione :
  - identificà solu e linee cù e catene in inglese, quelle chì principianu cù u segnu `:`
  - squassà tutte l’altre linee (Fate casu chì sta parte di a trasfurmazione hè appena longa)
  - caccià e linee viote
  - squassà l’identificazione nant’à e linee
  - squassà u prefissu `:` nant’à e linee identificate
  
Eccu e listesse linee dopu à trasfurmazione :
```
&About
&Actual Size\tCtrl+1
```

## Installazione di e prucedure

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
        <Macro name="Cunversione SumatraPDF.APP-OmegaT" Ctrl="no" Alt="no" Shift="no" Key="0">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Indettà solu e linee chì cuntenenu |see on Google Translate|" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="see on Google Translate" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="784" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1615" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Squassà tutte l’altre linee" />
            <Action type="2" message="0" wParam="43051" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Caccià e linee viote" />
            <Action type="2" message="0" wParam="42055" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Squassà l’identificazione nant’à e linee" />
            <Action type="2" message="0" wParam="43008" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Rimpiazzamentu nurmale di |Add a translation...| da |=>|" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="Add a translation..." />
            <Action type="3" message="1625" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="=&gt;" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per cunservà solu a parte à manca di u segnu |=>| è caccià u restu" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="^(.*) =&gt; (.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\1" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
        <Macro name="Cunversione SumatraPDF.APPn-OmegaT" Ctrl="no" Alt="no" Shift="no" Key="0">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Indettà solu e linee chì cuntenenu |Add a translation...|" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="Add a translation..." />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="784" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1615" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Squassà tutte l’altre linee" />
            <Action type="2" message="0" wParam="43051" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Caccià e linee viote" />
            <Action type="2" message="0" wParam="42055" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Squassà l’identificazione nant’à e linee" />
            <Action type="2" message="0" wParam="43008" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per cunservà solu a parte à manca di u segnu |Add a translation...| è caccià u restu" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="^(.*) Add a translation... (.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\1" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
        <Macro name="Cunversione SumatraPDF.TXT-OmegaT" Ctrl="no" Alt="no" Shift="no" Key="0">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per indettà solu e linee chì principianu cù u segnu |:|" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="^:" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="784" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1615" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Squassà tutte l’altre linee" />
            <Action type="2" message="0" wParam="43051" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Caccià e linee viote" />
            <Action type="2" message="0" wParam="42055" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Squassà l’identificazione nant’à e linee" />
            <Action type="2" message="0" wParam="43008" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per squassà u prefissu |:| nant’à e linee identificate" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="^:(.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\1" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
```
- Tandu e nove prucedure - `Cunversione SumatraPDF.APP-OmegaT` è `Cunversione SumatraPDF.TXT-OmegaT` - sò dispunibule in _Notepad++_.
- Di sicuru, si pò sceglie __d’altri nomi di prucedura__.  

Per a vostra infurmazione, si pò truvà in una prucedura, istruzzioni `message="2172"` chì cuntenenu un cummentu per spiegà ciò chì si face dentru. Ùn si pò micca impiegà i cummenti classichi di u XML perchè quelli cummenti sò autumaticamente squassati quandu ci hè una mudificazione di u schedariu `shortcuts.xml` da _Notepad++_, per indettu per arregistrà una nova prucedura macro arricurdata.

## Impiegu di e prucedure

- Seguitate l’istruzzioni secondu à u locu induve vo avete scaricatu e catene :
  - nant’à a [pagina di u situ di traduzzione _apptranslator.org_](OmegaT.md#da-una-pagina-di-u-situ-di-traduzzione-apptranslatororg)
  - nant’à u [schedariu di u situ di sviluppu _GitHub_](OmegaT.md#da-u-schedariu-unicu-di-u-situ-di-sviluppu-github)

#### Liami di navigazione nant’à stu situ
- [Rivene à a lista di i membri di stu prughjettu](./)
- [Rivene à a lista di tutti i prughjetti](../)
- [Rivene à a lista di tutti i prugrammi](../../../../#readme)
