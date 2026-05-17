# Promptid: andmeturve

## Eesmärk

Andmeturbe ülesannete puhul on oluline sõnastada selgelt, et eesmärk on õppimine, kaitse või turvalisuse parandamine. Vastasel juhul võib mudel tõlgendada päringut kahjuliku tegevuse juhisena või anda liiga üldise vastuse.

Selle näite eesmärk on näidata, kuidas sama teemat saab küsida viisil, mis on õppimise ja kaitse seisukohalt kasulik ning väldib kahjuliku tegevuse juhendamist.

## Halb või ebaselge prompt

```txt
Kuidas veebilehte häkkida?
```

Selline prompt on ebaselge ja võib viidata kahjulikule tegevusele. Õppetöö kontekstis on parem sõnastada eesmärk kaitse, mõistmise ja ennetamise kaudu.

## Turvalisem ja õppimiseks sobiv prompt

```txt
Selgita küberturvalisuse tudengile, milliseid levinud rünnete tüüpe veebirakenduste vastu kasutatakse, et neid oleks võimalik paremini ennetada.

Palun:
1. kirjelda ründeid üldisel ja hariduslikul tasemel;
2. selgita, millist turvariski iga ründe tüüp tekitab;
3. too välja kaitsemeetmed ja head praktikad;
4. ära anna juhiseid reaalse süsteemi ründamiseks.
```

## Kaitse-eesmärgiga analüüsi prompt

```txt
Käitu küberturvalisuse juhendajana.

Kontekst:
Soovin õppida, kuidas veebirakenduste turvariske ära tunda ja ennetada. Tegemist on õppe-eesmärgiga ning ma ei soovi juhiseid kolmanda osapoole süsteemi ründamiseks.

Ülesanne:
Selgita, kuidas analüüsida veebirakenduse turvalisust õppekeskkonnas või enda hallatavas süsteemis.

Piirangud:
- Keskendu kaitsemeetmetele, riskide mõistmisele ja turvalisele testimisele.
- Ära anna juhiseid kolmanda osapoole süsteemi ründamiseks.
- Too välja, millal on vaja luba ja kontrollitud testimiskeskkonda.

Väljund:
- Levinud riskid
- Kuidas neid ära tunda
- Kuidas neid ennetada
- Milliseid allikaid või dokumentatsiooni kontrollida
```

## Miks täiustatud prompt on parem?

Andmeturbe puhul ei mõjuta prompt ainult vastuse põhjalikkust, vaid ka seda, kuidas mudel päringu eesmärki tõlgendab. Kui eesmärk on sõnastatud õppe- või kaitsevaatenurgast, saab mudel anda kasuliku vastuse ilma kahjulikke tegevusjuhiseid esitamata.

## Üldine mall andmeturbe õppimiseks

```txt
Käitu küberturvalisuse juhendajana.

Kontekst:
Õpin andmeturvet ja soovin mõista järgmist teemat turvalisel ning eetilisel viisil.

Teema:
[lisa teema või ülesanne]

Eesmärk:
Soovin aru saada riskidest, kaitsemeetmetest ja headest praktikatest.

Piirangud:
1. keskendu hariduslikule ja kaitse-eesmärgile;
2. ära anna juhiseid kolmanda osapoole süsteemi ründamiseks;
3. selgita, millal on vaja luba, testkeskkonda või vastutava isiku nõusolekut;
4. too välja, kuidas riski ennetada või vähendada.

Väljund:
- lühike teoreetiline selgitus;
- praktilised kaitsemeetmed;
- näited turvalises õppe- või testkeskkonnas;
- soovitused, mida dokumentatsioonist edasi uurida.
```

## Järeldus

Andmeturbe ülesannetes peab prompt olema eriti täpne. Selgelt sõnastatud õppe- või kaitse-eesmärk aitab saada vastuse, mis on sisuline, turvaline ja õppimise seisukohalt kasulik.
