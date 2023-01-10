<link rel="stylesheet" href="style.css">

<header>
    <p class="capçal">Apunts</p>
    <h1 class="titol-assignatura">Enginyeria del programari</h1>
</header>

<div style="font-size: 0.8rem">

Tot el contingut són apunts i resums del Grau universitari "Enginyeria Informàtica" cursat en la Universitat Oberta de Catalunya.

Per lo tant, els textos són extractes de la documentació que ofereix la universitat en les assignatures respectives i estan complementats amb documents d'altres pàgines webs informatives, d'altres llibres o amb conclusions personals.

</div>

# Índex

- [Mòdul 1: Introducció a l'enginyeria del programari](#modul-1)
    1. [Què és l’enginyeria del programari?](#1-qu%C3%A8-%C3%A9s-lenginyeria-del-programari)
    2. [Organització de l’enginyeria del programari](#2-organitzaci%C3%B3-de-lenginyeria-del-programari)
    3. Mètodes de desenvolupament de programari
    4. Tècniques i eines de l’enginyeria del programari
    5. Estàndards de l’enginyeria del programari
- Mòdul 2: Orientació a objectes
    1. Què és l’orientació a objectes?
    2. Classificació i abstracció
    3. Ocultació d’informació i encapsulament
    4. Herència i polimorfisme
    5. Cas pràctic: un fòrum virtual
- Mòdul 3: Requisits
    1. Introducció als requisits
    2. Obtenció dels requisits
    3. Gestió de requisits
    4. Documentació dels requisits
    5. Casos d’ús
- Mòdul 4: Anàlisi UML
    1. Anàlisi orientada a objectes amb UML
    2. Model de casos d’ús
    3. Modelització de la interfície
    4. Model del domini

-----------------------------------------------

<h1 class="titol-modul" id="modul-1">Mòdul 1: Introducció a l'enginyeria del programari</h1>

# 1. Què és l'enginyeria del programari?

<div class="aclaracio">

**Enginyeria:** (_interpretació personal_) acció d'utilitzar els coneixements científics adequats per a conseguir solucionar problemes a trabés de la tecnologia.

>L'aplicació pràctica de la ciència i la tecnologia - [Viquipèdia](https://ca.wikipedia.org/wiki/Enginyeria)

>Art d'aplicar els coneixements científics a la invenció, al perfeccionament o a la utilització de les tècniques en totes llurs determinacions dins el camp industrial. - [Gran Enciclopèdia Catalana](https://www.enciclopedia.cat/gran-enciclopedia-catalana/enginyeria)

</div>

## 1.1. Programari i maquinari

**Programari:** La part intangible de qualsevol ordinador: tant les dades emmagatzemades com el conjunt d'accions a executar (_codi_).

>Conjunt dels programes de computació, procediments, regles, documentació i dades associades que formen part de les operacions d'un sistema de còmput - IEEE

<div class="aclaracio">

>**IEEE** són les sigles de _Institute of Electrical and Electronics Engineers_, l'Institut d'Enginyers Elèctrics i Electrònics, una associació tècnico-professional mundial dedicada a l'estandardització, entre altres coses. És la major associació internacional sense ànims de lucre formada per professionals de les noves tecnologies, com enginyers en informàtica, enginyers elèctrics, enginyers en electrònica, enginyers en sistemes i enginyers en telecomunicació. - [Viquipèdia](https://ca.wikipedia.org/wiki/Institute_of_Electrical_and_Electronics_Engineers)

</div>

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

Mentres abans el programari es construia per a fer càlculs matemàtics (_computadra_), avui en dia és una eina extesa a tot arreu (xarxes socials, sistemes d'informació, rellotges de polsera...). Per tant existeixen diferents tipus de programari ergo diferents maneres de desenvolupar-lo.

**Classificació de Roger Pressman (2005):**
- Programari de sistemes
- Programari d'aplicació
- Programari científic i d'enginyeria
- Programari encastat (_sistema embebido_)
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

## 1.6. L'enginyeria del programari comparada amb les altres enginyeries

Si s'aplica l'enginyeria al desenvolupament de programari es poden aprofitar els coneixements d'altres disciplines de l'enginyeria per millorar la manera en què gestionem aquestes activitats.

Així doncs s'han aplicat diferents metàfores per intentar taslladar els coneixements a la nostra disciplina. Però un dels perills de les metàfores és que, sovint, s'apliquen amb coneixements incomplets de partida, i pot portar a errors al traslladar els coneixements.

<p class="aclaracio">
No existeix un trasllat absolut de coneixements i pràctiques entre disciplines.
</p>

<div class="exemple">

**Exemple**:

L'arquitecta crea plànols que han d'estar llestos abans de començar la construcció. Els paletes són intercaviables (les instruccions a seguir són clares). Un cop finalitzada la feina el client pot contractar altres paletes pel manteniment.

Però no es té en compte factors com: l'edifici es construeix al mateix lloc on es farà servir, mentres que el programari no; el programari de qualitat s'ha de poder fer servir en entorns diferents; el cost de fer còpies del programari és gairabé nul comparat amb el cost del disseny.

</div>

**Diferències destacables** entre el programari i altres productes industrials:

1. **El programari és intangible**. No utilitza cap matèria prima física.
2. **El programari no es manufactura**. Crear-ne còpies té un cost quasi nul i el resultat de les còpies sempre és idèntic a l'original.
3. **El programari no es desgasta**. El tipus de manteniment és molt diferent ja que si una còpia falla no pot ser per desgast i per lo tant tota la resta de còpies també fallaran.
4. **El programari queda obsolet ràpidament**. La ràpida evolució tecnològica fa que quedi obsulet en poc temps a diferència d'altres disciplines industrials. Força a desenvolupar-ho amb poc temps i poc cost.

A més, cal destacar que l'enginyeria del programari és una disciplina relativament nova (comparada amb la resta d'enginyeries). L'experiència acumulada és relativament poca i aquest fet es veu agreujat per la ràpida evolució tecnològica, fonamentalment en dos eixos:

- Les noves possibilitats tecnològiques fan que canviï totalment la naturalesa dels productes que estem desenvolupant (per exemple l'aparició d'interficies gràfiques, d'Internet i/o els telèfons intel·ligents).
- L'augment de la potència de càlcul dels ordinadors provoca canvis fonamentals en les eines que es fan servir per desenvolupar programari (tant pels llenguatges i paradigmes com eines mateixes -entorns de desenvolupament, eines CASE...-)

>Les **eines CASE** (_computer aided software engineering_) són les eines que ens ajuden a dur a terme les diferents activitats de l’enginyeria del programari com ara la creació de models, generació de documentació, etc.

Per lo tant la majoria de coneixement queda obsolet ja que es va crear per solucionar problemes en un context diferent del que ens podem trobar avui en dia.

El **programari lliure** ha transformat totalment la manera de desenvolupar i mantenir el programari i ha promogut la creació d'estàndards, la reutilització de programari i a la difusió del coneixement respecte a com ha estat desenvolupat. Aquest nivell de transparència i col·laboració no existeix en cap altra enginyeria.



# 2. Organització de l'enginyeria del programari

**Mètodes de desenvolupament**: són els diferents mètodes definits que ens permet aplicar l'enginyeria a les activitats relacionades amb el programari, siguent sistemàtic, amb el desenvolupament, operació o manteniment (o una combinació de tots tres),

>Un mètode descriu les característiques del procés o procediment disciplinat utilitzat en l'enginyeria d'un producte o en la prestació d'un servei - IEEE

## 2.1. Organització del desenvolupament, operació i manteniment

Els processos de desenvolupament, d'operació i de manteniment poden tenir similituds, però les seves diferències fan que l'organització dels processos siguin molt diferents entre ells:

En el cas de l'operació les activitats són contínues, però el desenvolupament és temporal.

Les activitats de l'operació són repetitives, però el desenvolupament proporciona un resultat únic (un resultat per cada procés de desenvolupament).

>Mentre que el desenvolupament s'acostuma a organitzar en forma de projectes, l'operació s'organitza d'acord amb serveis.

Molts mètodes se centren en una única activitat de les tres mencionades. En aquest temari ens centrarem en les etapes de desenvolupament i manteniment.

<div class="aclaracio">
<p class="capçal">Lectures recomenades</p>
Si voleu aprofundir en la gestió de projectes, podeu consultar la guia PMBOK publicada pel Project Management Institute (PMI), mentre que si us interessa la gestió de l’operació del programari podeu consultar l’estàndard ITIL.
</div>

## 2.2. Organització dels projectes de desenvolupament

Els diferents mètodes per al desenvolupament del programari defineixen un o més processos de desenvolupament. La descripció d'un procés inclou:

- **Tasques**: quines fer i en quin ordre.
- **Rols**: dels diferents participants, quina responsabulitat tenen i quines tasques han de dur a terme.
- **Artefactes**: documents, programes, etc. que s'han de fer servir per cada tasca, i quins artefactes s'han de generar com a resultat.

Els criteris per escollir els processos definits per un mètode es basen en el seu abast (només al desenvolupament o també altres espectes), el tipus d'organització al que va dirigit, el tipus de producte a generar, entre d'altres...

## 2.3. Activitats de l'enginyeria del programari

Hi ha un seguit de tasques que coincidiran en tots els projectes de desenvolupament amb independencia de com s'organitzi.

**Activitat**: en aquest temari farem referència a _activitat_ com a un conjunt de tasques relacionades entre si. Les tasques són conceptes més concrets i que poden diferenciar molt entre projectes (generar un model conceptual, crear un diagrama de Gantt...), mentre que les activitats són més genèriques i coincideixen entre projectes (modlització, planificació...).

### 2.3.1. Gestió del projecte

>L'objectiu prinipal de la **gestió de projectes** és assegurar l'èxit del projecte

La gestió del projecte no és una activitat específica del desenvolupament del programari, i per això hi ha qui considera que no forma part de l'enginyeria del programari. Però forma part del projecte de desenvolupament i, per tant, els mètodes de desenvolupament l'han de tenir en compte.

Algunes tasques reslacionades amb la gestió del projecte:

- **Estudi de viabilitat**. Cal comprovar si per qüestions de cost i temps el projecte de desenvolupament és la millor solució
- **Estimació**. Temps i diners
- **Definir clarament els objectius del projecte**. En determinaran l'èxit o el fracàs.
- **Formar l'equip de desenvolupament**. Persones amb dedicació completa (desenvolupadors) o parcial(_stakeholders_)
- **Establir fites**. Permeten fer-ne un seguiment del procés.
- **Identificar riscos que puguin posar en perill el projecte**. Tant tecnològics com la resta de possibilitats (problemes legals, manca de suport de l'organització...)

<div class="aclaracio">
<p class="capçal">Stakeholder</p>
Qualsevol persona o organització interessada, afectada o implicada en el funcionament del programari que es desenvolupa.
</div>

La gestió del projecte variarà notablement segons el mètode de desenvolupament emprat.

**Podem resumir que la gestió del projecte consisteix en equilibrar tres variables**

1. l'abast del projecte (què inclourà i què no)
2. el temps (data final d'entrega)
3. el cost (recursos humans o materials)

La modificació d'una de les tres variables s'ha de comepensar modificant una de les altres dues.

>**Joc de suma zero**: En teoria de jocs, un joc de suma zero descriu una situació en què el guany o la pèrdua en què incorre un dels participants es compensa exactament per les pèrdues o guanys de la resta de participants. Així doncs, si sumem totes les pèrdues i tots els guanys, el resultat final és 0.

<div class="aclaracio">
<p class="capçal">Altres variables</p>
Wysocki (2009) afageix qualitat com a variable i distingeix entre cost (pressupost) i recursos (personal).
</div>

### 2.3.2. Identificació i gestió dels requisits

>Els requisits expressen les necessitats i restriccions que afecten un producte de programari que contribueix a la solució d'un problema del món real - SWEBOK (2004)

Per trobar-los cal comunicació i col·laboració amb els _stakeholders_.

Els requisits són el que determinen l'abast del projecte.

Les principals problemàtiques que ens podem trobar durant aquesta tasca són:

- **Diferències respecte a la informació amb què traballen les diferents parts**. _Stakeholders_ tenen una informació (referent al producte) i els desenvolupadors una altra (referent a la tencologia). Això pot generar perspectives diferents.
- **Limitacions del canal utilitzat**. Cada canal té pros i contras: comunicació escrita perd el llegunatge no verbal, mentre que si és verbal es perd la capacitat de revisió.
- **Limitacions del llenguatge utilitzat**. Llenguatge natural és propens a l'ambigüitat. Els llenguatges formals són menys expressius i necessiten que les dues parts l'entenguin.
- **Dificultat de definir el millor sistema possible**. _Stakeholders_ poden no acabar de comunicar els requisits del millor sistema possible (condicionats per altres sistemes que coneixen o no saber altres possibilitats).

<p class="aclaracio">Els problemes són generats per les complicacions durant la comunicació amb els <em>stakeholders</em>, i no pas per la naturalesa de l'enginyeria en sí.</p>

Per a solucionar aquests problemes s'usen tècniques basades en retroalimentació durant l'anlàlisi de requisits.

Per exemple: el prototipatge (ensenyar una versió amb aspecte similar al producte final però que no implementa la funcionalitat real) o els models (la seva utilitat està condicionada a que els _stakeholders_ entenguin lal notació).

### 2.3.3. Modelització

**Creació de models el sistema per desenvolupar**: facilitaran la comprensió dels requisits i el disseny del sistema.

És l'equivalent a la creació de maquetes en altres disciplines, amb la diferència que en aquest cas el model és intangible (com el producte final).

**UML** (_unified modeling language_) és el llenguatge més utilitzat per a creació de models de programari. Defineix tot un seguit de diagrames a partir dels quals podem elaborar els nostres models. Publicat per OMG (Object Management Group)

UML no imposa cap mètode de desenvolupament, i per això s'ha adoptat a la majoria de mètodes de desenvolupament actuals. També té l'avantatge que només defineix la notació que s'ha de fer servir però no quins artefactes s'han de generar (un mateix diagrama es pot fer servir en diversos artefactes -model de domini, diagrama de classes de disseny, etc...)

### 2.3.4. Construcció i proves

Inclou l'escriptura del codi font (implementació) i la realització de proves que garanteixin que ni hi hagi errors i que el producte compleixi amb els seus requisits.

Llavors podríem **desplegar** el producte: crear els arxius executables i donar-los als usuaris.

### 2.3.5. Qualitat

Seria una activitat que inclouria totes les etapes del desenvolupament.

Per medir la qualitat necessitem, a part de els criteris d'acceptació del sistema (què necessita el projecta per dir que està finalitzat), un conjunt de mètriques per verificar si compleix amb els criteris de qualitat marcats.

### 2.3.6. Manteniment reenginyeria

**Manteninemt correctiu**: corregir errors detectats al programari, modificant el codi font i generant una nova versió del programa.

**Manteniment evolutiu**: afegir noves funcionalitats (o adaptar les existents) per satisfer noves necessitats detectades després de la fi del desenvolupament.

### 2.3.7. Activitats des del punt de vista del cicle de vida del projecte

El _Project Management Institute_ (associació professional que publica estàndards de bones pràctiques en la gestió de projectes) fa una classifiació diferent, es fixa en la gestió del projecte i en quin punt del cicle de vida es du a terme cada tasca:

- **Tasques d'iniciació**. Decidir si el projecte es du a terme o se substitueix per una altra solució
- **Tasques de planificació**. Definir quines tasques fer i en quin ordre.
- **Tasques d'execució**. Escriure els programes.
- **Tasques de seguiment i control**.  Serveixen per detectar problemes i corregir-los, així com validar la planificació.
- **Tasques de tancament**. Tot lo relacionat amb la finalització del projecte (comprovar que satisfà les necessitats, resoldre contractes, traspassar el programari a l'equip d'operacions).

Poden estar executades una després de l'altre, a l'hora o combinades de diferents maneres.

## 2.4. Rols en l'enginyeria de programari

En els projectes intervenen moltes persones, i una bona definició de rols pot ser determinant per arribar a l'èxit del projecte.

Els rols que hi hauran en un mètode dependran del seu abast. No tots els mètodes tindran els mateixos rols.

<div class="aclaracio"><p class="capçal">Lectura recomenada</p>

**Tom DeMarco; Timothy Lister** (1999). Peopleware: productive Projects and Teams (2a. ed.). Dorset House Publishing Company.
</div>

- El cap de projectes
- Els experts del domini
- L'analista funcional
- L'arquitecte
- L'analista orgànic o analista tècnic
- Els programadors
- L'expert de qualitat (provador)
- L'encarregat del desplegament
- El responsable de producte
- Altres rols

### 2.4.1. El cap de projectes

Responsable d'aconseguir els objectius del projecte.

És un rol no tècnic encarregat d'organitzar el projecte, coordinar l'equip i vetllar pels objectius (tant de costos com de valor generat).

### 2.4.2. Els experts del domini

Persones que coneixen el domini del sistema que s'està desenvolupant, els principals coneixedors dels requisits. Normalment no són tècnics sinó experts d'altres coneixements (vendes, finances, producció, etc).

Aquest rol també és conegut com a "analista de negoci" (_business analyst_).

### 2.4.3. L'analista funcional

Pèrfil tècnic. Ha d'unificar les diferents visions del domini en un únic model.

A diferència dels experts del domini, sí ha de conèixer la tecnologia, encara que no en conegui els detalls.

### 2.4.4. L'arquitecte

Rol tècnic. Ha de definir el disseny del sistema i escollir la tecnologia adequada. Amb la informacuió que li doni l'analista, crearà l'arquitecutra i el disseny que serà utilitzat com a base pel treball dels desenvolupadors.

### 2.4.5. L'analista orgànic o analista tècnic

Fa el disseny detallat del sistema (respectant la feina de l'arquitecte). El destinatari de la seva feina és el programador.

### 2.4.6. Els programadors

Escriuen el codi font amb els que es generaran els programes. Experts en la tecnologia d'implementació. També s'inclou a altres especialistes que participen creant codi pel programa (encara que no sigui amb un llenguatge de programació), com els especialistes en bases de dades.

### 2.4.7. L'expert de qualitat (provador)

Vetlla per la qualitat del producte desenvolupat. No és qui comprova la qualitat del codi font (d'això s'encarreguen els programadors amb les proves automàtitzades), sinó que s'encarrega d'opinar sobre el producte final.

Verifica que el programa compleix amb els requisits, i és qui decideix si el programa podrà acabar en mans dels usuaris finals.

### 2.4.8. L'encarregat del desplegament

Encarregat d'empaquetar i enviar el programari un cop estigui finalitzat el seu procés de desenvolupament (validat i tot).

### 2.4.9. El responsable de producte

Té la visió global del producte que es vol desenvolupar i vetlla pel seu desenvolupament correcte. No ha de ser expert en el domini però sí que ha de conèixer l'estrategia d'organització.

### 2.4.10. Altres rols

Els rols que hi hagi en un projecte dependrà molt del mètode aplicat, i per lo tant podrien haver-hi atres rols (o menys rols).

Hi ha altres persones influents al projecte que no formen part de l'equip de desenvolupament (cap de desenvolupament, director general de l'organització, etc).



# 3. Mètodes de desenvolupament de programari