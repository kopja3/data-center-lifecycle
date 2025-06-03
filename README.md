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
   
Erilliset palvelinsalit: Datakeskus koostuu erillisistä konesalitiloista (”white space”), jotka on suunniteltu palvelinlaitteille. Tilat ovat kontrolloituja ympäristöjä, joissa lämpötila, ilmankosteus ja pölyisyys pidetään tarkasti hallinnassa 24/7.
Laiteräkit ja kaapit: Palvelimet ja muut ICT-laitteet asennetaan standardikokoisiin laiteräkkeihin (palvelinkaappeihin). Räkkeihin on järjestetty sekä virransyöttö että tietoliikennekaapelointi. Räkkejä sijoitetaan riveihin siten, että muodostetaan kuuma- ja kylmäkäytävät optimaalisen jäähdytyksen saavuttamiseksi.
Kaksinkertainen lattiarakenne: Monissa datakeskuksissa on korotettu lattia. Sen alla kulkee kaapelointi ja kylmä ilmavirta palvelinlaitteille. Korotettu lattia sekä vaihtoehtoisesti katon kautta kulkevat kaapelihyllyt varmistavat siistin kaapeloinnin ja helpottavat sekä jäähdytysilman jakelua että huoltotöitä.

(Konesalitilojen huolellinen suunnittelu varmistaa, että IT-laitteisto toimii optimaalisissa olosuhteissa. Se luo pohjan muille järjestelmille, kuten sähkölle ja jäähdytykselle, jotka integroituvat rakenteisiin.)

2. Sähkönsyöttö ja varavoima
   
Datakeskuksessa on kaksi toisistaan riippumatonta sähkönsyöttöä (A- ja B-syötöt), jotka jaetaan erillisiin pää- ja jakokeskuksiin sekä laitteiden PDU-yksiköihin. UPS-järjestelmät turvaavat hetkellisen varavirtasyötön sähköhäiriöiden aikana. Pidempiä katkoksia varten käytetään varavoimageneraattoreita, jotka käynnistyvät automaattisesti. 
Kaikki järjestelmät on maadoitettu ja varustettu ylijännitesuojauksella. Hälytykset ja valvonta varmistavat, että poikkeamat huomataan nopeasti.

Primäärinen sähkönsyöttö: Datakeskus on kytketty sähköverkkoon useilla syöttöyhteyksillä. Tyypillisesti käytössä on kaksi toisistaan riippumatonta syöttöä sähköverkosta, jotta verkkosähköä saadaan kahdesta suunnasta (A- ja B-syötöt). Tämä varmistaa, että vaikka toinen syöttö katkeaisi, toinen voi pitää laitteet toiminnassa.

Keskeytymätön virtalähde (UPS): UPS-laitteet (Uninterruptible Power Supply) tarjoavat akuston avulla hetkellisen varavirtalähteen, jos primäärisessä sähkössä tapahtuu häiriö. UPS tasoittaa jännitepiikkejä ja -katkoja ja antaa riittävästi aikaa käynnistää varavoimageneraattorit ilman, että palvelimet huomaavat katkosta.

Varavoimageneraattorit: Dieselgeneraattorit (tai muu varavoima, kuten kaasugeneraattorit) käynnistyvät automaattisesti laajemmassa sähkökatkossa. Ne pystyvät tuottamaan sähköä koko datakeskuksen kuormalle pitkiäkin aikoja, yleensä polttoainesäiliöiden ansiosta useiksi tunneiksi tai päiviksi. Generaattorit testataan säännöllisesti, jotta ne toimivat varmasti hätätilanteessa.

Sähkönjakelu ja redundanssi: Sähkö jaetaan datakeskuksessa varmistetusti. Jokaiselle räkkikaapille tuodaan yleensä kaksi erillistä syöttöä (yhdistettynä kahdentaviin PDU-virtajakoyksiköihin), jolloin yksittäisen sähkönjakelukomponentin vikaantuessa toinen syöttö jatkaa sähkönsyöttöä. Koko sähköjärjestelmä on suunniteltu N+1- tai 2N-periaatteella, eli siinä on ylimääräistä kapasiteettia tai rinnakkaiset järjestelmät jatkuvuuden takaamiseksi.


(Sähkönsyötön varmistusjärjestelmät takaavat, että palvelimet pysyvät käynnissä kaikissa tilanteissa. Kahdennetut syötöt, UPSit ja varavoima muodostavat ketjun, joka on yhtä vahva kuin sen vahvin lenkki – ja datakeskuksissa jokainen lenkki on suunniteltu kestämään. Seuraavaksi tarkastellaan, kuinka yhtä lailla kriittinen jäähdytys huolehtii siitä, että laitteet eivät ylikuumene.)

3. ICT-laitteet ja tietoliikenne

