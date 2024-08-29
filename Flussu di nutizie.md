# Impiegà _Thunderbird_ per riceve un flussu di nutizie _Atom_ o _RSS_

## Cuncettu
- Parechji siti web - cum’è _GitHub_ o _GitLab_ - ingenereghjanu un flussu di nutizie `Atom` o `RSS` secondu a so attività
- _Thunderbird_ pò riceve un’infurmazione quand’un tale flussu hè creatu

## I siti web

### GitHub

Ci hè una funzione in _GitHub_ chì permette d’ingenerà un flussu di nutizie `Atom` secondu certe attività di _GitHub_.  

Per indettu, eccu i liami di certi flussi _Atom_ :  

```
https://github.com/:user.atom
https://github.com/:user/:repo/releases.atom
https://github.com/:user/:repo/tags.atom
https://github.com/:user/:repo/commits.atom
https://github.com/:user/:repo/commits/master/:path/:directory.atom
https://github.com/:user/:repo/commits/master/:path1/:path2/:file.atom
```
  
Ci vole à rimpiazzà `:user` da u nome d’utilizatore _GitHub_ è `:repo` da u nome di u dipositu. `:path1` è `:path2` sò un esempiu di dui chjassi, `:directory` hè un nome di sottucartulare è `:file` un nome di schedariu.

Per u nostru bisognu, avemu da impiegà l’utimu tipu d’indirizu chì permette di sapè quand’un schedariu hè mudificatu.

Eccu un esempiu reale : `https://github.com/Patriccollu/Lingua_Corsa-Infurmatica/commits/ceppu/README.md.atom`

### GitLab

Ci hè una funzione simile in _GitLab_ chì permette d’ingenerà un flussu di nutizie `Atom` secondu certe attività di _GitLab_.  

Per indettu, eccu i liami di certi flussi _Atom_ :  

```
https://gitlab.com/freepascal.org/lazarus/lazarus/-/commits/main/lcl/languages/lclstrconsts.pot?format=atom
https://framagit.org/fiat-tux/hat-softwares/lufi/-/commits/master/themes/default/lib/Lufi/I18N/lufi.pot?format=atom
https://code.videolan.org/videolan/vlc/-/commits/master/po/vlc.pot?format=atom
https://code.videolan.org/videolan/vlc/-/tags?format=atom
```
L’ultima linea insù permette di sapè quandu ci hè una versione nova.

### D’altri siti

Ma ci n’hè d’altri chì permettenu d’ingenerà un flussu di nutizie simile secondu certe attività.  

Per indettu, eccu i liami reale di certi flussi :  

```
https://filezilla-project.org/newsfeed.php
https://hg.mozilla.org/mozilla-central/rss-log
https://community.mp3tag.de/c/announcements.rss
https://sourceforge.net/projects/veracrypt/rss?path=/VeraCrypt%20Nightly%20Builds/Windows
https://www.apptranslator.org/rss?app=SumatraPDF&lang=co
```

## Thunderbird

Ci hè una funzione in _Thunderbird_ chì permette d’**abbunassi** à i flussi d’attualità `Atom` o `RSS` è dunque di riceve un avvertimentu in _Thunderbird_ quandu quellu flussu hè ingeneratu.

In corte parolle, ci vole à :
- Creà un contu di flussu
- Abbunassi à unu o parechji flussi (📗)
- Leghje i vostri flussi
  
Per sapene di più, seguitate l’[istruzzioni - in francese - per abbunassi à i flussi di nutizie](https://support.mozilla.org/fr/kb/comment-s-abonner-aux-flux-de-nouvelles-et-blogs) nant’à u situ web di l’assistenza di _Thunderbird_.  
Ci hè dinù a listessa infurmazione in lingua inglese : [_How to Subscribe to News Feeds and Blogs_](https://support.mozilla.org/en-US/kb/how-subscribe-news-feeds-and-blogs).
  
(📗) L’indirizzi di i liami à impiegà sò indicati in u paragrafu `I flussi di nutizie` di u schedariu `Traduzzione.md` di u prugramma currispundente.

Si pò rimpiazzà _Thunderbird_ da un altru prugramma di messaghjeria s’ella si pò abbunassi à i flussi d’attualità `Atom` o `RSS`.

#### Liami di navigazione nant’à stu situ
- [Rivene à a lista di tutti i sottucartulari di prughjettu](../../tree/ceppu/Prughjetti)
- [Rivene à a lista di tutti i prugrammi tradutti in lingua corsa](../../#readme)
