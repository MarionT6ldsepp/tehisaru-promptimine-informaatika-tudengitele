# Promptid: algoritmid ja andmestruktuurid

## Eesmärk

Selle näite eesmärk on näidata, et lihtsa ja konkreetse küsimuse puhul ei pruugi pikk prompt olla vajalik. Samas võib vastuse liigse lühendamise korral väheneda vastuse kontrollitavus.

Algoritmide ja andmestruktuuride ülesannetes on õppimise seisukohalt oluline näha lisaks vastusele ka põhjendust: millist omadust, algoritmi või meetodit kasutati ning miks see konkreetse ülesande puhul sobib.

## Töös kasutatud esialgne prompt

```txt
Milline on vähim toespuude arv, mis saab olla sidusal graafil, kus on 10 tippu ja 10 serva?
```

## Töös kasutatud täiustatud prompt

```txt
Milline on vähim toespuude arv, mis saab olla sidusal graafil, kus on 10 tippu ja 10 serva? Anna ainult vastus.
```

## Katsetuse tulemus

Esialgse prompti korral vastasid kolm mudelit neljast õigesti. Vastused olid aga sageli pikemad, kui ülesande eesmärk nõudis.

Täiustatud prompt vähendas vastuse mahtu, kuid muutis lahenduse kontrollimise keerulisemaks. Kui mudelilt küsida ainult lõppvastust, ei ole kasutajal võimalik näha, millisele seosele mudel vastuse tugines. Seetõttu võib vale vastus jääda kergemini märkamata.

## Õppimiseks sobivam prompt

```txt
Lahenda järgmine graafiteooria ülesanne.

Ülesanne: Milline on vähim toespuude arv, mis saab olla sidusal graafil, kus on 10 tippu ja 10 serva?

Palun:
1. selgita lühidalt, millist graafi omadust kasutad;
2. näita lahenduskäiku;
3. anna lõpus konkreetne vastus;
4. hoia vastus võimalikult lühike, kuid kontrollitav.
```

## Üldine mall algoritmide ja andmestruktuuride ülesande jaoks

```txt
Käitu informaatika õppejõuna.

Ülesanne:
[lisa ülesande tekst]

Minu eesmärk:
Soovin aru saada, kuidas ülesanne lahendatakse, mitte ainult lõppvastust saada.

Palun:
1. nimeta kasutatav mõiste, algoritm või omadus;
2. selgita lahenduskäiku samm-sammult;
3. põhjenda, miks valitud meetod sobib;
4. anna lõpus konkreetne vastus;
5. hoia vastus võimalikult lühike, kuid kontrollitav.
```

## Järeldus

Algoritmide ja andmestruktuuride puhul on hea prompt selline, mis tasakaalustab lühiduse ja kontrollitavuse. Ainult lõppvastust tasub küsida siis, kui kasutaja oskab tulemust ise kontrollida. Õppimise eesmärgil on parem paluda mudelil lisada vähemalt lühike põhjendus.