Palvelimet: Nämä ovat datakeskuksen tietojenkäsittelyn ydin. Palvelimet suorittavat laskentaa ja ajaa sovelluksia ympäri vuorokauden. Ne tuottavat lämpöä ja kuluttavat merkittävästi sähköä, joten niiden keskeytymätön toiminta vaatii tehokasta jäähdytystä ja luotettavaa sähkönsyöttöä.
Tallennusjärjestelmät: Datakeskuksessa on laajamittaisia tallennusratkaisuja (esim. levypohjaiset RAID-järjestelmät, SSD-kamppeet tai nauhakirjastot) datan säilyttämiseen. Nämä järjestelmät varmistavat, että tieto on saatavilla 24/7. Nekin sijaitsevat räkkiin asennettuina ja vaativat sekä sähköä että jäähdytystä.
Verkkolaitteet: Kytkimet, reitittimet ja muut verkkokomponentit liittävät palvelimet toisiinsa ja ulkomaailmaan. Ne muodostavat datakeskuksen sisäisen tietoverkon selkärangan. Verkkolaitteet huolehtivat dataliikenteestä keskeytyksettä, ja niiden redundanssi (esim. kahdentamalla kriittiset kytkimet) varmistaa, ettei yhden laitteen vika pysäytä yhteyksiä.

Ulkomaailman yhteydet: Datakeskuksen palvelut ovat hyödytöntä ilman luotettavia tietoliikenneyhteyksiä. Datakeskukset on kytketty internetiin ja mahdollisiin yksityisiin verkkoihin useiden operaattoreiden kautta. Yhteydet toteutetaan useilla fyysisillä reiteillä (esim. moninkertaiset valokuitukaapelit eri reittejä pitkin), jotta yhden reitin katkeaminen ei eristä datakeskusta.
Kahdennetut verkkoyhteydet: Yhteydet suunnitellaan kahdennetuiksi (redundant) ja varmennetuiksi. Käytössä voi olla esimerkiksi kaksi tai useampi erillinen reititin ja kytkinyhteys eri palveluntarjoajille, jotka jakavat verkkokuorman. Vikatilanteessa toinen yhteys jatkaa liikennöintiä automaattisesti. Tämä takaa, että data kulkee sisään ja ulos datakeskuksesta 24/7.
Sisäverkon kapasiteetti: Myös datakeskuksen sisäinen tietoverkko on suunniteltu korkealle kaistalle ja matalalle viiveelle, jotta valtavat datamäärät liikkuvat sujuvasti. Konesalin sisällä on nopeat runkoyhteydet palvelinriviä ja -kaappeja yhdistäville kytkimille. Verkon laitteissa on usein ylimääräisiä portteja ja linkkikapasiteettia, jotta kasvunvaraa ja vikasietoisuutta on riittävästi.

(ICT-laitteiden ja tietoliikenteen osuus takaa, että datakeskus pystyy suorittamaan varsinaisen tehtävänsä: datan tallennuksen, käsittelyn ja siirron luotettavasti. Jotta tämä on mahdollista ympäri vuorokauden, laitteiston on saatava keskeytyksettä virtaa ja riittävä jäähdytys, ja niiden toiminnasta on oltava jatkuva näkyvyys – nämä seikat käsitellään seuraavaksi.)


4. Jäähdytys- ja ilmastointijärjestelmät

Jäähdytysjärjestelmät ylläpitävät laitteiden toimintalämpötilan ja ilmankosteuden. Palvelinsalien ilmastointia hoitavat CRAC-/CRAH-yksiköt, jotka hyödyntävät kylmävesi- tai glykolijäähdytystä. Lämpö siirretään ulkoilmaan jäähdytystornien tai kuivasäteilijöiden avulla. Järjestelmät on kahdennettu ja suunniteltu energiatehokkaiksi. Hukkalämmön hyödyntäminen esimerkiksi kiinteistön lämmitykseen vähentää ympäristökuormaa.

Ilmastointi ja lämpötilanhallinta: Palvelinsalit on varustettu tehokkailla jäähdytys- ja ilmanvaihtojärjestelmillä, jotka ylläpitävät tasaista viileää lämpötilaa (tyypillisesti noin 18–27°C) ja sopivaa ilmankosteutta ympäri vuorokauden. Ilmastointijärjestelmät kierrättävät ilmaa jatkuvasti suodattaen pölyä ja tuoden raitista ilmaa tarvittaessa.

CRAC- ja CRAH-yksiköt: (Computer Room Air Conditioning / Air Handling) Palvelinsaleissa käytetään erillisiä jäähdytysyksiköitä, jotka viilentävät ilmaa. CRAC-yksiköt hyödyntävät kylmäaine- tai jäähdytysnestekiertoa poistaakseen lämpöä, ja CRAH-yksiköt puolestaan käyttävät rakennuksen jäähdytettyä vettä lämmön siirtämiseen. Nämä laitteet sijoitetaan usein palvelinsalin reunoille tai rivien väleihin ja puhaltavat kylmän ilman palvelinlaitteiden ottoaukkoihin.

