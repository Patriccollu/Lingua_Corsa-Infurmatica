# Prucedure di cunversione di schedariu di traduzzione di _SumatraPDF_

Eccu parechje prucedure di cunversione di u schedariu di traduzzione di _SumatraPDF_ per ch’ellu sia accettatu da __OmegaT__, attrezzu di traduzzione assistita da l’urdinatore.  

Ste prucedure devenu esse caricate è impiegate in _Notepad++_ per fà a trasfurmazione. Ogni prucedura eseguisce un inseme di cumande per trasfurmà u cuntenutu di u schedariu apertu in _Notepad++_.

## Scopu di e prucedure

- E traduzzioni di _SumatraPDF_ sò amministrate nant’à un situ web da un’appiecazione particulare chì si chjama _App Translator_ chì permette a mudificazione in linea di e catene, sia una catena dopu à l’altra, sia tutte e catene inseme via a funzione « Bulk ».
- Per disgrazia, _App Translator_ ùn permette, nè d’espurtà, nè d’impurtà un schedariu di traduzzione chì cuntene tutte e catene.
- Dunque, ciò chì si pò fà hè una copia di i dati grossi di tutte e catene chì sò affissate da _App Translator_ è di trasfurmale in un furmatu di testu accettatu da _OmegaT_ via una prucedura autumatica installata nant’à _Notepad++_.

