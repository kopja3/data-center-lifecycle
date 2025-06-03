# Itseopiskelumateriaali: Vihreä datakeskus ja energiatehokkuus

Tämä itseopiskelumateriaali tarjoaa johdannon vihreän datakeskuksen käsitteisiin, energian kulutukseen ja uudelleenkäyttöön sekä keskeisiin mittareihin (EN 50600-4 -standardi). Materiaali on suunnattu erityisesti IT-alan ammattilaisille, abiturienteille, IT-teknikoille ja perustuu oppaaseen "Vihreän datakeskuksen rakentaminen Suomessa".

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
Vihreä datakeskus on suunniteltu ja sen mekaaniset, sähköiset ja tietojärjestelmät on optimoitu yhdessä maksimaalisen energiatehokkuden ja vähäisen ympäristövaikutuksen saavuttamiseksi (Gowrin et al. 2005).

**Materiaalin eteneminen**  
1. Vihreän datakeskuksen elementit ja periaatteet  
2. Energian kulutus ja uudelleenkäyttö  
3. EN 50600-4 -standardi ja mittarit  

---
1. Konesalitilat ja rakenteet
   
Datakeskuksen palvelinsalit ovat lämpötilaltaan ja kosteudeltaan hallittuja tiloja, joissa laitteiden sijoittelu tukee tehokasta ilmankiertoa. Palvelinsaleissa käytetään kuuma-/kylmäkäytäväperiaatetta ja vahvistettua lattiarakennetta, jonka alla kulkee kaapelointi ja jäähdytysilmavirta. Keskuksen tukitiloissa on mm. sähkö- ja jäähdytyslaitteet sekä kaapelointioperaattoreiden tilat. Rakennus on palo-osastoitu ja varustettu kulkureiteillä huoltoa ja laajennuksia varten.
(Konesalitilojen huolellinen suunnittelu varmistaa, että IT-laitteisto toimii optimaalisissa olosuhteissa. Se luo pohjan muille järjestelmille, kuten sähkölle ja jäähdytykselle, jotka integroituvat rakenteisiin.)

2. Sähkönsyöttö ja varavoima
   
Datakeskuksessa on kaksi toisistaan riippumatonta sähkönsyöttöä (A- ja B-syötöt), jotka jaetaan erillisiin pää- ja jakokeskuksiin sekä laitteiden PDU-yksiköihin. UPS-järjestelmät turvaavat hetkellisen varavirtasyötön sähköhäiriöiden aikana. Pidempiä katkoksia varten käytetään varavoimageneraattoreita, jotka käynnistyvät automaattisesti. Kaikki järjestelmät on maadoitettu ja varustettu ylijännitesuojauksella. Hälytykset ja valvonta varmistavat, että poikkeamat huomataan nopeasti.
(Sähkönsyötön varmistusjärjestelmät takaavat, että palvelimet pysyvät käynnissä kaikissa tilanteissa. Kahdennetut syötöt, UPSit ja varavoima muodostavat ketjun, joka on yhtä vahva kuin sen vahvin lenkki – ja datakeskuksissa jokainen lenkki on suunniteltu kestämään. Seuraavaksi tarkastellaan, kuinka yhtä lailla kriittinen jäähdytys huolehtii siitä, että laitteet eivät ylikuumene.)

3. ICT-laitteet ja tietoliikenne

Palvelimet hoitavat laskentaa ja datankäsittelyä, tallennusjärjestelmät varmistavat datan saatavuuden ja verkkolaitteet (kytkimet, reitittimet) liittävät kokonaisuuden sisäisiin ja ulkoisiin yhteyksiin. Laitteet on sijoitettu räkkikaappeihin, ja sisäinen kaapelointi on selkeästi järjestetty. Tietoliikenneyhteydet on kahdennettu, ja verkkoinfrastruktuuria hallitaan DCIM-järjestelmillä ja muilla työkaluilla. Verkkoarkkitehtuuri mahdollistaa suuren kaistanleveyden ja matalan viiveen.
(ICT-laitteiden ja tietoliikenteen osuus takaa, että datakeskus pystyy suorittamaan varsinaisen tehtävänsä: datan tallennuksen, käsittelyn ja siirron luotettavasti. Jotta tämä on mahdollista ympäri vuorokauden, laitteiston on saatava keskeytyksettä virtaa ja riittävä jäähdytys, ja niiden toiminnasta on oltava jatkuva näkyvyys – nämä seikat käsitellään seuraavaksi.)