Kylmä vesi ja jäähdytystornit: Datakeskuksen jäähdytysjärjestelmässä voi olla keskitetty jäähdytyskoneikko (chiller), joka tuottaa kylmää vettä. Kylmä vesi kiertää palvelinsalien ilmajäähdyttimille, ja lämpö siirretään ulkona sijaitseviin jäähdytystorneihin tai kuivasäteilijöihin, jotka luovuttavat lämmön ulkoilmaan. Järjestelmässä on usein useita rinnakkaisia chiller-yksiköitä ja pumppuja, jotta yhden vikaantuessa muut jatkavat jäähdytystä (N+1-redundanssi).

Kuuma- ja kylmäkäytäväjärjestely: Laiteräkit on yleensä aseteltu siten, että muodostuu erilliset kylmäkäytävät (räkkirivien edustat, joihin kylmä ilma johdetaan) ja kuumakäytävät (räkkirivien taustat, joista lämmin poistoilma kerätään). Tällä rakenteellisella ratkaisulla estetään kuuman ja kylmän ilman sekoittuminen ja tehostetaan jäähdytystä. Kuumakäytävät voidaan jopa kapseloida ja kuuma ilma ohjata suoraan jäähdytysjärjestelmään, jolloin jäähdytys toimii energiatehokkaammin.

Kosteudenhallinta: Jäähdytysjärjestelmä sisältää myös ilmankosteuden säätelyn. Liian kuiva ilma lisää staattisen sähkön riskiä ja liian kostea voi aiheuttaa laitteisiin kondensaatiota. Ilmankostuttimet tai kuivaimet varmistavat, että ilmankosteus pysyy suositellulla tasolla (esim. 40–60 %) jatkuvasti.

(Jäähdytysjärjestelmät siis varmistavat, että IT-laitteet pysyvät viileinä ja toimintakykyisinä ympäri vuorokauden. Yhdessä sähkönsyötön kanssa ne muodostavat datakeskuksen “ylläpitoinfrastruktuurin”, joka huolehtii laitteiden perusedellytyksistä.)

6. Turvallisuus- ja valvontajärjestelmät

Fyysinen turvallisuus kattaa kulunvalvonnan, kameravalvonnan ja vahvistetut rakenteet. Paloturvallisuus perustuu varhaisiin ilmaisimiin ja kaasusammutusjärjestelmiin. Ympäristöolosuhteita ja sähkönsyöttöä seurataan jatkuvasti antureilla ja valvontajärjestelmillä. Keskitetty valvomo tai NOC huolehtii hälytyksiin reagoimisesta ympäri vuorokauden. Kaikki järjestelmät tukevat luotettavaa ja keskeytymätöntä toimintaa.

Kulunvalvonta: Datakeskuksen fyysinen turvallisuus on kriittistä, jotta luvattomat henkilöt eivät pääse laitteisiin käsiksi. Kulunvalvontajärjestelmä valvoo kaikkia ovia ja alueita – datakeskukseen pääsy vaatii henkilökohtaisen tunnisteen (kuten kulkukortin, PIN-koodin tai biometrisen tunnisteen). Järjestelmä tallentaa käyntilokit, ja käyttöoikeudet on rajattu vain välttämättömille henkilöille ja alueille.

Videovalvonta: Kamerajärjestelmät seuraavat datakeskuksen tiloja ympäri vuorokauden. Valvontakamerat kattavat sisäänkäynnit, käytävät, laitetilat ja kriittiset kohdat. Kuvamateriaali tallennetaan ja sitä valvotaan aktiivisesti tai analysoidaan tarvittaessa jälkikäteen, mikä lisää turvallisuutta ja toimii pelotteena luvattomalle toiminnalle.

Murto- ja ympäristöhälyttimet: Datakeskuksessa on murtohälytysjärjestelmä, joka reagoi esimerkiksi oven pakottamiseen, lasin rikkoutumiseen tai liikkeeseen kielletyllä alueella. Lisäksi turvajärjestelmiin kuuluu ympäristöhälyttimiä, kuten tunnistimet tulvimisen tai savun havaitsemiseen. Hälytykset on kytketty vartiointiin tai päivystyskeskukseen, joka reagoi viipymättä.

Fyysisen rakenteen turvallisuus: Itse rakennus on suunniteltu kestämään ulkoisia uhkia. Datakeskuksen seinät, ovet ja lattiat ovat usein vahvistettuja ja paloturvallisia. Monesti laitetilat sijaitsevat rakennuksen sisäosissa ilman ulkoseiniä, mikä lisää suojaa. Myös varajäähdytys ja varavirtalaitteet on suojattu erillisissä tiloissa, jotta sabotaasi tai onnettomuus ei lamauta kriittisiä järjestelmiä.
Paloturvajärjestelmät

