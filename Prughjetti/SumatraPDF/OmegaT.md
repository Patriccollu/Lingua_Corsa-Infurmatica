# Istruzzioni per impiegà _OmegaT_ per a traduzzione di _SumatraPDF_

- Per fà una traduzzione, l'appiecazione _OmegaT_ hà bisognu di schedarii di fonte cù una lingua sfarente di quella di destinazione. Di regula, a lingua di fonte hè l’inglese è quella di destinazione hè u corsu. D’altronde tutte e memorie di traduzzione pruviste nant’à stu situ sò in u sensu da l’inglese ver di u corsu.

- Per disgrazia, ùn si pò truvà un schedariu di traduzzione chì cuntene solu e catene in inglese di _SumatraPDF_.
  
- Eccu l’istruzzioni per scaricà l’ultima versione di e catene in inglese è custruisce un schedariu di traduzzione appruntatu per un trattamentu cù l’appiecazione _OmegaT_.

## Scaricamentu di e catene à traduce

- Ci hè dui lochi induve si pò truvà ste catene à traduce, mischiate cù d’altre infurmazioni :
  - nant’à una [pagina di u situ di traduzzione _apptranslator.org_](https://www.apptranslator.org/app/SumatraPDF/co)
  - nant’à un [schedariu di u situ di sviluppu _GitHub_](https://github.com/sumatrapdfreader/sumatrapdf/blob/master/src/docs/translations.txt)

## Preparazione di e catene nanzu a traduzzione

- Seguitate l’[istruzzioni per installà e prucedure di cunversione](Cunversione.md) chì seranu impiegate per identificà e catene in inglese.

### Da una pagina di u situ di traduzzione _apptranslator.org

- Andà à a pagina di u situ di traduzzione _apptranslator.org_ chì cuntene tutte e catene in inglese à traduce è e so traduzzioni in lingua corsa :  
  https://www.apptranslator.org/app/SumatraPDF/co
- Cupià tutte e linee di sta pagina, per indettu via a cumanda CTRL-A, per mettele in u preme’papei
- Lancià u prugramma _Notepad++_ è apre un schedariu novu, dunque viotu
- Incullacci tutte e linee di u preme’papei, per indettu via a cumanda CTRL-V
- Ci vole à trasfurmà u so cuntenutu per cunservà solu e catene in inglese qu’ellu ci vole à traduce.
- Sceglie `Macro`, eppò `Eseguisce una macro parechje volte…`
- Selezziunà `Cunversione SumatraPDF.APP-OmegaT` per cunservà tutte e catene in inglese o `Cunversione SumatraPDF.APPn-OmegaT` per cunservà solu e catene nove à traduce
- Cliccu nant’à `Eseguisce 1 volta`
- Appughjà nant’à u buttone `Eseguisce`
- Arregistrà u schedariu cù u nome `omegat_translations.txt`

### Da u schedariu unicu di u situ di sviluppu _GitHub_

- Scaricà l’ultima mudificazione di u schedariu `translations.txt` chì si trova nant’à u dipositu _GitHub_ :  
https://github.com/sumatrapdfreader/sumatrapdf/blob/master/src/docs/translations.txt
  - Fà un cliccu dirittu nant’à u buttone « _Raw_ » chì si trova à diritta, accant’à l’icone di u screnu, di a mina è di a curbella
  - Sceglie l’ozzione « _Arregistrà a sibula di a leia sottu…_ »
  - Arregistrà u schedariu cù u listessu nome
- Ci vole à trasfurmà u so cuntenutu per cunservà solu e catene in inglese qu’ellu ci vole à traduce.
- Lancià u prugramma _Notepad++_ è apre stu schedariu
- Sceglie `Macro`, eppò `Eseguisce una macro parechje volte…`
- Selezziunà `Cunversione SumatraPDF.TXT-OmegaT`
- Cliccu nant’à `Eseguisce 1 volta`
- Appughjà nant’à u buttone `Eseguisce`
- Arregistrà u schedariu cù u nome `omegat_translations.txt`

## Copia di i schedarii di lingua inglese

- Cupià o dispiazzà u schedariu trasfurmatu in u cartulare `\source\` di u prughjettu __SumatraPDF__ in _OmegaT_.

## Ozzione o preferenze particulare à definisce in OmegaT

- Lancià l’appiecazione _OmegaT_
- Sceglie `Ozzioni` eppò `Filtri di schedariu…`
  - Verificà l’ozzione di u furmatu `Testu` : 
          `Taglià u testu d’origine per fà paragrafi :`  
    - [x] `À ogni linea`

## Traduzzione in lingua corsa

- Lancià l’appiecazione _OmegaT_ è apre stu prughjettu per traducelu.

## Preparazione di u schedariu dopu a traduzzione

✔️ Ùn ci hè alcunu approntu à fà à u schedariu di lingua corsa.

## Incaricamentu di u schedariu di traduzzione

- Seguitate l’[istruzzioni per aghjunghje o mudificà e catene](Traduzzione.md#istruzzioni-per-pigli%C3%A0-in-contu-e-nove-catene-tradutte) nant’à u situ di traduzzione.