4. Jäähdytys- ja ilmastointijärjestelmät

Jäähdytysjärjestelmät ylläpitävät laitteiden toimintalämpötilan ja ilmankosteuden. Palvelinsalien ilmastointia hoitavat CRAC-/CRAH-yksiköt, jotka hyödyntävät kylmävesi- tai glykolijäähdytystä. Lämpö siirretään ulkoilmaan jäähdytystornien tai kuivasäteilijöiden avulla. Järjestelmät on kahdennettu ja suunniteltu energiatehokkaiksi. Hukkalämmön hyödyntäminen esimerkiksi kiinteistön lämmitykseen vähentää ympäristökuormaa.
(Jäähdytysjärjestelmät siis varmistavat, että IT-laitteet pysyvät viileinä ja toimintakykyisinä ympäri vuorokauden. Yhdessä sähkönsyötön kanssa ne muodostavat datakeskuksen “ylläpitoinfrastruktuurin”, joka huolehtii laitteiden perusedellytyksistä.)

6. Turvallisuus- ja valvontajärjestelmät

Fyysinen turvallisuus kattaa kulunvalvonnan, kameravalvonnan ja vahvistetut rakenteet. Paloturvallisuus perustuu varhaisiin ilmaisimiin ja kaasusammutusjärjestelmiin. Ympäristöolosuhteita ja sähkönsyöttöä seurataan jatkuvasti antureilla ja valvontajärjestelmillä. Keskitetty valvomo tai NOC huolehtii hälytyksiin reagoimisesta ympäri vuorokauden. Kaikki järjestelmät tukevat luotettavaa ja keskeytymätöntä toimintaa.
(Turvallisuus- ja valvontajärjestelmät varmistavat, että datakeskuksen toiminta ei keskeydy inhimillisten tai ympäristöllisten riskien takia. Fyysiset uhat, kuten tunkeutuminen tai tulipalo, pidetään hallinnassa, ja teknisten järjestelmien tilaa seurataan herkeämättä. Tämä monitasoinen turvaverkko täydentää datakeskuksen kokonaisuutta siten, että kaikki edellä kuvatut osa-alueet – tilat, laitteet, sähkö, jäähdytys ja turvallisuus – toimivat yhdessä luotettavasti.)

Yhteenveto
Nämä järjestelmät muodostavat datakeskuksen perustan ja toimivat yhdessä varmistaakseen 24/7-toiminnan. Seuraavaksi opiskelumateriaalissa syvennytään siihen, miten energiatehokkuus, vihreä lähestymistapa ja ympäristöystävälliset ratkaisut nivoutuvat datakeskuksen arkeen.


Sitaatit:
https://www.suomenhuoltovarmuusdata.fi/palvelukuvaukset
https://www.theseus.fi/bitstream/10024/793429/2/Svahn_Niklas.pdf
https://www.theseus.fi/bitstream/10024/793429/2/Svahn_Niklas.pdf
https://www.suomenhuoltovarmuusdata.fi/palvelukuvaukset
https://tnnet.fi/palvelut/konesalipalvelut/
https://tnnet.fi/palvelut/konesalipalvelut/







Gowrin (2005) mukaan vihreä datakeskus on datakeskus, jonka mekaaniset, sähköiset ja tietojärjestelmät on suunniteltu ja optimoitu yhdessä maksimaalisen energiatehokkuuden ja vähäisen ympäristövaikutuksen saavuttamiseksi.

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
