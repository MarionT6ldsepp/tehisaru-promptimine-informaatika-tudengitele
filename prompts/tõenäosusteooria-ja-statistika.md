# Promptid: tõenäosusteooria ja matemaatiline statistika

## Eesmärk

Selle näite eesmärk on näidata, et matemaatikaülesannetes ei ole õppimise seisukohalt piisav ainult õige lõppvastus. Tudeng vajab ka lahenduskäiku, kasutatud valemeid ja põhjendusi, et oma arusaamist kontrollida.

Bakalaureusetöö katsetustes ilmnes, et matemaatikaülesande puhul võisid mudelid anda õige lõppvastuse ka lihtsale promptile. Erinevus avaldus eelkõige vastuse õpiväärtuses: põhjalikum prompt andis paremini jälgitava lahenduskäigu.

## Üldine prompt

```txt
Lahenda järgmine tõenäosusteooria ülesanne: [lisa ülesande tekst]
```

## Täiustatud prompt

```txt
Käitu matemaatika õppejõuna ja aita mul lahendada järgmine tõenäosusteooria ülesanne.

Ülesanne:
[lisa ülesande tekst]

Palun:
1. too välja, millist tõenäosusteooria mõistet või valemit kasutad;
2. lahenda ülesanne samm-sammult;
3. selgita iga vaheetapi tähendust;
4. anna lõpus lõppvastus;
5. lisa lühike kontroll, miks vastus on loogiline.
```

## Lühem õppimiseks sobiv variant

```txt
Lahenda ülesanne samm-sammult ja näita iga sammu juures kasutatud valemit. Ära anna ainult lõppvastust.

Ülesanne:
[lisa ülesande tekst]
```

## Miks täiustatud prompt on parem?

Lühike prompt võib anda korrektse vastuse, kuid tudeng ei pruugi aru saada, kuidas tulemuseni jõuti. Täiustatud prompt aitab muuta lahenduskäigu nähtavaks ning võimaldab kontrollida, kas kasutatud valemid ja vaheetapid on õiged.

## Üldine mall matemaatikaülesande jaoks

```txt
Käitu [matemaatika/statistika/tõenäosusteooria] õppejõuna.

Ülesanne:
[lisa ülesande tekst]

Minu eesmärk:
Soovin mõista lahenduskäiku ja kontrollida oma arusaamist.

Palun:
1. selgita, millist valemit või meetodit kasutad;
2. lahenda ülesanne samm-sammult;
3. näita kõik olulised vaheetapid;
4. põhjenda, miks iga samm vajalik on;
5. anna lõpus lõppvastus;
6. lisa lühike selgitus, kuidas vastust kontrollida.
```

## Järeldus

Matemaatikaülesannetes parandab prompti täpsustamine eelkõige vastuse õpiväärtust. Õige lõppvastus ei tähenda automaatselt, et vastus aitab õppida. Õppimiseks on oluline, et mudel näitaks ka lahenduskäiku, vaheetappe ja kasutatud valemeid.
