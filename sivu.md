# Kotitehtävät

## h1 Kybertappoketju

### Herrasmieshakkerit – Valkohattuhakkerit, vieraana Iiro Uusitalo (1.10.2019)

- Uutisoinnissa/tiedottaessa hyökkäyksistä tärkeää vastata ihmisten kysymykseen siitä, onko tämä ongelma minulle vai ei. Turha paniikki vie resursseja pois ja luo stressiä ihmisille. (tämä liittyen Simjacker -haavoittuvuudesta uutisointiin)

- F-Securen Honeypoteissa havaittu enemmän Linux- kuin Windows-haittaohjelmia ensimmäistä kertaa (huom. jakso julkaistu 1.10.2019). Kyse ei ole niinkään palvelinpuolen haittohjelmista, vaan IOT-laitteisiin kohdistetuista haittaohjelmista (tai pikemminkin IOT-laitteiden valmistajat eivät varaudu kyberturvaan riittävästi).

- Iiro Uusitalo, Linuxin/infran kanssa enemmän pyörinyt tietoturva-asiantuntija.

- Team Whack – Ylelle kuvattu sarja, joka on tehty mahdollisimman realistiseksi hakkerointikuvaukseksi oikeilla laitteilla ja oikeilla työkaluilla.

- Team Rot – valkohattuhakkeriryhmä, joka tekee erilaisia haasteita yms. Järjestivät Kuntahaasteen, jonka ideana oli suorittaa tekninen murtotestaus johonkin kuntaan. Suurin osa kunnista käyttää samoja käytäntöjä, joten yhdelle tehdystä testauksesta on sama hyöty useille muille. Testaukset olleet ilmaisia kohteille, sillä toiminta ollut vapaaehtoista. Aikaraja haasteeseen oli noin 30 tuntia per henkilö. Testauksen alueeseen kuului kaikki kunnan toiminnot. Haavoittuvuuksia löytyi yhdeksän, joista neljä oli täysin uusia.

- Kysymys kurinalaisuudesta kolahtaa, kuinka juuri voi optimoida omaa aikaa hakkeroinnin oppimiselle mahdollisimman laadukkaasti ja laajasti? Töissäkin pitää käydä ja tehdä muita opintoja, joten aikahaaste on valtava.

### Hutchins et al 2011: Intelligence-Driven Computer Network Defense Informed by Analysis of Adversary Campaigns and Intrusion Kill Chains, chapters Abstract, 3.2 Intrusion Kill Chain.
- APT:t (Advanced Persistent Threat) edustavat hyvin resursoituja ja koulutettuja vastustajia/hyökkääjiä, jotka suorittavat usean vuoden mittaisia murtokampanjoita. Kohteet ovat taloudellisia, omistusoikeudellisia tai kansallisen turvallisuuden informaatiota käsitteleviä.

- Tappoketjumallilla voi kuvata murtojen eri vaiheita ja kartoittaa vastustajan/hyökkääjän toimien indikaattoreita puolustaville toiminnoille sekä tunnistaa yksittäisten murtojen suurempiin kampanjoihin linkittäviä kuvioita. Mitä laajemmin kybertappoketju ymmärretään ja institutionalisoidaan niin sitä epätodennäköisemmäksi vastustajien/hyökkääjien onnistumiset käyvät.

- Tappoketjumalli on systemaattinen prosessi, joka kohdentuu hyökkääjään luodakseen halutun vaikutteen. Alunperin käytetty sotilaallisessa toiminnassa. Tietoverkkohyökkäyksissä ja -vakoilussa tappoketjuvaiheet ovat:

1. tiedustelu – tutkitaan, identifioidaan ja valitaan kohteet
2. aseellistaminen – yhdistetään etäyhteyden muodostava troijalainen johonkin exploitiin, jotta saadaan toimitettava kuorma
3. toimitus – välitetään ase kohdennettuun ympäristöön
4. hyödynnys – laukaistaan murtajan koodi
5. asennus – asennetaan takaovi uhrijärjestelmään jolloin voidaan pysyä ympäristössä
6. command and control (c2) – luodaan c2-kanava, jolla voidaan kontrolloida kohdeympäristöä
7. toimet kohteissa – edellä olevien askelien jälkeen murtautujat voivat tehdä haluamiaan toimia kohdeympäristöissä. Usein tämä on tietojen (datan) varastamista tai saatavuuden rikkomista. Vaihtoehtoisesti murtautujat saattavat halua vain pääsy-yhteyden kohdeympäristöön siirtyäkseen kohteen verkon muihin ymppäristöihin.

KKO 2003:36

- Tietomurto, jossa tekijä oli yrittänyt tunkeutua oikeudettomasti pankin tietojärjestelmään. Porttiskannaamalla oli yrittänyt löytää avoimia välityspalvelimia. Skannaus ei kuitenkaan läpäissyt palomuuria.

- Vaikka tekijän mukaan porttiskannauksella ei ollut tarkoitus murtautua pankin järjestelmiin vaan vain todeta auki olevat välityspalvelimet, ei oikeus tätä pitänyt uskottavana. Täten kyseessä oli tietojärjestelmään kohdistunut tietomurron yritys.

- Tärkeä muistaa, että herkästi voi tulla oikeudellisia seurauksia mikäli harjoittelee hakkerointia avoimissa ymäpristöissä. Hyvä siis tupla/tripla tsekata ettei harjoitteluympäristöt ole yhteydessä internetiin ettei käy kalpaten ja tule sakkotuomioita maksettavaksi.

### The Art of Hacking -videoita en saanut nyt pyörimään.

### Virtuaalikoneharjoitteet

Kalin asennus – asensin Kalin verkkosivuilta (https://www.kali.org/get-kali/#kali-platforms) suoraan valmiiksi rakennetun kuvan VirtualBoxiin. Muutin tähän vain RAMin määrän 4:ään gigaan käyttöönottaessa. Kaikki sujui niin kuin piti.

Koneen irrottaminen verkosta onnistui hyvin openvpn:llä ja sain testattua ettei internetiin saanut yhteyttä pingaamalla 8.8.8.8:aa sekä google.comia.
Sain tehtyä porttiskannauksen, mutta en osannut siitä edetä pidemmälle.
