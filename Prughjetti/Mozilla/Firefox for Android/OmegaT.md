# Istruzzioni per impiegà _OmegaT_ per a traduzzione di _Firefox for Android_

Eccu l’istruzzioni per scaricà l’ultima versione di i schedarii di traduzzione in lingua inglese, appruntalli per un trattamentu cù l’appiecazione _OmegaT_, è rinfrescà a versione in lingua corsa.

## Scaricamentu di i schedarii di lingua inglese

À st’ora, schedarii, ci n’hè 30, tutti cù u listessu nome `strings.xml` è ognunu in u so sottucartulare. Ancu di grazia, ci hè una prucedura per scaricalli tutti di manera autumatica. Sta prucedura, chì impiega __Windows PowerShell__, si chjama `Schedarii in inglese.ps1`.

###  A prucedura autumatica

- Apre a prucedura per [scaricà tutti i schedarii in inglese](Schedarii%20in%20inglese.ps1)
- Cliccà nant’à u buttone `Raw`, insù è à dirittu, accant’à l’icone di u screnu, di a mina, è di a curbella
- Selezziunà tutte e linee cù a cumanda `Ctrl-A`
- Cupià tutte e linee cù a cumanda `Ctrl-C`
- Lancià _Windows PowerShell_ cù un cliccu dirittu nant’à u listinu « Démarrer »
- Rimpiazzià u cartulare attuale - cù a cumanda `CD u_mo_cartulare` - da quellu induve ci vole à piazzà i schedarii scaricati, per indettu : `CD C:\Traduzzione\OmegaT\Firefox_Android\source\`
- Incullà e linee cupiate cù a cumanda `Ctrl-V`
- Quandu tutte e cumande sò state passate, i schedarii d’origine in inglese si trovanu in u cartulare sceltu
- Chjode _Windows PowerShell_ cù a cumanda `exit`

###  A manera manuale

- Nant’à un navigatore Internet, andà à st’indirizzi :  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/browser/awesomebar/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/browser/engine-system/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/browser/errorpages/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/browser/menu2/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/browser/menu/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/browser/toolbar/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/addons/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/app-links/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/autofill/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/awesomebar/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/contextmenu/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/customtabs/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/downloads/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/findinpage/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/media/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/privatemode/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/prompts/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/pwa/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/qr/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/readerview/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/sitepermissions/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/tabs/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/feature/webnotifications/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/lib/crash/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/service/nimbus/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/support/base/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/support/ktx/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/support/migration/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/android-components/components/ui/tabcounter/src/main/res/values/strings.xml  
  https://github.com/mozilla-l10n/android-l10n/blob/master/mozilla-mobile/fenix/app/src/main/res/values/strings.xml  

- Per ogni schedariu, fà un __cliccu dirittu__ nant’à u buttone `Raw`, insù è à dirittu, accant’à l’icone di u screnu, di a mina, è di a curbella.

- Arregistrateli, unu dopu à l’altru, cù sti nomi :
```
  browser-awesomebar-strings-xml  
  browser-engine-system-strings-xml  
  browser-errorpages-strings-xml  
  browser-menu2-strings-xml  
  browser-menu-strings-xml  
  browser-toolbar-strings-xml  
  feature-addons-strings-xml  
  feature-app-links-strings-xml  
  feature-autofill-strings-xml  
  feature-awesomebar-strings-xml  
  feature-contextmenu-strings-xml  
  feature-customtabs-strings-xml  
  feature-downloads-strings-xml  
  feature-findinpage-strings-xml  
  feature-media-strings-xml  
  feature-privatemode-strings-xml  
  feature-prompts-strings-xml  
  feature-pwa-strings-xml  
  feature-qr-strings-xml  
  feature-readerview-strings-xml  
  feature-sitepermissions-strings-xml  
  feature-tabs-strings-xml  
  feature-webnotifications-strings-xml  
  lib-crash-strings-xml  
  service-nimbus-strings-xml  
  support-base-strings-xml  
  support-ktx-strings-xml  
  support-migration-strings-xml  
  ui-tabcounter-strings-xml  
  fenix-app-strings-xml  
```
## Preparazione di i schedarii nanzu a traduzzione

✔️ Ùn ci hè nisunu approntu à fà à i schedarii di lingua inglese.

## Copia di i schedarii di lingua inglese

- Cupià o dispiazzà stu schedariu in u cartulare `source` di u prughjettu _Firefox for Android_ in _OmegaT_.

## Ozzione o preferenze particulare à definisce in OmegaT

✔️ Nisuna.

## Traduzzione in lingua corsa

- Lancià l’appiecazione _OmegaT_ è apre stu prughjettu per traducelu.

## Preparazione di i schedarii nanzu a traduzzione

✔️ Ùn ci hè nisunu approntu à fà à i schedarii di lingua corsa.

## Incaricamentu di i schedarii di lingua corsa

Per ogni schedariu, ci vole à impiegà _Pontoon_ per impurtacci u schedariu traduttu in lingua corsa.
- Fà un cliccu nant’à a vostra icona d’utilizatore chì si trova insù è à dirittu, accant’à l’icona di a campana 🔔
- Sceglie a funzione _`Upload Translations`_ (ghjè una funzione riservata à u respunsevule di prughjettu)
- Selezziunà u schedariu di lingua corsa chì si trova in u cartulare `target` di u prughjettu _Firefox for Android_ in _OmegaT_
- À a fine di stu trattamentu, _Pontoon_ hè statu rinfrescatu cù a nova traduzzione.
