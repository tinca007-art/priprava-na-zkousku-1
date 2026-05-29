# Příprava na zkoušku

- Po naklonování repozitáře proveď `npm install`.
- Nezapomeň vždy před každým úkolem odkomentovat cestu k úkolu v souboru `vite.config.js`

## Úkol 1

Nastyluj odstavec `.box` tak, aby splňoval následující požadavky:

1. **CSS proměnná** – definuj CSS proměnnou `--color` a nastav ji na libovolnou barvu. Použij tuto proměnnou pro barvu textu odstavce.
2. **Textové vlastnosti** – nastav odstavci:
   - velikost písma na `14px`
   - řádkování na `1.6`
   - font na `Arial, sans-serif`
   - zarovnání textu na střed (`center`)
3. **Box** – nastav odstavci:
   - šířku `200px`
   - rámeček o tloušťce `2px`, plné čáry, barvu na hodnotu #ff8833, která nejprve ulož do CSS proměnné `--color`
   - vnitřní odsazení  `16px`
4. **Centrování** – odstavec musí být horizontálně i vertikálně vycentrovaný uprostřed stránky.

Všechny styly piš do souboru `scss/main.scss`.

## Úkol 2

Nastyluj dva divy `.box` pomocí Sass proměnných a CSS proměnných:

1. **Sass proměnné** – vytvoř dvě Sass proměnné:
   - `$main-color` s hodnotou `#0088ff`
   - `$dark-color` s hodnotou o 20 % tmavší než `$main-color`
3. **Pozadí divů** – nastav jednotlivým divům barvu pozadí pomocí proměnných:
   - `.box--primary` dostane barvu pozadí z proměnné `$main-color`
   - `.box--dark` dostane barvu pozadí z proměnné `$dark-color`
4. **Společné styly** – nastav oběma divům `.box`:
   - šířku `200px`, výšku `100px`
   - bílou barvu textu
   - zarovnání textu na střed, řádkování `100px` (pro vertikální vycentrování textu)

Všechny styly piš do souboru `scss/main.scss`.

## Úkol 3

Vytvoř Sass mixin `fancyTitle`, který nadpisu přidá dekorativní čárku pod text pomocí pseudoelementu `::after`.

1. **Mixin** – definuj mixin s názvem `fancyTitle`.
    Mixin pomocí pseudoelementu `::after` přidá k prvku, u kterého se použije (nadpis) čárku pod nadpisem.
    Čárka bude mít:
   - šířku `80px` a výšku `5px`
   - libovolnou barvu pozadí (`background-color`)
2. **Použití mixinu** – přilinkuj mixin (`@include fancyTitle`) na selektor `.title`

Všechny styly piš do souboru `scss/main.scss`.

## Úkol 4

Pomocí flexboxu vytvoř základní layout stránky se záhlavím, postranním panelem, obsahem a zápatím.

Výsledný layout by měl vypadat takto:

```
┌──────────────────────────┐
│          header          │
├────────┬─────────────────┤
│        │                 │
│sidebar │    content      │
│        │                 │
├────────┴─────────────────┤
│          footer          │
└──────────────────────────┘
```

**`.sidebar`** – pevná šířka `200px`, libovolná barva pozadí
**`.content`** – zaplní zbývající šířku vedle sidebaru, libovolná barva pozadí

Všechny styly piš do souboru `scss/main.scss`.

## Úkol 5

Vytvoř responzivní kartičku osoby. Na desktopu jsou foto a informace vedle sebe, na mobilu pod sebou.

```
Desktop (≥ 600px):          Mobil (< 600px):

┌───────┬──────────────┐    ┌──────────────────┐
│       │ Jana Nováková│    │                  │
│ foto  │ Front. Dev.  │    │      foto        │
│       │ +420 123 ... │    │                  │
└───────┴──────────────┘    ├──────────────────┤
                            │ Jana Nováková    │
                            │ Frontend Dev.    │
                            │ +420 123 456 789 │
                            └──────────────────┘
```

Obrázek na desktopu bude mít šířku 200px, na mobilu bude přes celou šířku stránky.
Použij přístup **mobile first**.

Všechny styly piš do souboru `scss/main.scss`.
