# Promptid: andmebaasid

## Eesmärk

Selle näite eesmärk on näidata, et andmebaasi ülesannete puhul on kontekst hädavajalik. Kui mudelile ei anta andmebaasi skeemi, võib ta hakata ise oletama tabelite ja veergude nimesid ning koostada päringu, mis ei vasta tegelikule andmebaasile.

Andmebaasi ülesannetes peab prompt sisaldama piisavalt infot selle kohta, millised tabelid, veerud ja seosed on olemas ning milliseid piiranguid lahenduses järgida tuleb.

## Töös kasutatud esialgne prompt

```txt
Kirjuta päring, mis väljastaks klubide nimed, kelle liikmete hulgas on mängija(d), kes on mänginud täpselt ühe partii mustadega. Ei tohi kasutada vaatlust ja neid konstante, mida ülesandes pole.
```

## Töös kasutatud täiustatud prompt

```txt
Ole kogenud andmebaasi administraator.

Kontekst: Kasutan järgmist andmebaasi skeemi:
- Klubid(id, Nimi)
- Isikud(id, Klubi) - kus Klubi viitab Klubid(id)-le
- Partiid(id, must, valge) - kus must ja valge viitavad Isikud(id)-le

Ülesanne: Kirjuta SQL-päring, mis väljastab klubide nimed, kelle liikmete hulgas on mängija(d), kes on mänginud täpselt ühe partii mustadega.

Piirangud: Ära kasuta vaatlust (VIEW). Ära kasuta konstantidena väärtusi, mida ülesandes pole mainitud.

Formaat: Esita ainult SQL-päring koos lühikese (kuni 3 lauset) selgitusega.
```

## Katsetuse tulemus

Esialgne prompt sisaldas ülesande kirjeldust ja piirangut, kuid ei sisaldanud andmebaasi skeemi. Selle tulemusena tegid osa mudelitest ise oletusi tabelite ja veergude nimede kohta ning koostasid päringuid, mis ei olnud tegeliku andmebaasi jaoks kasutatavad.

Täiustatud prompt lisas andmebaasi skeemi, rolli, ülesande, piirangud ja soovitud väljundiformaadi. Selle tulemusena andsid mudelid funktsionaalselt korrektse lahenduse.

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

Andmebaasi ülesannetes on prompti kõige olulisem osa kontekst. Mudel ei saa koostada usaldusväärset päringut, kui tal puudub info tegeliku skeemi kohta. Seetõttu tuleks andmebaasi ülesannete puhul alati lisada tabelid, veerud, seosed ja piirangud.
