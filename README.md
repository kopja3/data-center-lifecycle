# Itseopiskelumateriaali: Vihreä datakeskus ja energiatehokkuus

Tämä itseopiskelumateriaali tarjoaa johdannon vihreän datakeskuksen käsitteisiin, energian kulutukseen ja uudelleenkäyttöön sekä keskeisiin mittareihin (EN 50600-4 -standardi). Materiaali on suunnattu erityisesti abiturienteille ja perustuu aiemmin laadittuun oppaaseen "Vihreän datakeskuksen rakentaminen Suomessa".

---

## Johdanto

**Herätä kiinnostus**  
Tiesitkö, että jokainen netissä katsomasi video ja pilvitiedosto asuu fyysisesti datakeskuksessa? Ne kuluttavat sähköä ja tuottavat lämpöä. Mitä tapahtuu kulisseissa, kun käytämme digitaalisia palveluja?

**Mikä on datakeskus?**  
Datakeskus on suuri palvelintila, jossa säilytetään ja käsitellään dataa. Ne ovat internetin, pilvipalveluiden ja mobiilisovellusten selkäranka.

**Ympäristöhaaste**  
Datakeskukset kuluttavat n. 2–3 % maailman sähköstä, ja osuus kasvaa digitalisaation myötä. Tämä luo haasteita ilmastotavoitteille: sähkön tuotannon päästöt ja kuumenevien palvelinten jäähdytys.

### Havainnollistava kuva
Kuva esittää datakeskuksen sijaintia valtakunnallisessa sähköverkossa ja energian virtauksia.
[Katso datakeskuksen sijaintikaavio](assets/Datacenter_in_global_Finngrid_network.PNG)



**Vihreä datakeskus -käsite**  
Vihreä datakeskus on suunniteltu ja operoitu ympäristöä säästäen: energiatehokkaasti, uusiutuvilla energialähteillä ja hukkaenergiaa hyödyntäen.

**Materiaalin eteneminen**  
1. Vihreän datakeskuksen elementit ja periaatteet  
2. Energian kulutus ja uudelleenkäyttö  
3. EN 50600-4 -standardi ja mittarit  

---

## Osa 1: Vihreän datakeskuksen elementit ja periaatteet

**Tiivis teoriaosuus**  
- **Energiatehokkuus**: Jokainen wattitunti hyödynnettävä maksimaalisesti. Palvelinlaitteiden energiapihi valinta ja älykäs kapasiteetin hallinta.  
- **Tehokas jäähdytys**: Vapaajäähdytys ulkoilmalla, veden/meriveden käyttö, hyvä ilmanvaihto ja eristys.  
- **Uusiutuva energia**: Sähkö tuulipuistoista, aurinkopaneeleista tai muista uusiutuvista lähteistä.  
- **Hukkalämmön hyödyntäminen**: Lämmön talteenotto esim. kaukolämpöverkkoon.  
- **Kestävä suunnittelu ja elinkaari**: Sijainti, rakennusmateriaalit, kierrätys ja päivitykset.

**Visuaalinen tuki**  
Infografiikka, jossa energian virtaus: uusiutuva sähkö → palvelimet → lämpö kiertoon → minimihukka.

**Käytännön esimerkki**  
Google Haminan datakeskus: rakennettu vanhaan paperitehtaaseen, merivesijäähdytys, 100 % uusiutuvaa energiaa, PUE ~1,1.

**Jatkolukuvinkki**  
> Syvennä aihetta oppaasta *“Vihreän datakeskuksen rakentaminen Suomessa”*.

**Pohdintatehtävä**  
Mitkä vihreän datakeskuksen periaatteista ovat tärkeimpiä ja miksi?

---

## Osa 2: Energian kulutus ja uudelleenkäyttö datakeskuksessa

**Tiivis teoriaosuus**  
- Sähkönkulutus: IT-laitteet (palvelimet, levyt, verkkolaitteet), jäähdytys, UPS, valaistus.  
- PUE (Power Usage Effectiveness): vertaa kokonaiskulutusta IT-kulutukseen.  
- Kulutuksen vähentäminen: virtualisointi, lämpötilojen optimointi, tehokas ilmankierto.  
- Hukkalämmön talteenotto: lämpöpumput ja lämmönvaihtimet siirtävät lämmön uusiokäyttöön.  
- Haasteet: investoinnit, sijainti, tekniset rajoitteet.

**Visuaalinen tuki**  
Kaavio: perinteinen vs. hukkalämpöä hyödyntävä datakeskus.

**Käytännön esimerkki**  
Telia Helsinki Data Center: lämpö kaukolämpöverkkoon, tuhansien kotien lämmitykseen. Yandex Mäntsälässä ja LUMI Kajaanissa hyödyntävät myös.

**Jatkolukuvinkki**  
> Lue esim. Ylen uutinen “Datakeskusten hukkalämpöä on pian pakko hyötykäyttää” (7.6.2023).

**Pohdintatehtävä**  
Miksi kaikki datakeskukset eivät kierrätä hukkalämpöä? Esteet ja mahdollisuudet?

---

## Osa 3: EN 50600-4 -standardi ja kestävän datakeskuksen mittarit

**Tiivis teoriaosuus**  
- **EN 50600-4**: eurooppalainen standardisarja mittaa datakeskusten energiatehokkuutta ja kestävyyttä.  
- **PUE**: kokonaiskulutus / IT-kulutus.  
- **ERF (Energy Reuse Factor)**: kuinka suuri osa energiasta hyödynnetään uudelleen (0–1).  
- **Muut mittarit**: Renewable Energy Factor, CUE, WUE.

**Standardin merkitys**  
Standardi mahdollistaa vertailukelpoisuuden ja kannustaa jatkuvaan parantamiseen. EU-direktiivit edellyttävät läpinäkyvää raportointia.

**PUE ja ERF yhdessä**  
Pelkkä PUE ei riitä: ERF huomioi lämmön uudelleenkäytön.

**Visuaalinen tuki**  
Kaavio: PUE-vertailu (2,0 vs. 1,2) ja PUE+ERF-laskenta lämmön talteenoton kanssa/ilman.

**Käytännön esimerkki**  
LUMI Kajaanissa: ilman lämmön talteenottoa PUE ~1,04, talteenoton kanssa PUE ~1,24 mutta ERF merkittävästi korkeampi.

**Jatkolukuvinkki**  
> Tutustu Green Grid -materiaaleihin tai CENELECin standardiselityksiin.

**Pohdintatehtävä**  
Mitkä mittarit ovat sinulle tärkeimpiä datakeskuksen ympäristöystävällisyyden arvioinnissa?

---

## Yhteenveto

✅ Vihreän datakeskuksen elementit: energiatehokkuus, uusiutuva energia, hukkalämpö.  
✅ Energian kulutus ja uudelleenkäyttö: optimointi, esimerkit Suomesta.  
✅ EN 50600-4 -standardi: objektiivinen mittaristo kestävyyden arviointiin.

> **Innostava päätös:**  
> Digitaalinen maailma kasvaa – vihreät datakeskukset mahdollistavat kestävän kasvun!

**Mahdollisuus syventyä**  
> Lue lisää: *“Vihreän datakeskuksen rakentaminen Suomessa”* -opas.

**Lopputehtävä (vapaaehtoinen)**  
Kirjoita pohdinta: *Miten sinä selittäisit vihreän datakeskuksen idean ja merkityksen jollekin, joka ei ole koskaan kuullut siitä?*

---

**Hyviä opiskeluita ja uusia oivalluksia vihreän datakeskuksen maailmaan!**
