# Promptid: andmebaasid

## Eesmärk

Selle näite eesmärk on näidata, et andmebaasi ülesannete puhul on kontekst hädavajalik. Kui mudelile ei anta andmebaasi skeemi, võib ta hakata ise oletama tabelite ja veergude nimesid ning koostada päringu, mis ei vasta tegelikule andmebaasile.

Andmebaasi ülesannetes peab prompt sisaldama piisavalt infot selle kohta, millised tabelid, veerud ja seosed on olemas ning milliseid piiranguid lahenduses järgida tuleb.

## Esialgne prompt

```txt
Kirjuta päring, mis väljastaks klubide nimed, kelle liikmete hulgas on mängija(d), kes on mänginud täpselt ühe partii mustadega. Ei tohi kasutada vaatlust ja neid konstante, mida ülesandes pole.
```

## Täiustatud prompt

```txt
Ole kogenud andmebaasi arendaja.

Kontekst: Kasutan järgmist andmebaasi skeemi:
- Klubid(id, Nimi)
- Isikud(id, Klubi) – kus Klubi viitab Klubid(id)-le
- Partiid(id, must, valge) – kus must ja valge viitavad Isikud(id)-le

Ülesanne:
Kirjuta SQL-päring, mis väljastab klubide nimed, kelle liikmete hulgas on mängija(d), kes on mänginud täpselt ühe partii mustadega.

Piirangud:
- Ära kasuta vaatlust ehk VIEW-d.
- Ära kasuta konstantidena väärtusi, mida ülesandes pole mainitud.
- Ära eelda tabeleid ega veerge, mida skeemis ei ole.

Väljund:
Esita SQL-päring ja lisa kuni kolme lause pikkune selgitus, miks päring töötab.
```

## Miks täiustatud prompt on parem?

Esialgne prompt sisaldab ülesande kirjeldust, kuid ei anna mudelile piisavalt infot andmebaasi struktuuri kohta. Selle tulemusena võib mudel teha oletusi tabelite või veergude nimede kohta. Täiustatud prompt lisab skeemi, piirangud ja väljundiformaadi, mistõttu on vastus tõenäolisemalt konkreetse ülesandega kooskõlas.

## Üldine mall andmebaasi ülesande jaoks

```txt
Ole kogenud andmebaasi arendaja.

Andmebaasi skeem:
[lisa tabelid, veerud ja seosed]

Ülesanne:
[lisa ülesande tekst]

Piirangud:
[lisa piirangud, näiteks keelatud konstruktsioonid, nõutud SQL-dialekt või vormistus]

Palun:
1. kirjuta SQL-päring;
2. ära eelda tabeleid ega veerge, mida skeemis ei ole;
3. järgi kõiki ülesandes antud piiranguid;
4. selgita lühidalt, miks päring töötab;
5. kui ülesandes on mitu võimalikku lahendust, eelista lihtsamat ja loetavamat varianti.
```

## Järeldus

Andmebaasi ülesannetes on prompti kõige olulisem osa kontekst. Mudel ei saa koostada usaldusväärset päringut, kui tal puudub info tegeliku skeemi kohta. Seetõttu tuleks andmebaasiülesannete puhul alati lisada tabelid, veerud, seosed ja piirangud.
