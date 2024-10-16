---
theme: seriph
background: https://source.unsplash.com/collection/94734566/1920x1080
class: 'text-center'
highlighter: shiki
lineNumbers: false
info: |
  ## Matomo-tilin auditointi
  Esitelmä Matomo-tilin auditointia varten Riihimäen kaupungille.
drawings:
  persist: false
css: unocss
---

# Matomo-tilin auditointi
## Riihimäen kaupunki

<div class="text-orange-500 text-2xl font-bold mb-4">
Verkkoanalytiikkastrategian kehittäminen
</div>

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-4 py-2 rounded cursor-pointer bg-white bg-opacity-10 hover:bg-opacity-20 transition duration-200 ease-in-out">
    Aloita esitys <carbon:arrow-right class="inline"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <a href="https://matomo.org" target="_blank" alt="Matomo Website"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:logo-github />
  </a>
</div>

<div class="abs-bl m-6 flex gap-2">
  <div class="text-sm opacity-50">
    Esittäjä: Juuso Jaakkola<br>
    Päivämäärä: 17.10.2024
  </div>
</div>

---
layout: two-cols
---

<!-- {id: esityslista} -->

# Esityslista

<div class="text-sm">

1. Johdanto Matomoon
2. Auditoinnin tavoitteet
3. Keskeiset painopistealueet
4. Menetelmät
5. Havainnot ja suositukset
6. Seuraavat vaiheet

</div>

::right::

<div class="pl-4 pt-10">
  <div class="w-full h-64 bg-blue-500 rounded-lg flex items-center justify-center text-white text-4xl font-bold">
    Analytiikka
  </div>
</div>

---
layout: image-right
image: 'https://source.unsplash.com/random/800x600'
---

# Johdanto Matomoon

<v-clicks>

- 🔓 Avoimen lähdekoodin verkkoanalytiikka-alusta
- 🛡️ Yksityisyyteen keskittyvä vaihtoehto Google Analyticsille
- 🖥️ Itse ylläpidetty tai pilvipalveluna tarjottu
- 🔧 Muokattava ja laajennettava

</v-clicks>

---

# Auditoinnin tavoitteet

<div class="grid grid-cols-2 gap-4">
  <div v-click class="bg-blue-500 text-white p-4 rounded-lg">
    <carbon-document-add class="text-3xl mb-2" />
    <div class="font-bold">Arvioida nykyinen Matomo-toteutus</div>
  </div>
  <div v-click class="bg-green-500 text-white p-4 rounded-lg">
    <carbon-search class="text-3xl mb-2" />
    <div class="font-bold">Tunnistaa puutteet seurannassa ja raportoinnissa</div>
  </div>
  <div v-click class="bg-yellow-500 text-white p-4 rounded-lg">
    <carbon-chart-average class="text-3xl mb-2" />
    <div class="font-bold">Arvioida tietojen tarkkuus ja luotettavuus</div>
  </div>
  <div v-click class="bg-red-500 text-white p-4 rounded-lg">
    <carbon-security class="text-3xl mb-2" />
    <div class="font-bold">Varmistaa yksityisyydensuojasäännösten noudattaminen</div>
  </div>
</div>

---

# Keskeiset painopistealueet

<div class="grid grid-cols-2 gap-4">
  <div v-click="1">
    <h3 class="text-orange-500"><carbon-settings class="inline-block" /> Seurannan asetukset</h3>
  </div>
  <div v-click="2">
    <h3 class="text-green-500"><carbon-chart-line class="inline-block" /> Tavoitteiden määrittely</h3>
  </div>
  <div v-click="3">
    <h3 class="text-blue-500"><carbon-shopping-cart class="inline-block" /> Verkkokaupan seuranta</h3>
  </div>
  <div v-click="4">
    <h3 class="text-purple-500"><carbon-cube class="inline-block" /> Mukautetut ulottuvuudet</h3>
  </div>
  <div v-click="5">
    <h3 class="text-red-500"><carbon-user-profile class="inline-block" /> Segmentointi</h3>
  </div>
  <div v-click="6">
    <h3 class="text-yellow-500"><carbon-report class="inline-block" /> Raporttien käyttö</h3>
  </div>