- Eccu a pagina di u situ web induve _App Translator_ affisseghja e catene in inglese chì sò à traduce è quelle chì sò dighjà tradutte in lingua corsa :
  - [pagina di u situ di traduzzione _apptranslator.org_](https://www.apptranslator.org/app/SumatraPDF/co)

### Esempiu d’infurmazione affissata nant’à a pagina di traduzzione da u situ _apptranslator.org_

```
Home : SumatraPDF : Corsican, 1090 strings	history                     Logged in as Patriccollu (logout)

				Edit many translations at once

# History => # Cronolugia (by Patriccollu on 26-09-06)                           Edit •  Google Translate
	# Storicu (by ai claude on 26-09-04)
$ Favorites => $ Favuriti (by ai claude on 26-07-29)                             Edit •  Google Translate
% TOC => % Tavula di cuntenutu (by Patriccollu on 26-08-27)                      Edit •  Google Translate
	% TDM (by ai claude on 26-08-19)
%s not supported => %s micca ricunnisciutu (by Patriccollu on 26-08-27)          Edit •  Google Translate
	%s micca supportatu (by ai claude on 26-07-29)
3D => 3D (by ai claude on 26-07-29)                                              Edit •  Google Translate
= Settings => = Parametri (by ai claude on 26-09-04)                             Edit •  Google Translate
```

Quandu si face una copia simplice di st’infurmazione, è ch’ella s’incolla in u preme’papei, eccu ciò chì si trova :
```
Home : SumatraPDF : Corsican, 1090 strings history Logged in as Patriccollu (logout)

Edit many translations at once
# History => # Cronolugia (by Patriccollu on 26-09-06)
# Storicu (by ai claude on 26-09-04)
Edit •  Google Translate
$ Favorites => $ Favuriti (by ai claude on 26-07-29)
Edit •  Google Translate
% TOC => % Tavula di cuntenutu (by Patriccollu on 26-08-27)
% TDM (by ai claude on 26-08-19)
Edit •  Google Translate
%s not supported => %s micca ricunnisciutu (by Patriccollu on 26-08-27)
%s micca supportatu (by ai claude on 26-07-29)
Edit •  Google Translate
3D => 3D (by ai claude on 26-07-29)
Edit •  Google Translate
= Settings => = Parametri (by ai claude on 26-09-04)
Edit •  Google Translate
```

- Una prima prucedura macro - `Cunversione SumatraPDF.APP.inglese-OmegaT(.txt)` - ghjova à cunservà tutte e linee in inglese, quelle chì sò dighjà tradutte è quelle chì sò sempre à traduce. Eccu u detagliu di quella trasfurmazione :
  - indettà e linee in attesa di traduzzione chì cuntenenu | => | trà duie altre parte
  - trasfurmà ste linee per cunservà solu a prima parte chì cuntene a catena à traduce
  - indettà e linee tradutte chì cuntenenu u segnu | => |
  - trasfurmà ste linee per cunservà solu a prima parte chì cuntene a catena à traduce
  - squassà tutte l’altre linee

Eccu e linee di u listessu esempiu dopu sta trasfurmazione :
```
# History
$ Favorites
% TOC
%s not supported
3D
= Settings
```

- Una seconda prucedura macro - `Cunversione SumatraPDF.APP.tuttu-Tavula(.xlsx)` - ghjova à cunservà tutte e linee in inglese chì sò dighjà tradutte in lingua corsa è di piazzalle in 4 culonne : nome di u traduttore, data di a mudificazione, catena d’origine in inglese, è catena tradutta in corsu. Eccu u detagliu di quella trasfurmazione :
  - indettà e linee tradutte, quelle chì cuntenenu u segnu | => |
  - squassà tutte l’altre linee
  - trasfurmà ste linee per cunservà e 4 parti, in un altru ordine, staccate da una tabulazione : traduttore, data di a traduzzione, catena d’origine è traduzzione
  
Eccu e linee di u listessu esempiu dopu sta trasfurmazione :
```
Patriccollu	26-09-06	# History	# Cronolugia
ai claude	26-07-29	$ Favorites	$ Favuriti
Patriccollu	26-08-27	% TOC	% Tavula di cuntenutu
Patriccollu	26-08-27	%s not supported	%s micca ricunnisciutu
ai claude	26-07-29	3D	3D
ai claude	26-09-04	= Settings	= Parametri
```

- Eccu una terza prucedura macro - `Cunversione SumatraPDF.APP.AI.ordinata-Tavula(.txt)` - chì ghjova à cunservà solu e linee mudificate da l’intelligenza artificiale è ordinalle da a più recente à a più vechja. Eccu u detagliu di quella trasfurmazione :
  - indettà e linee chì cuntenenu un nome di traduttore chì principia da |ai |
  - squassà tutte l’altre linee
  - trasfurmà ste linee per piazzà a data di mudificazione in a prima culonna
  - ordinà tutte ste linee secondu à sta data, da a più recente à a più vechja

Eccu e listesse linee dopu à trasfurmazione :
```
26-09-04	ai claude	= Settings	= Parametri
26-07-29	ai claude	3D	3D
26-07-29	ai claude	$ Favorites	$ Favuriti
```

### Esempiu d’infurmazione affissata nant’à a pagina di cronolugia da u situ _apptranslator.org_
Cù AppTranslator, si pò dinù affissà a cronolugia di tutte e mudificazioni fatte per a lingua corsa, clicchendu nant’à « History » à u principiu di a pagina di traduzzione :
  - [pagina di a cronolugia di e traduzzioni _apptranslator.org_](https://www.apptranslator.org/app/SumatraPDF/history?lang=co)

Eccu un esempiu di ciò chì s’affisseghja :
```
 Home : SumatraPDF : Corsican : History                                Logged in as Patriccollu (logout)

1970 translations in Corsican — all languages

prev · page 1 of 2 · next
user 	lang 	age 	string 	translation
Patriccollu 	co 	0d 	&Manual 	&Manuale in linea (in inglese)
Patriccollu 	co 	0d 	File %s not found 	Ùn si pò truvà u schedariu %s
Patriccollu 	co 	0d 	Enter run command 	Stampittà a cumanda à lancià
ai claude 	co 	1d 	Visual Search With Google &Lens 	Ricerca Visuale cù Google Lens
ai claude 	co 	1d 	Too large for this DPI 	Troppu grande per stu DPI
ai claude 	co 	1d 	Serial Number: 	Numeru di Serie:
ai claude 	co 	1d 	&Page 	Pagina
Patriccollu 	co 	4d 	Show Comment 	Affissà u cummentu
Patriccollu 	co 	4d 	Search syntax: 	Sintassa di ricerca :
Patriccollu 	co 	4d 	Reading stopped 	Lettura piantata
```

- Eccu un’altra prucedura macro - `Cunversione SumatraPDF.APP.crono.ordinata-Tavula(.xlsx)` - chì ghjova à cunservà tutte e linee di a cronolugia di traduzzione è d’arritrusà l’ordine di ste linee. Di più a prucedura caccia u spaziu chì si trova à a fine d’ogni culonne. Eccu u detagliu di quella trasfurmazione :
  - indettà e linee tradutte chì cuntenenu a catena |co | trà dui tabulazioni
  - squassà tutte l’altre linee
  - trasfurmà ste linee cambiendu l’ordine di e 4 parti staccate da una tabulazione : nome di u traduttore, co, età di a mudificazione, catena d’origine in inglese, è catena tradutta in corsu
  - arritrusà l’ordine di tutte e linee
  
Eccu e listesse linee dopu à trasfurmazione :
```
Patriccollu	co	4d	Reading stopped	Lettura piantata
Patriccollu	co	4d	Search syntax:	Sintassa di ricerca :
Patriccollu	co	4d	Show Comment	Affissà u cummentu
ai claude	co	1d	&Page	Pagina
ai claude	co	1d	Serial Number:	Numeru di Serie:
ai claude	co	1d	Too large for this DPI	Troppu grande per stu DPI
ai claude	co	1d	Visual Search With Google &Lens	Ricerca Visuale cù Google Lens
Patriccollu	co	0d	Enter run command	Stampittà a cumanda à lancià
Patriccollu	co	0d	File %s not found	Ùn si pò truvà u schedariu %s
Patriccollu	co	0d	&Manual	&Manuale in linea (in inglese)
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
        <Macro name="Cunversione SumatraPDF.APP.inglese-OmegaT(.txt)" Ctrl="no" Alt="no" Shift="no" Key="0" FolderName="Cunversioni SumatraPDF">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per indettà e linee in attesa di traduzzione chì si finiscenu da |Add a translation...|" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="Add a translation...$" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="784" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1615" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per trasfurmà e linee in attesa di traduzzione chì si finiscenu da |Add a translation...|, per cunservà solu a catena inglese" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="(.*) Add a translation...$" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\1" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per indettà solu e linee tradutte, dunque quelle chì cuntenenu u segnu | => |" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="(.*) => (.*) \((.*)\)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="784" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1615" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per trasfurmà e linee tradutte, dunque quelle chì cuntenenu u segnu | => |, per cunservà solu a catena inglese" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="(.*) => (.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\1" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Cumanda nurmale per caccià tutte e linee senza indetta" />
            <Action type="2" message="0" wParam="43051" lParam="0" sParam="" />
        </Macro>
        <Macro name="Cunversione SumatraPDF.APP.tuttu-Tavula(.xlsx)" Ctrl="no" Alt="no" Shift="no" Key="0" FolderName="Cunversioni SumatraPDF">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per indettà solu e linee tradutte, dunque quelle chì cuntenenu u segnu | => |" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="(.*) => (.*) \(by (.*) on (.*)\)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="784" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1615" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Cumanda nurmale per caccià tutte e linee senza indetta" />
            <Action type="2" message="0" wParam="43051" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per trasfurmà e linee tradutte, dunque quelle chì cuntenenu u segnu | => |, in 4 culonne per esse cupiate in un tabulatore" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="(.*) => (.*) \(by (.*) on (.*)\)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\3\t\4\t\1\t\2" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
        </Macro>
        <Macro name="Cunversione SumatraPDF.APP.IA.ordinata-Tavula(.xlsx)" Ctrl="no" Alt="no" Shift="no" Key="0" FolderName="Cunversioni SumatraPDF">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per indettà solu e linee tradutte, dunque quelle chì cuntenenu u segnu | => | è chì sò state tradutte da l'IA" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="(.*) => (.*) \(by ai (.*) on (.*)\)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="784" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1615" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Cumanda nurmale per caccià tutte e linee senza indetta" />
            <Action type="2" message="0" wParam="43051" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per trasfurmà e linee tradutte, dunque quelle chì cuntenenu u segnu | => | è piazzà a data in prima culonna" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="(.*) => (.*) \(by ai (.*) on (.*)\)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\4\tai \3\t\1\t\2" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Cumanda nurmale per ordinà tutte e linee da a data, da a più recente à a più anziana" />
            <Action type="2" message="0" wParam="42060" lParam="0" sParam="" />
        </Macro>
        <Macro name="Cunversione SumatraPDF.APP.crono.ordinata-Tavula(.xlsx)" Ctrl="no" Alt="no" Shift="no" Key="0" FolderName="Cunversioni SumatraPDF">
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per indettà tutte e linee di cronolugia" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="(.*)\tco \t" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1702" wParam="0" lParam="784" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1615" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Cumanda nurmale per caccià tutte e linee senza indetta" />
            <Action type="2" message="0" wParam="43051" lParam="0" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Espressione regulare per trasfurmà e linee di cronololugia squassendu i spazii di fine d'ogni culonna" />
            <Action type="3" message="1700" wParam="0" lParam="0" sParam="" />
            <Action type="3" message="1601" wParam="0" lParam="0" sParam="(.*) \tco \t(.*) \t(.*) \t(.*)" />
            <Action type="3" message="1625" wParam="0" lParam="2" sParam="" />
            <Action type="3" message="1602" wParam="0" lParam="0" sParam="\1\tco\t\2\t\3\t\4" />
            <Action type="3" message="1702" wParam="0" lParam="768" sParam="" />
            <Action type="3" message="1701" wParam="0" lParam="1609" sParam="" />
            <Action type="0" message="2172" wParam="0" lParam="0" sParam="Cumanda nurmale per arritrusà tutte e linee" />
            <Action type="2" message="0" wParam="42083" lParam="0" sParam="" />
        </Macro>
```
- Tandu ste prucedure nove sò dispunibule in _Notepad++_.
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
