# Notino Frontend Assignment

## Description
Vytvoriť jednoduchý e-shop, ktorý bude pozostávať z 2 stránok:
- List produktov
- Košík


## Stránky
### List produktov
Zobrazí produkty na stránke vedľa seba, podobne ako je to na stránkach [Notino](https://www.notino.cz/parfemy/). Každý produkt má "Add to cart" button, 
ktorým sa môže sa produkt vloži do košíka (localStorage/sessionStorage).

**API**

Ako zdroj produktov slúži `https://raw.githubusercontent.com/MarianKmotorka/products-mock/main/data.json` 
> **Poznámka:** Dáta si nesťahujte do projektu, ale načítavajte si ich pomocou fetch/axios/... 

**Definícia API**
API vracia JSON objekt, ktorý obsahuje 3 rôzne typy produktov. Tieto produkty majú niektoré vlastnosti spoločné - id, title, description, price, rating, category, thumbnail.
Každá kategória má svoje špeciálne vlastnosti

**Kategorie**
- smarphones 
  - ram
  - storage
  - color
- fragrances
  - gender
  - volume
  - vegan
- home-decoration
  - width
  - height
  - depth

> **Upozornenie:** Pri výpise produktov zobrazte všetky atribúty daného produktu

### Košík
Zobrazí obsah košíku (localStorage, sessionStorage) pre aktuálneho použivateľa

#### Optional
- odstraniť produkt z košíku
- celkova suma produktov v košíku

### Product detail - Optional
Zobrazí detail produktu, neexistuje k tomu API, preto treba použiť rovnaké API ako pre list produktov.


## Kľúčové body
- Typescript
- Performance - memoizácia, ...
- Štruktúra kódu
- Štýlovanie (CSS) stačí minimálne - možnosť použiť hociaký CSS framework, library,...
