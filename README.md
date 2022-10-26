# Web Typography, 2020/2021

Als je doof bent, of als je om een andere reden geen geluid kunt horen, dan mis je veel informatie als je een film kijkt. Knisperende voetstappen, langzaam aanzwellende muziek, nerveus getik op een deur, je hoort het natuurlijk allemaal niet. Nu bestaat er zoiets als *closed caption*, wat een type ondertiteling is waarbij ook dingen als omgevingsgeluiden en de muziek beschreven worden. Hierdoor krijgt een kijker die informatie wel binnen.

Alleen wordt die auditieve informatie nogal neutraal beschreven. Het geluid van huilend persoon zou bijvoorbeeld beschreven kunnen worden als *snikgeluid op de achtergrond*. En iemand die lacht zou geschreven kunnen worden als *iemand lacht.* Heel neutraal, bijna zakelijk, en bovendien allebei in precies hetzelfde neutrale lettertype. Terwijl het toch echt over twee heel verschillende emoties gaat. 

Dat kan visueel sterker. 

En dat gaan jullie doen.

## Leerdoelen

- Je kan de kennis over vormgeving die je hebt opgedaan tijdens de minor technisch toepassen met behulp van CSS
- Je kan verborgen nuance uit een audiotrack overtuigend vertalen naar visuele (typografische) beelden
- Je kan je typografische keuzes onderbouwen.
- Je hebt de exclusive design principles gebruikt.

## Oplevering

Je levert een werkende versie op, gemaakt met HTML, CSS en JavaScript. Deze staat op Github. In een duidelijke readme documenteer en onderbouw je je ontwerpkeuzes. Je developmentgeschiedenis is terug te vinden op GitHub.

Je levert ook een *screen recording* met audio op van je fragment. Dit is een video van de definitieve versie, gemaakt van jouw browserscherm.

De beoordeling is mondeling en volgt [de rubric uit het beoordelingsformulier](web-typografie-beoordeling.pdf).

## Typografische restricties

Je *moet* een van deze twee opties kiezen, en je keuze moet je onderbouwen. In je readme staat een uitleg over je overwegingen om de ene of de andere restrictie te kiezen.

### Optie 1: Systeemfont

De eerste optie is dat je gebruik maakt van het zogenaamde *systeemfont* van degene die naar jouw werk kijkt. Dit font verschilt per operating system, en het verschilt soms zelfs per versie van het operating system. Het is ook aan te passen door de gebruiker zelf. 

Je hebt dus geen controle over welk lettertype er precies gebruikt wordt. Het levert dus een onzeker, en beperkt typografisch palet op. Je hebt geen *light* versies, of *extrabold*. En ook geen serif en sans-serif versie van dezelfde familie. In dit geval heb je alleen de beschikking over normal, **bold** en _italic_. Dit heeft natuurlijk ook zijn voordelen!

### Optie 2: Brenner

