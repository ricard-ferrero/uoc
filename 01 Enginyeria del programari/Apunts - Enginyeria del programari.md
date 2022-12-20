<link rel="stylesheet" href="style.css">

<h1 class="titol-assignatura"> Enginyeria del programari</h1>

<h1 class="titol-modul">Mòdul 1: Introducció a l'enginyeria del programari</h1>

# 1. Què és l'enginyeria del programari?

<div class="aclaracio">

**Enginyeria:** (_interpretació personal_) acció d'utilitzar els coneixements científics adequats per a conseguir solucionar problemes a trabés de la tecnologia.

>L'aplicació pràctica de la ciència i la tecnologia - [Viquipèdia](https://ca.wikipedia.org/wiki/Enginyeria)

>Art d'aplicar els coneixements científics a la invenció, al perfeccionament o a la utilització de les tècniques en totes llurs determinacions dins el camp industrial. - [Gran Enciclopèdia Catalana](https://www.enciclopedia.cat/gran-enciclopedia-catalana/enginyeria)

</div>

## 1.1. Programari i maquinari

**Programari:** La part intangible de qualsevol ordinador: tant les dades emmagatzemades com el conjunt d'accions a executar (_codi_).

>Conjunt dels programes de computació, procediments, regles, documentació i dades associades que formen part de les operacions d'un sistema de còmput - IEEE

**Maquinari:** La part física de l'ordinador (components electrònics) que permet l'execusió d'instruccions (càlculs) del _programari_.

## 1.2. El desenvolupament de programari

>**Desenvolupament de programari** l'acte de produir o crear programari.

**Codi màquina:** llista d'instruccions que l'ordinador pot entendre i executar directament. El codi màquina no és llegible per a les persones, i les instruccions són poques i molt senzilles com per a utilitzar-les per construir programes complexos d'una manera clara per a l'home.

**Llenguatge de programació:** eina que s'utilitzar per programar que permet escriure instruccions a un nivell d'abstracció més elevat, amb instruccions compostes i més complexes. Aquest desrpés es transforma en codi màquina per a ser exectutat.

>**Codi font:** la manera llegible en què s'escriu el programari

------------------------------------------------

L'objectiu del programari és cobrir unes necessitats en concret, ja siguin d'un client (o organització), un determinat grup d'usuaris o per a ús personal; pot ser venut o simplement oferit gratuïtament.

_Desenvolupament del programari_ és un concepte molt més ampli a simplement programar (creació de codi font), ja que també recull moltes altres activitats, com per exemple:
- estudi i documentació de les necessitats dels usuaris
- manteniment del programari
- coordinació del treball en equip
- redacció de manuals/ajudes a usuaris
- etc...

Com que la qualitat obtinguda i el cost del desenvolupament són importants, organitzacions i empreses han convertit aquestes activitats en una _enginyeria_.

## 1.3. L'àmbit de l'enginyeria del programari