</div>

---

# Menetelmät

<v-clicks>

1. 🔍 Tilin tarkastelu ja asetusten analysointi
2. 🧪 Seurantakoodin tarkastus
3. 📊 Tietojen laadun arviointi
4. 👥 Käyttäjähaastattelut
5. 🏆 Vertailu parhaisiin käytäntöihin
6. ⚡ Suorituskykytestaus

</v-clicks>

---

# Havainnot: Seurannan asetukset

<div class="flex justify-center h-100">  

```mermaid {scale: 0.8}
graph TD
A[Seurantakoodi] --> B{Oikein toteutettu?}
B -->|Kyllä| C[Tarkka tiedonkeruu]
B -->|Ei| D[Tietojen eroavaisuudet]
D --> E[Suosittele korjauksia]
style A fill:#f9a825,stroke:#f57f17,stroke-width:2px
style B fill:#64b5f6,stroke:#1976d2,stroke-width:2px
style C fill:#81c784,stroke:#388e3c,stroke-width:2px
style D fill:#e57373,stroke:#d32f2f,stroke-width:2px
style E fill:#ffb74d,stroke:#f57c00,stroke-width:2px
```

</div>

---

# Havainnot: Tavoitteiden määrittely

<div class="grid grid-cols-2 gap-4">
<div>

## Nykytila
<v-clicks>

- 🎯 X tavoitetta määritelty
- 🌪️ Y konversiosuppiloa asetettu
- 📝 Z tapahtumaa seurataan

</v-clicks>
</div>
<div>

## Suositukset
<v-clicks>

- ➕ Lisää tavoitteita keskeisille käyttäjätoiminnoille
- 🔍 Tarkenna konversiosuppiloita
- 🔄 Toteuta tapahtumaseuranta vuorovaikutuksille

</v-clicks>
</div>
</div>

---
layout: image-right
image: '#2a2a2a'
---

# Suositukset

<v-clicks>

1. 🔄 Päivitä seurantakoodi kaikilla sivuilla
2. 🛒 Toteuta laajennettu verkkokaupan seuranta
3. 🧩 Aseta mukautetut ulottuvuudet käyttäjäominaisuuksille
4. 🎯 Luo segmenttejä kohdennettua analyysia varten
5. 📅 Määritä säännölliset automaattiset raportit
6. 🎓 Järjestä henkilöstölle koulutusta Matomon käytöstä

</v-clicks>

---

# Seuraavat vaiheet

<div class="grid grid-cols-5 gap-4 mt-8">
  <div v-click class="bg-blue-500 text-white p-4 rounded-lg text-center">
    <carbon-task class="text-3xl mb-2" />
    <div class="font-bold">Priorisoi suositukset</div>
  </div>
  <div v-click class="bg-green-500 text-white p-4 rounded-lg text-center">
    <carbon-calendar class="text-3xl mb-2" />
    <div class="font-bold">Luo toteutusaikataulu</div>
  </div>
  <div v-click class="bg-yellow-500 text-white p-4 rounded-lg text-center">
    <carbon-user-multiple class="text-3xl mb-2" />
    <div class="font-bold">Jaa vastuut</div>
  </div>
  <div v-click class="bg-red-500 text-white p-4 rounded-lg text-center">
    <carbon-time class="text-3xl mb-2" />
    <div class="font-bold">Aikatauluta seuranta-auditointi</div>
  </div>
  <div v-click class="bg-purple-500 text-white p-4 rounded-lg text-center">
    <carbon-loop class="text-3xl mb-2" />
    <div class="font-bold">Luo jatkuva seurantaprosessi</div>
  </div>
</div>

---
layout: center
class: text-center
---

