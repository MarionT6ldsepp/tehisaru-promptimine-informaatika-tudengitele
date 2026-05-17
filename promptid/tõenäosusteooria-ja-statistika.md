# Promptid: tõenäosusteooria ja matemaatiline statistika

## Eesmärk

Selle näite eesmärk on näidata, et matemaatika ülesannetes ei ole õppimise seisukohalt piisav ainult õige lõppvastus. Üliõpilane vajab ka lahenduskäiku, kasutatud valemeid ja põhjendusi, et oma arusaamist kontrollida.

Bakalaureusetöö katsetustes ilmnes, et matemaatika ülesande puhul võisid mudelid anda õige lõppvastuse ka lihtsale promptile. Erinevus avaldus eelkõige vastuse õpiväärtuses: põhjalikum prompt andis paremini jälgitava lahenduskäigu.

## Töös kasutatud esialgne prompt

```txt
Olgu X ~ U(-10,10). Leida tõenäosus P(k < X < k+4), kus -10 < k < k+4 < 10.
```

## Töös kasutatud täiustatud prompt

```txt
Ole matemaatika õppejõud, kes selgitab üliõpilasele lahenduskäiku.

Ülesanne: Olgu X ~ U(-10,10). Leida tõenäosus P(k < X < k+4), kus -10 < k < k+4 < 10.

Selgita lahendus samm-sammult järgmises järjekorras:

1. Defineeri jaotus ja kirjuta tihedusfunktsioon
2. Püstita integraal
3. Arvuta integraal
4. Esita lõplik vastus murruna ja kümnendmurruna

Ära jäta ühtegi vahesammu vahele.
```

## Katsetuse tulemus

Mõlema prompti puhul olid vastused faktiliselt õiged. Oluline erinevus ilmnes aga vastuse asjakohasuses, täielikkuses ja õppimisväärtuses.

Esialgse promptiga said mudelid küll õige vastuse, kuid lahenduskäik ei olnud alati struktureeritud viisil, mis toetaks üliõpilase arusaamist. Täiustatud promptiga esitasid kõik mudelid detailse lahenduskäigu koos põhjendustega, mida saab kasutada õppematerjalina.

## Lühem õppimiseks sobiv prompt

```txt
Lahenda järgmine ülesanne samm-sammult. Näita kasutatud valemit, olulisi vaheetappe ja lõppvastust nii murruna kui ka kümnendmurruna.

Ülesanne:
[lisa ülesande tekst]
```

## Üldine mall matemaatika ülesande jaoks

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

Matemaatika ülesannetes parandab prompti täpsustamine eelkõige vastuse õpiväärtust. Õige lõppvastus ei tähenda automaatselt, et vastus aitab õppida. Õppimiseks on oluline, et mudel näitaks ka lahenduskäiku, vaheetappe ja kasutatud valemeid.
