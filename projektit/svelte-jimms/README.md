# Tilapäinen kansio storybook:ssa käytettäville kuville

Svelte-tehtävien osalta storybook-palvelimen konfiguraatio on rikki,
eikä se osaa tällä hetkellä näyttää kuvia samasta `harjoitukset`-kansiosta,
jonne svelte-tehtävät tehdään.

Tilapäisesti svelte-tehtävissä tarvittavat kuvat voi sijoittaa tähän kansioon.

## Viittaaminen tähän kansioon sijoitettuihin kuvatiedostoihin

Esimerkiksi, jos tämä kansio sisältäisi `kuva.png`-kuvatiedoston, 
käytettäisiin sitä seuraavasti svelte-komponentista:

```svelte
<img src="kuva.png" />
```

## Build

Kun olet rakentamassa sivua, tämä polku ei välttämättä kuitenkaan toimi.

Voit tällöin joutua kopioimaan tämän kansion (`/harjoitukset-apu/src/harjoitukset`) sisällön `static`-kansion (`/harjoitukset-apu/static`) alle.

Tällöin myös kaikki resurssien käytöt pitää vaihtaa käyttämään `static`-polkua.
Tämä tapahtuukin edellisestä poiketen ilman `static`-kansion nimeä

Esim. yllä mainittu "kuva.png" löytyisi `static`-kansiosta suoraan sen nimellä:

```svelte
<img src="kuva.png" />
```

Toisin sanoen, kaikki static-kansiosta löytyvät asiat löytyvät suoraan static-kansion juuresta lähtevän polun avulla.

Esim. `kuva2.png`-kuva (löytyy kansiosta `/harjoitukset-apu/static/kuvat/kuva2.png`) löytyy `static`-kansiossa ollessaan sen kansiolla ja tiedostonimellä:

```svelte
<img src="kuvat/kuva2.png" />
```
