# Istruzzioni per impiegà _OmegaT_ per a traduzzione di _GeneWeb_

Per fà una traduzzione, l'appiecazione _OmegaT_ hà bisognu di schedarii di fonte cù una lingua sfarente di quella di destinazione. Di regula, a lingua di fonte hè l’inglese è quella di destinazione hè u corsu. D’altronde tutte e memorie di traduzzione pruviste nant’à stu situ sò in u sensu da l’inglese ver di u corsu.

Eccu l’istruzzioni per scaricà l’ultima versione di u schedariu di traduzzione è appruntallu per un trattamentu cù l’appiecazione _OmegaT_.

## Scaricamentu di u schedariu à traduce

- Si pò scaricà u schedariu di traduzzione chì cuntene __tutte e lingue__ da quì :  
  https://github.com/geneweb/geneweb/blob/master/hd/lang/lexicon.txt

## Preparazione di u schedariu nanzu a traduzzione

- Ci vole à trasfurmà u so cuntenutu per cunservà solu e catene in inglese qu’ellu ci vole à traduce.
- Seguitate l’[istruzzioni per l’adopru d’una prucedura](Cunversione.md) per fà sta trasfurmazione.

## Copia di i schedarii di lingua inglese

- Cupià o dispiazzà u schedariu trasfurmatu `omegat_lexicon.txt` in u cartulare `source` di u prughjettu __GeneWeb__ in _OmegaT_.

## Ozzione o preferenze particulare à definisce in OmegaT

- Lancià l’appiecazione _OmegaT_
- Sceglie `Ozzioni` eppò `Filtri di schedariu…`
  - Verificà l’ozzione di u furmatu `Testu` : 
          `Taglià u testu d’origine per fà paragrafi :`  
    - [x] `À ogni linea`

## Traduzzione in lingua corsa

- Lancià l’appiecazione _OmegaT_ è apre stu prughjettu per traducelu.

## Preparazione di u schedariu dopu a traduzzione

- À st’ora, a ricustruzione di u schedariu di traduzzione `lexicon.txt` hè un’operazione __manuale__

- Ma si pò quantunque appruntà u schedariu `omegat_lexicon.txt` grazia à _Notepad++_ per aghjunghje a catena `co: ` in capu d’ogni linea. Què si pò fà cù una cumanda di rimpiazzamentu impieghendu st’ozzioni :
  - Cosa à circà : `^`
  - Rimpiazzà cù : `co: \1`
  - Modu di ricerca : `Spressione regulare`
  - Cliccu nant’à u buttone `Rimpiazzalle tutte`

## Incaricamentu di u schedariu di traduzzione

- Quandu u schedariu `lexicon.txt` hè ricustruitu cù tutte e traduzzioni in lingua corsa, ci vole à creà una richiesta _Pull Request_ nant’à _GitHub_ per dumandà a so mudificazione in u dipositu.