Palonilmaisimet: Datakeskuksessa käytetään herkästi ja nopeasti reagoivia palonilmaisujärjestelmiä. Tyypillisesti asennetaan sekä perinteisiä savuilmaisimia että aktiivisia järjestelmiä, kuten ilmansamplausilmaisimet (VESDA), jotka imuroivat jatkuvasti ilmaa ja havaitsevat savuhiukkaset jo ennen näkyvää savua. Varhaisen varoituksen avulla ehditään reagoida ennen kuin palo pääsee valloilleen.

Automaattiset sammutusjärjestelmät: Palon sattuessa datakeskuksessa on automaattinen sammutusjärjestelmä. Yleisiä ratkaisuja ovat kaasusammutusjärjestelmät, jotka vapauttavat inerttiä kaasua (esim. argon-, typpi- tai hiilidioksidipohjaisia seoksia) tulipaloalueelle. Kaasu tukahduttaa palon poistamalla hapen tai viilentämällä palotilaa aiheuttamatta laitevaurioita vedestä. Joissain tapauksissa on myös vesisprinklerit tai sumusammutus, yleensä esitoiminnalliset sprinklerit, jotka aktivoituvat vasta, kun lämpötila nousee tarpeeksi korkeaksi – tämä estää turhat vedenvahingot.

Palosegmentointi: Rakennus ja palvelinsalit on jaettu paloalueisiin, jotta mahdollinen tulipalo rajoittuu pieneen osaan eikä leviä koko datakeskukseen. Paloseinät, -ovet ja -läpiviennit on toteutettu standardien mukaan (esim. 60 min tai 120 min paloeristys). Tämä antaa myös sammutusjärjestelmille ja pelastushenkilökunnalle aikaa reagoida ennen kuin kriittiset laitteet vaarantuvat laajemmin.

Savunpoisto ja hätäilmanvaihto: Jos paloa syntyy, datakeskuksessa voi olla savunpoistojärjestelmä tai hätäilmanvaihto, joka käynnistyy poistaen savukaasuja tiloista. Näin turvataan ihmisten poistuminen ja laitteiden vahingot jäävät pienemmiksi. Savunpoisto toimii yhdessä paloilmaisimien ja sammutusjärjestelmien kanssa automaattisesti.

Ympäristövalvonta: Kaikkia kriittisiä olosuhteita seurataan jatkuvasti. Anturit mittaavat lämpötilaa, ilmankosteutta, ilman virtausta, ilmanpaine-eroja (esim. kylmä- ja kuumakäytävien välillä) sekä havaitsevat mahdolliset vesivuodot tai muut ympäristömuutokset. Nämä sensorit kytkeytyvät automaatiojärjestelmään, joka hälyttää heti, jos arvot poikkeavat sallituista rajoista.

Infrastruktuurin hallinta (DCIM): Datakeskuksissa käytetään usein keskitettyjä hallintajärjestelmiä, kuten DCIM (Data Center Infrastructure Management) tai rakennusautomaatiojärjestelmiä. Niiden avulla operoidaan sähkö-, jäähdytys- ja turvajärjestelmiä yhtenäisesti. Käyttöliittymästä voidaan nähdä laitteiden tilat, energiankulutus, lämpötila- ja kosteusjakaumat sekä mahdolliset hälytykset reaaliajassa.

Laitteiden ja verkon monitorointi: Myös itse ICT-laitteiden toiminta on valvonnassa. Palvelimien, tallennuslaitteiden ja verkkokomponenttien kuntoa ja suorituskykyä seurataan (esim. palvelinten prosessorikuorma, muistin käyttö, verkkoliikenteen määrät). Monitorointiohjelmistot hälyttävät, jos jokin laite kaatuu, kuormittuu liikaa tai jos yhteyksissä on ongelmia. Näin ylläpitohenkilöstö voi puuttua ongelmiin ennen kuin ne aiheuttavat käyttökatkoa.

Hälytykset ja reagointi: Kaikki valvontajärjestelmien keräämät hälytykset kootaan hälytysjärjestelmään, joka voi ilmoittaa päivystäville teknikoille tekstiviestillä, sähköpostilla tai muulla tavalla. Monissa datakeskuksissa on 24/7 miehitys tai vähintään päivystysrinki, joka reagoi hälytyksiin välittömästi. Nopea reagointi yhdistettynä automaattisiin varajärjestelmiin varmistaa, että pienetkin viat tai poikkeamat korjataan ennen kuin ne eskaloituvat vakaviksi ongelmiksi.

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