# Kiitos

<div class="text-2xl text-orange-500 font-bold mb-4">
Kysymyksiä? Keskustellaan!
</div>

<div class="flex justify-center">
  <div class="w-64 h-64 bg-gradient-to-br from-orange-400 to-red-500 rounded-full flex items-center justify-center text-white text-4xl font-bold">
    Kiitos!
  </div>
</div>

---

# Ohjeita käyttäjälle

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-4 py-2 rounded cursor-pointer bg-white bg-opacity-10 hover:bg-opacity-20 transition duration-200 ease-in-out">
    Siirry diaan "Käyttäjien hallinta Matomossa" <carbon:arrow-right class="inline"/>
  </span>
  <span @click="$nav.go(15)" class="px-4 py-2 rounded cursor-pointer bg-white bg-opacity-10 hover:bg-opacity-20 transition duration-200 ease-in-out">
    Siirry diaan "Tagien hallinta Matomossa" <carbon:arrow-right class="inline"/>
  </span>
  <span @click="$nav.go(3)">/esityslista</span>
</div>

---

# Käyttäjien hallinta Matomossa

<div class="grid grid-cols-2 gap-4">
<div>
<v-clicks>

1. Lisää käyttäjä Matomoon:
   - Mene Matomon hallintapaneeliin
   <img src="./assets/matomo_1.png" alt="Matomo hallintapaneeli" width="200" />
   - Valitse vasemmalta "Käyttäjät"
   - Klikkaa "Lisää uusi käyttäjä"
   - Syötä käyttäjän sähköpostiosoite ja määritä salasana

</v-clicks>
</div>
<div>
<v-clicks>

2. Anna käyttöoikeudet tiettyyn sivustoon:
   - Etsi juuri luotu käyttäjä ja klikkaa "Muokkaa"
   - Käyttäjän profiilisivulla näet listan Matomossa olevista sivustoista
   - Valitse sivustokohtaisesti käyttöoikeus:
     - Näytä: Tarkastele raportteja ja dataa
     - Kirjoita: Tarkastele raportteja ja muokkaa asetuksia
     - Admin: Täydet hallintaoikeudet
     - Ei pääsyä: Ei näe mitään dataa

</v-clicks>
</div>
</div>

---

# Käyttöoikeuksien hallinta

<v-clicks>

- Rajoitettu pääsy tiettyihin osioihin:
  - Käytä Mukautettuja dimensioita, Segmenttejä tai Tavoitteita
  - Rajoita näytettävää dataa käyttäjän oikeuksien perusteella

- Varmistus ja ilmoitukset:
  - Käyttäjä näkee vain sallitut sivustot tai osiot
  - Lähetä ilmoitus sähköpostitse Matomon sisäänrakennetulla toiminnolla

</v-clicks>

---

# Tagien hallinta

<v-clicks>

1. Luo uusi tagi:
   - Mene Matomon hallintapaneeliin
   - Valitse vasemmalta "Tagit"
   - Klikkaa "Lisää uusi tagi"
   - Syötä tagin nimi ja kuvaus

</v-clicks>
---

# Tagien hallinta

<v-clicks>

2. Aseta tagi käyttäjän tai sivuston tagiin:
   - Etsi juuri luotu tagi ja klikkaa "Muokkaa"
   - Valitse sivustokohtaisesti tagin käyttäjä:
     - Näytä: Tarkastele raportteja ja dataa
     - Kirjoita: Tarkastele raportteja ja muokkaa asetuksia
     - Admin: Täydet hallintaoikeudet
     - Ei pääsyä: Ei näe mitään dataa

</v-clicks>

---

# Tagien hallinta

<v-clicks>

3. Luo uusi tagi:
   - Mene Matomon hallintapaneeliin
   - Valitse vasemmalta "Tagit"
   - Klikkaa "Lisää uusi tagi"
   - Syötä tagin nimi ja kuvaus

</v-clicks>