Mentres abans el programari es construia per a fer càlculs matemàtics (_computadra_), avui en dia el és una eina extesa a tot arreu (xarxes socials, sistemes d'informació, rellotges de polsera...). Per tant existeixen diferents tipus de programari ergo diferents maneres de desenvolupar-lo.

**Classificació de Roger Pressman (2005):**
- Programari de sistemes
- Programari d'aplicació
- Programari científic i d'enginyeria
- Programari encastat
- Programari de línies de productes
- Aplicacions web
- Programari d'intel·ligència artificial

Les categories no són excloents i és habituall que s'hagi de desenvolupar programari que pertanyi a varies d'elles.

En aquesta assignatura ens centrarem només en una categoria: _programari d'aplicació desenvolupat a mida_, concretament:

>**Programari per a sistemes d'informació**: qualsevol combinació de tecnologia de la informació i activitats humanes que utilitzen aquesta tecnologia per a donar suport a l'operació, gestió o presa de decisions.

El programari per a sistemes d'informació gestiona certa informació mitjantçant una _base de dades_ i dóna suport a una sèrie d'activitats humanes dins del context d'un _sistema d'informació_.

<p class="aclaracio">
Un sistema d'informació no és un sistema informàtic. Aquest poden ser, per exemple, un conjunt d'albarans escrits a mà, o també pot estar format per un sistema informàtic de gestió de comandes.
</p>

## 1.4. Què és l'enginyeria del programari?

> **Enginyeria**: l'aplicació d'un enfocament sistemàtic, disciplinat i quantificable a les estructures, màquines, productes, sistemes o processos per a obtenir un resultat esperat - IEEE

> **Engiyeria del programari**: l'aplicació d'un enfocament sistemàtic, disciplinat i quantificable al desnvolupament, operació i manteniment del programari; és a dir, l'aplicació de l'enginyeria al programari - IEEE

**Desenvolupament**: procés que porta a la producció del programari.

**Operació**: execució del programari dins del seu entorn d'execució per tal de dur a terme la seva funció.

**Manteniment**: modificació del producte de programari per tal de corregir-ne els errors o bé adaptar-lo a noves necessitats.

En l'enginyeria del programari s'han de dur a terme totes aquestes activitats i així poder _mesurar, quantificar i analitzar_ els diferents processos relacionats amb la vida del producte de programari.

Això ens permet extreure conclusions aplicables a futurs projectes de programari. _Quins recursos són necessaris per un nou programari? Quant de temps caldria per afegir una nova funcionalitat? Quins riscos podem trobar?_

## 1.5. Història de l'enginyeria del programari

En l'inici del programari es feia com un producte gratuït inclòs en la compra del maquinari i fabricat pels mateixos fabricants del maquinari. No hi havia el concepte de _programari empaquetat_ com aproducte.

**No** hi havia planificació ni predicció de costos i temps. Però **sí** hi havia tècniques de reutilització (programació modular).

En el comitè científic de l'OTAN, octubre 1968, va definir formalment el terme _enginyeria del programari_.

-------------------------------------------------------

En la conferència de l'OTAN es va parlar de la _crisi del programari_: la dificultat d'escriure programari correcte, entenedor i verificable, i que tenia com a conseqüencia la dificultat de planificar els costos del projecte, els plaços de termini, problemes amb la qualitat, etc...

**Informe Chaos** (Standish Group, 1995) estudi sobre desenvolupament de programari a EUA, i exposava que:

- 90% de projectes no complien amb els requisits de temps, cost o qualitat
- 31% de projectes eren cancel·lats
- només 16% de projectes acabaven en el temps, pressupost i abast planificats

Durant dècades, es va intentar solucionar la crisi del programari inventant eines, tecnologies i pràctiques. No es va poguer solucionar de manera definitiva els problemes però sí algunes millores.

**"No Silver Bullet"** (Fred Brooks, 1986) és un article on s'explica que no hi ha una solució única (_perfecte, màgica_) per al problema, i per molt que s'investigui en tecnologia o gestió no es pot aconseguir gaires millores d'un ordre de magnitud en productivitat, fiabilitat o simplicitat, com a mínim en una dècada (a diferència del maquinari que es millora en dos ordres de magnitud cada dos anys).

La causa de les afirmacions de Brooks era que les millores que per aquell llavors s'estaven aconseguint podien pal·liar la complexitat accidental però no la complexitat essencial (la inherent al desenvolupament de programari).

Als 90' Internet va provocar un creixement molt ràpid en demanda de programari especialitzat (sobretot en la Web). Això va generar la necessitat de solucions de programari més simples, ràpides de desenvolupar i econòmiques.

L'informe Chaos de 2009 mostra la següent evolució en els projectes entre 1994 i 2009:

|             | 1994 | 2009 |
| ----------: | :--: | :--: |
| reixits     | 16%  | 32%  |
| cancel·lats | 31%  | 24%  |

Se segueix creient que no existeixen solucions màgiques i se segueixen buscant solucions. Algunes d'aquestes _que veurem en aquesta assignatura_ són:

- línies de producte
- desenvolupament guiat per models
- patrons o metodologies àgils de desenvolupament

