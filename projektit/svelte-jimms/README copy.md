# Kansio kuville ja muille resursseille

Lisää kuvat, fontit, ikonit ja muut resurssit tähän kansioon.

Tällöin niiden käyttö tapahtuu seuraavasti:

Esim. tästä kansiosta valmiiksi löytyvä `kuva.png`-kuva löytyy svelte-tiedostosta käytettäessä suoraan sen nimellä:

```svelte
<img src="kuva.png" />
```

Toisin sanoen, kaikki static-kansiosta löytyvät asiat löytyvät suoraan static-kansion juuresta lähtevän polun avulla.

Esim. `kuva2.png`-kuva (löytyy kansiosta `/harjoitukset-apu/static/kuvat/kuva2.png`) löytyy `static`-kansiossa ollessaan sen kansiolla ja tiedostonimellä:

```svelte
<img src="kuvat/kuva2.png" />
```
