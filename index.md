# Epistemisk usikkerhet

Jeg lærte nylig om et nyttig statistisk konsept - skillet mellom aleatorisk og epistemisk usikkerhet. Ordet "aleatorisk" kommer fra det romerske terningspillet alea, og aleatorisk usikkerhet er usikkerheten som kommer av de sanne stokastiske elementene i utfallet vi modellerer. Epistemisk usikkerhet er derimot usikkerheten som kommer av ting vi ikke vet, men som påvirker utfallet. Et eksempel på aleatorisk usikkerhet er usikkerhet i målingsmetoden som ligger til grunn for dataene, mens et eksempel på epistemisk usikkerhet er hvilke kort motstanderen sitter med i poker.

![Cæsar modellerer invasjon av Italia](https://github.com/Fesche/log_b/blob/gh-pages/img/C%C3%A6SAR_PAUSED_ON_THE_BANKS_OF_THE_RUBICON.gif)
<br>*<sub><sup>"Alea iacta est" - Julius Cæsar som blander sammen aleatorisk og epistemisk usikkerhet</sub></sup>*

Allerede i eksemplet over, valgt for å være erketypisk, kan man imidlertid merke en spenning. Hvis man kan forbedre målemetoden, er ikke da målingsusikkerhet epistemisk? Og hvis man antar at modellen må forholde seg til spillets regler i poker, er ikke da usikkerheten som resulterer av å ikke vite motstanderens hånd ureduserbar, og dermed aleatorisk? Definisjonene er dermed avhengig av kontekst, og selv aleatorisk usikkerhet fordufter for Maxwells demon. 

Definisjonen er allikevel nyttig som konseptuelt verktøy når man tenker over bruk av maskinlæringsmodeller. Lærebøker i maskinlæring og statistikk har en tendens til å behandle all usikkerhet som aleatorisk, men i virkeligheten er det skjelden at dette er den viktigste kilden til usikkerhet. Problemet er at det alltid er fristende å tolke en output fra en modell trent til binær klassifisering som sannsynligheten for at utfallet finner sted. I "modell-universet", bestående av et sett observasjoner av et utvalg dimensjoner, så er dette i de fleste tilfeller matematisk korrekt. Hvis dataene inneholder alle relevante dimensjoner for utfallet, og er representative for en underliggende fordeling så har man ingenting å frykte. Hvis man derimot modellerer utfall som finner sted i virkeligheten og avhenger av komplekse systemer (som menneskelige avgjørelser), så har man som regel ingen grunn til å tro at noen av disse antagelsene holder. Modellens output må dermed tolkes ikke som en sannsynlighet, men som en sannsynlighet *gitt modellens tilgjengelige observasjoner*. Dette høres kanskje ut som flisespikkeri, men det er viktig å ha i bakhodet når man skal formidle resultatene fra en modellkjøring. Dersom man har grunn til å tro at det finnes viktige dimensjoner eller sjeldne observasjoner som ikke finnes i modellens treningsdata er dette vel så viktig informasjon å få med seg når man tolker resultatet av en kjøring som selve outputen fra modellen. Den epistemiske usikkerheten kan være så mangt, inkludert ukjente variabler som dominererer alle dimensjoner inkludert i modellen.

Det vitner om fagets umodenhet at dette ikke er konsepter som gnis inn fra starten på universitetet. I hvert fall ble det ikke gnidd inn da jeg tok mine kurs i maskinlæring for 3-4 år siden.

Til slutt: EUs matsikkerhetsmyndighet EFSA har utviklet [et rammeverk for formidling av usikkerhet](https://efsa.onlinelibrary.wiley.com/doi/10.2903/j.efsa.2019.5520) som inkluderer åtte punkter:

> 1. unqualified conclusions with no expression of uncertainty; 
> 2. description of a source of uncertainty; 
> 3. qualitative description of the direction and/or magnitude of uncertainty; 
> 4. inconclusive assessment; 
> 5. a precise probability; 
> 6. an approximate probability; 
> 7. a probability distribution; and 
> 8. a two-dimensional probability distribution.

Jeg skal definitivt ha dette i bakhodet når jeg kommuniserer output fra mine modeller fremover!

# Trær og dumme voksne

Som barn var jeg velsignet med mange leker. Jeg hadde Action Man, Game Boy, hoppestav og diablo. 

Til tross for dette, var det to leker jeg utvilsomt likte best. Hadde du spurt mine venner, tror jeg også de ville ha gitt det samme svaret. Hvis de i det hele tatt hadde kommet på å kategorisere disse tingene som leker.

Jeg snakker selvfølgelig om ball og pinne.

Ballen er en selvskreven topp-leke. Barn og voksne verden over leker ukentlig med ball. Wikipedia kan liste over 170 forskjellige ballsporter fra samtlige av verdens kriker og kroker. Ballen er den universale leke. Går jeg forbi noen som sparker en fotball, kan jeg ikke la være å lengselsfullt håpe på at de skal skyte den i min retning, bare så jeg kan sparke den tilbake. Finner jeg en liten ball, plukker jeg den opp nesten uten unntak, eller sparker den gatelangs til den triller ned i en uangripelig grøft. Selv ett enkelt sprett eller spark er nok. Nok til at humøret løftes, og gangen blir litt lettere. 

Pinnen, på den andre side, mistenker jeg å være noe mindre universal. Det er langt færre pinnesporter enn ballsporter, og som voksen må jeg innrømme at den engang så magiske pinnen har mistet mye av sin sjarm. Da jeg gikk på barneskolen derimot, var pinnen alfa og omega. Skolen min lå omringet av skog, og denne skogens pinner utgjorde min barndoms borger og sverd. Hver vår og høst bygget vi små hytter og mektige slott av pinner, og inntil vi var gamle nok til å gjøre faktisk skade var skolegården regelmessig vitne til episke slag.

Det er her de voksne kommer inn i historien. Eller rettere sagt, overraskende nok er det ikke her de kommer inn. For det var aldri volden vi utøvde mot hverandre som berettiget irettesettelse. Det var volden vi utøvde mot trærne.

Det er ikke til å skyve under en stol, at trærne var de største ofrene under pinnelek. Og kan så være ble skogen omkring skolen litt tynnere i veksten takket være vår innsats, men det er de voksnes argument som alltid forundret meg. De sa alltid noe i duren "hva om noen kom og rev armene av deg? Ville du likt det?". Selv som barn syntes jeg dette argumentet var nærmest pinlig dårlig. Det kunne da umulig være sammenliknbart å rive en pinne av et tre og å rive en lem av et menneske? Eller et hvilket som helst annet dyr? Hvis det er vold å knekke greiner av et tre, hva er det da å høste en kornåker? Folkemord? Greit nok om dere syntes det ble stygt med de brukne grenene, eller næret en slags spirituell omsorg for buskvekster, men forklar det da på en måte som gir mening. Under denne oppfatning forholdt jeg meg til min egen fornuft, og fortsatte å høste greiner fra trær, om enn kanskje litt mer omtenksomt enn tidligere.

Kan du tro min store overraskelse da jeg kom tilbake til skolen som voksen, og fikk se at nesten hele skogen var fjernet til fordel for asfaltert lekeplass og parkeringsplass. De dumme voksne hadde dradd opp alle trærne. Mine gamle lærere må ha sagt opp i protest.
