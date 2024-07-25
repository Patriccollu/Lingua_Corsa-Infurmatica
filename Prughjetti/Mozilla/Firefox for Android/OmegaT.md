# Istruzzioni per impiegà _OmegaT_ per a traduzzione di _Firefox for Android_

Eccu l’istruzzioni per scaricà l’ultima versione di i schedarii di traduzzione in lingua inglese, appruntalli per un trattamentu cù l’appiecazione _OmegaT_, è rinfrescà a versione in lingua corsa.

## Scaricamentu di i schedarii di lingua inglese

À st’ora, schedarii, ci n’hè più chè 30, tutti cù u listessu nome `strings.xml` è ognunu in u so sottucartulare. Ancu di grazia, ci hè una prucedura per scaricalli tutti di manera autumatica. Sta prucedura, chì impiega __Windows PowerShell__, si chjama `Schedarii in inglese.ps1`.  

Per a vostra infurmazione, ci hè una prucedura simile per scaricà i schedarii in lingua corsa chì si chjama `Schedarii in corsu.ps1`.

###  A prucedura autumatica

- Apre a prucedura per [scaricà tutti i schedarii in inglese](Schedarii%20in%20inglese.ps1)
- Cliccà nant’à u buttone `Raw`, insù è à dirittu, accant’à l’icone di u screnu, di a mina, è di a curbella
- Selezziunà tutte e linee cù a cumanda `Ctrl-A`
- Cupià tutte e linee cù a cumanda `Ctrl-C`
- Lancià _Windows PowerShell_ cù un cliccu dirittu nant’à u listinu « Démarrer »
- Rimpiazzià u cartulare attuale - cù a cumanda `CD u_mo_cartulare` - da quellu induve ci vole à piazzà i schedarii scaricati, per indettu : `CD C:\Traduzzione\OmegaT\Firefox_Android\source\`
- Incullà e linee cupiate cù a cumanda `Ctrl-V`
- Appughjate nant’à u tastu `Entrée`
- Quandu tutte e cumande sò state passate, i schedarii d’origine in inglese si trovanu in u cartulare sceltu
- Chjode _Windows PowerShell_ cù a cumanda `exit`

###  A manera manuale

Ci hè parechji schedarii à traduce, è a lista cambia di quandu in quandu.

- Nant’à un navigatore Internet, andà à st’indirizzi :  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/browser/engine-system/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/browser/errorpages/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/browser/menu2/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/browser/menu/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/browser/toolbar2/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/browser/toolbar/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/compose/awesomebar/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/compose/browser-toolbar/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/compose/cfr/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/compose/tabstray/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/addons/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/app-links/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/autofill/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/awesomebar/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/contextmenu/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/customtabs/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/downloads/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/findinpage/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/fxsuggest/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/media/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/privatemode/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/prompts/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/pwa/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/qr/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/readerview/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/search/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/sitepermissions/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/tabs/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/webnotifications/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/lib/crash/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/service/nimbus/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/support/base/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/support/ktx/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/ui/tabcounter/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/ui/widgets/src/main/res/values/strings.xml/  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/fenix/app/src/main/res/values/strings.xml  
- Per ogni schedariu, fà un __cliccu dirittu__ nant’à u buttone `Raw`, insù è à dirittu, accant’à l’icone di u screnu, di a mina, è di a curbella

- Arregistrateli, unu dopu à l’altru, cù quelli nomi :
```
components-browser-engine-system-strings.xml
components-browser-errorpages-strings.xml
components-browser-menu2-strings.xml
components-browser-menu-strings.xml
components-browser-toolbar2-strings.xml
components-browser-toolbar-strings.xml
components-compose-awesomebar-strings.xml
components-compose-browser-toolbar-strings.xml
components-compose-cfr-strings.xml
components-compose-tabstray-strings.xml
components-feature-addons-strings.xml
components-feature-app-links-strings.xml
components-feature-autofill-strings.xml
components-feature-awesomebar-strings.xml
components-feature-contextmenu-strings.xml
components-feature-customtabs-strings.xml
components-feature-downloads-strings.xml
components-feature-findinpage-strings.xml
components-feature-fxsuggest-strings.xml
components-feature-media-strings.xml
components-feature-privatemode-strings.xml
components-feature-prompts-strings.xml
components-feature-pwa-strings.xml
components-feature-qr-strings.xml
components-feature-readerview-strings.xml
components-feature-search-strings.xml
components-feature-sitepermissions-strings.xml
components-feature-tabs-strings.xml
components-feature-webnotifications-strings.xml
components-lib-crash-strings.xml
components-service-nimbus-strings.xml
components-support-base-strings.xml
components-support-ktx-strings.xml
components-ui-tabcounter-strings.xml
components-ui-widgets-strings.xml
fenix-app-strings.xml
```
## Preparazione di i schedarii nanzu a traduzzione

✔️ Ùn ci hè nisunu approntu à fà à i schedarii di lingua inglese

## Copia di i schedarii di lingua inglese

- Cupià o dispiazzà stu schedariu in u cartulare `source` di u prughjettu _Firefox for Android_ in _OmegaT_

## Ozzione o preferenze particulare à definisce in OmegaT

- Lancià l’appiecazione _OmegaT_
- Sceglie `Ozzioni` eppò `Filtri di schedariu…`
  - Attivà u furmatu `Risorse Android`

## Traduzzione in lingua corsa

- Lancià l’appiecazione _OmegaT_ è apre stu prughjettu per traducelu.

## Preparazione di i schedarii dopu a traduzzione

✔️ Ùn ci hè nisunu approntu à fà à i schedarii di lingua corsa.

## Incaricamentu di i schedarii di lingua corsa

Per ogni schedariu, ci vole à impiegà _Pontoon_ per impurtacci u schedariu traduttu in lingua corsa.
- Fà un cliccu nant’à a vostra icona d’utilizatore chì si trova insù è à dirittu, accant’à l’icona di a campana 🔔
- Sceglie a funzione _`Upload Translations`_ (ghjè una funzione riservata à u respunsevule di prughjettu)
- Selezziunà u schedariu di lingua corsa chì si trova in u cartulare `target` di u prughjettu _Firefox for Android_ in _OmegaT_
- À a fine di stu trattamentu, _Pontoon_ hè statu rinfrescatu cù a nova traduzzione.