Je kan er ook voor kiezen om gebruik te maken van de complete Brenner familie. Dit is een zeer uitgebreid en uiterst flexibel font. [Hier kan je je verdiepen in dit font](https://www.typotheque.com/blog/brenner_an_unusual_typeface_family_with_distinct_voices). Als je kiest voor dit font dan heb je de beschikking over een *sans serif*, een *condensed*, een *serif*, een *monotype*, een *slab*, een *display* en een *script* versie. En veel van deze versies hebben varianten van *light* tot *bold*, en allemaal zowel *bold* als *italic*.

Met Brenner zijn er natuurlijk veel en veel meer mogelijkheden dan met systeemfonts. Dat kan zowel een voordeel als een nadeel zijn. 

Voor een overzicht, zie [de brenner.pdf](brenner.pdf).

## Het fragment

Ik heb een fragment voorbereid. Het gaat om twee scenes uit *Blade Runner 2049*. De captions staan in de HTML, en ze verschijnen in sync met de video. [Kijk maar](closed-captions/index.html).

### De captions

De captions staan in de html, in het bestand index.html. Je kan aan elke paragraaf eventueel een of meer classes toevoegen. Bijvoorbeeld `voice1` of `voice2 soft`. Classes voeg je handmatig toe in de html.

Met JavaScript worden er een paar dingen extra gedaan: 

- er wordt aan elke paragraaf een unieke class toegevoegd (`p0`, `p1`, etc)
- Elk woord wordt in een aparte `span` gezet. Hierdoor kan je elk woord apart stylen, en eventueel ook [na elkaar laten verschijnen](https://github.com/cmda-minor-vid/web-typography-18-19/blob/master/closed-captions/css.css#L41).

### Tijdens het afspelen

Tijdens het afspeelen wordt er een class `on` op de caption gezet als hij moet verschijnen, en een class `off` als hij klaar is. *Zowel class `on` als class `off` blijft op de caption staan!*

De timimg van de captions kan je aanpassen in [closed-captions/captions.js](closed-captions/captions.js).

Er verschijnen ook classes op de body op momenten dat er geluiden worden afgespeeld, zoals `sound1` en `sound2`. Je kan geluiden toevoegen in [closed-captions/sounds.js](closed-captions/sounds.js).

*let op,* de geluiden zijn niet compleet, dit zal je zelf moeten aanvullen.

## Typografie

Voor de typografie heb ik gekozen voor het Brenner font, dit heb ik gekozen omdat ik hier de meeste kansen en verschillende mogelijkheden in zag. Door de verschillende soorten kan ik kiezen welke bij wat voor personage past. Ik heb gekozen voor Brenner Mono Bold. Een simpele een stevige letter. De personages (voice 1 & voice 2) praten beide erg streng en bazig waardoor ik vond dat er een bold font bij aansloot.

Voor voice 3  het personage met een zin, Fuck off, skin-job! heb ik gekozen om het in een italic stijl te plaatsen. Zo valt het voor de kijker op dat er iets “speciaals” aan de hand is met deze zin. Dit personage loopt voorbij en brengt in de paar seconden een onprettige sfeer met zich mee. Om de sfeer te proberen over te brengen heb ik de woorden Fuck Off een line-through gegeven om aan te geven dat dit aanstootgevende woorden zijn. Verder heb de woorden wel op normaal groote gelaten omdat het verder redelijk timide maar krachtig werd uitgesproken en ik de kijker niet het gevoel wilde geven dat het geschreeuwd werd.

De vierde stem/ het vierde personage is voice 4. Deze komt in mij  einde terug in de filmscène. Het is een wat kalmere stem vergeleken de andere drie, ergens ook wel een beetje opgewekt.  Ik heb ook dit personage in Brenner Mono Bold  gedaan omdat ondanks hij wat kalmer is is de boodschap wel scherp. Hierdoor heb ik een contrast met kleur en typografie gebruikt om het gevoel zo goed mogelijk over te brengen op de kijker.
 
## Kleurkeuze

Ik heb er voor gekozen de kijker een echt filmbeleving te proberen te geven. Een zwarte achtergrond zodat de filmscène er goed in naar voren komt.  Voor de verschillende personages heb ik ook verschillende kleuren gebruikt. Zo heb ik voor voice 1  een lichte groen blauwe neon kleur gebruikt. Deze komt goed naar voren op de zwarte achtergrond. Voor voice 2 heb ik gekozen voor een neon roze kleur. Ook deze kleur komt goed naar voren met de zwarte achtergrond. De kleuren van Voice 1 & Voice 2 heb ik gebaseerd op het allereerste beeld van deze film scene. De twee neon-borden zijn dezelfde kleuren. 
Voor Voice 3 heb ik een rode kleur uitgekozen. Rood wordt vaak geassocieerd met kwaad en boos zijn. Doordat het personage aan het vloeken is in de scene heb ik dit gevoel proberen over te brengen.
Als laatste voice 4, Voice 4 is een wat zachtere en timide stem met een duidelijke boodschap. Doordat ik al een wat stevigere letter heb uitgekozen wilde ik een goede balans vormen voor dit personage. Ik heb gekozen voor een gele kleur, geel wordt gezien als een vrolijke en lieve kleur. Vandaar dat ik een stevige letter wilde combineren met een wat lievere kleur om zo de balans te vinden en ook hier een gevoel mee heb proberen over te brengen.
 
In de scènes gaan er sirenes en/of alarmen af. Dit zijn vaak noodsignalen en zijn meestal rood. Ik heb daarom ervoor gekozen om een rode kleur te gebruiken voor deze geluiden zodat een doof persoon ook snel deze link kan leggen. Naast de rode kleur heb ik ook gekozen voor wit. Dit heb   ik gedaan voor de schelle geluiden. Omdat het witte licht al snel pijn gaat doen aan ogen en en de schelle geluiden aan de oren wilde ik deze ervaring hetzelfde houden. 
Ook is het geluid van de sire/alarm aan het opbouwen van heel zacht naar steeds luider. Hier heb ik ook wit voor gebruikt. het licht wordt steeds feller naarmate het geluid toeneemt. Zo heb ik geprobeerd dezelfde opbouwende spanning te creëren

## Feedbacksessies/Voortgangsgesprekken





## Uittesten


## Exclusive Design Principles
Study Situation
Ignore Conventions
Prioritise Identity
Add Nonsense


## Nawoord
---
Webtypgrafie vond ik een erg lastig vak. Code is een onderwerp waar ik veel moeite mee heb en hierdoor minder leuk ben gaan vinden dan voorheen. Maar ondanks ik het een moeilijke opdracht vond heb ik er wel ontzettend veel van geleerd en het zelfs leuk gevonden! Iets wat ik uiteindelijk erg belangrijk vind. > Ik heb mijzelf uitgedaagd voor deze opdracht en ik ben er best wel trots op. Ik heb helaas wel een 2e fragment moeten laten vallen omdat ik heel lang ben bezig geweest met het uitzoeken hoe alles werkt. Daarom heb ik alleen het 1e fragment zo goed mogelijk proberen neer te zetten!


## Bronnen