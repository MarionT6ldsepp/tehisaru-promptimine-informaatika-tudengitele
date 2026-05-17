# Promptid: algoritmid ja andmestruktuurid

## Eesmärk

Selle näite eesmärk on näidata, et vastuse mahu piiramine võib olla kasulik, kuid ainult juhul, kui kasutaja oskab vastust ise kontrollida. Kui küsida mudelilt ainult lõppvastust, võib vale või puudulik lahendus jääda märkamata.

Algoritmide ja andmestruktuuride ülesannetes on õppimise seisukohalt oluline näha lisaks vastusele ka põhjendust: millist omadust, algoritmi või meetodit kasutati ning miks see konkreetse ülesande puhul sobib.

## Esialgne prompt

```txt
Milline on vähim toespuude arv, mis saab olla sidusal graafil, kus on 10 tippu ja 10 serva?
```

## Täiustatud prompt: kiire vastus

```txt
Milline on vähim toespuude arv, mis saab olla sidusal graafil, kus on 10 tippu ja 10 serva? Anna ainult vastus.
```

## Täiustatud prompt: õppimiseks sobivam variant

```txt
Lahenda järgmine graafiteooria ülesanne.

Ülesanne: Milline on vähim toespuude arv, mis saab olla sidusal graafil, kus on 10 tippu ja 10 serva?

Palun:
1. selgita lühidalt, millist graafi omadust kasutad;
2. näita lahenduskäiku;
3. anna lõpus konkreetne vastus;
4. hoia vastus võimalikult lühike, kuid kontrollitav.
```

## Miks täiustatud prompt on parem?

Esialgne prompt võib anda küll õige vastuse, kuid õppimise seisukohalt ei pruugi sellest piisata. Täiustatud prompt suunab mudelit esitama lühikese lahenduskäigu, mille põhjal saab tudeng kontrollida, kas vastuseni jõuti õigel viisil.

## Üldine mall algoritmi ülesande jaoks

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
