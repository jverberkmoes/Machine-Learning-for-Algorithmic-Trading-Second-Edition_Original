### 
# META Data Translation/Vertaling
# Date translation: jan-8-2026
# Translator      : Jos Verberkmoes (Discretionair investor), Netherlands
# Source file     : /01_machine_learning_for_trading/README.md (English)
# Translated file : /01_machine_learning_for_trading/READMENL.md (Dutch)
# Added at the end: PARTS & Chapters - Machine Learning For Trading by Stefan Jansen 
### 

# Machine Learning voor handel: Van idee tot uitvoering
Algoritmische handel maakt gebruik van computerprogramma's die **algoritmes** uitvoeren om bepaalde of alle elementen van een handelsstrategie te automatiseren. Algoritmes zijn een reeks stappen of regels die zijn ontworpen om een doel te bereiken. Ze kunnen vele vormen aannemen en optimalisatie mogelijk maken gedurende het hele beleggingsproces, van idee generatie tot vermogensallocatie, handelsuitvoering en risicomanagement. 

**Machine Learning** (ML) omvat algoritmes die regels of patronen leren uit data om een doel te bereiken, zoals het minimaliseren van een voorspellingsfout. De voorbeelden in dit boek illustreren hoe ML-algoritmes informatie uit data kunnen halen om belangrijke beleggings- activiteiten te ondersteunen of te automatiseren. Deze activiteiten omvatten het observeren van de markt en het analyseren van data om verwachtingen over de toekomst te vormen en te beslissen of koop- of verkooporders moeten worden geplaatst, evenals het beheren van 
de resulterende portefeuille om aantrekkelijke rendementen te behalen ten opzichte van het risico.

Uiteindelijk is het doel van actief beleggingsbeheer het genereren van alfa, gedefinieerd als portfoliorendementen die hoger zijn dan de benchmark die voor evaluatie wordt gebruikt. De **fundamentele wet van actief beheer** stelt dat de sleutel tot het genereren van alfa ligt in het hebben van nauwkeurige rendementsprognoses in combinatie met het vermogen om op deze prognoses te reageren (Grinold 1989; Grinold en Kahn 2000).

De wet definieert de **informatieverhouding** (IR) om de waarde van actief beheer uit te drukken als de verhouding tussen het rendementsverschil tussen de portefeuille en een benchmark en de volatiliteit van die rendementen. De IR wordt verder benaderd als het product van:
  - De **informatiecoëfficiënt** (IC), die de kwaliteit van de prognoses meet als hun rangcorrelatie met de uitkomsten
  - De wortel van de **strategiebreedte**, uitgedrukt als het aantal onafhankelijke weddenschappen op deze prognoses

De concurrentie tussen ervaren beleggers op de financiële markten impliceert dat het maken van nauwkeurige voorspellingen om alfa te genereren superieure informatie vereist, hetzij door toegang tot betere data, een superieur vermogen om deze te verwerken, of beide. Hier komt ML om de hoek kijken: toepassingen van **ML for Trading (ML4T)** zijn er doorgaans op gericht om efficiënter gebruik te maken van een snel diversificerende hoeveelheid data om betere en meer bruikbare voorspellingen te genereren, waardoor de kwaliteit van beleggingsbeslissingen en -resultaten verbetert.

Historisch gezien werd algoritmische trading enger gedefinieerd als de automatisering van de uitvoering van transacties om de kosten voor de verkopende partij te minimaliseren. Dit boek neemt een breder perspectief, aangezien het gebruik van algoritmes in het algemeen en ML in het bijzonder een breder scala aan activiteiten beïnvloedt, van het genereren van ideeën en het extraheren van signalen uit data tot assetallocatie, bepaling positiegrootte en het testen en evalueren van strategieën.

Dit hoofdstuk behandelt trends in de sector die hebben geleid tot de opkomst van ML als bron van concurrentievoordeel in de beleggingsindustrie. We zullen ook bekijken hoe ML in het beleggingsproces past om algoritmische handelsstrategieën mogelijk te maken. Meer specifiek behandelen we de volgende onderwerpen:
  - Belangrijkste trends achter de opkomst van Machine Learning in de beleggingssector
  - Het ontwerpen en uitvoeren van een handelsstrategie die gebruik maakt van Machine Learning
  - Populaire toepassingen van Machine Learning in de handel


## De opkomst van Machine Learning in de beleggingssector

De beleggingssector heeft zich de afgelopen decennia drastisch ontwikkeld en blijft zich ontwikkelen te midden van toenemende concurrentie, technologische vooruitgang en een uitdagende economische omgeving. In dit onderdeel worden de belangrijkste trends besproken die de algehele beleggingsomgeving hebben gevormd, en in het bijzonder de context voor algoritmische handel en het gebruik van Machine Learning.

De trends die algoritmische handel en Machine Learning (ML) tot hun huidige prominentie hebben gebracht, zijn onder andere:
   -  Veranderingen in de marktmicrostructuur, zoals de verspreiding van elektronische handel en de integratie van markten over verschillende activaklassen en geografische gebieden.
   - De ontwikkeling van beleggingsstrategieën die zijn geformuleerd in termen van blootstelling aan risicofactoren, in plaats van activaklassen.
   - De revoluties in rekenkracht, datageneratie en -beheer, en statistische methoden, inclusief doorbraken in deep learning.
   - De betere prestaties van de pioniers in algoritmische handel ten opzichte van menselijke, discretionaire (naar eigen inzicht, oordeel of goeddunken) beleggers.

Daarnaast hebben de financiele crises van 2001 en 2008 invloed gehad op de manier waarop beleggers diversificatie en risicomanagement benaderen. Een gevolg hiervan is de opkomst van goedkope passieve beleggingsinstrumenten in de vorm van Exchange Traded Funds (ETF's). Te midden van lage rendementen en lage volatiliteit na de crisis van 2008, die leidde tot grootschalige aankopen van activa door toonaangevende centrale banken, verschoven kostenbewuste beleggers meer dan $ 3,5 biljoen van actief beheerde beleggingsfondsen naar passief beheerde ETF's.

De concurrentiedruk komt ook tot uiting in de lagere beheerkosten van hedgefondsen. Deze daalden van de traditionele 2 procent jaarlijkse beheerkosten en 20 procent winstafdracht naar gemiddeld respectievelijk 1,48 procent en 17,4 procent in 2017.
Van elektronische naar hoogfrequente handel

### Van elektronische naar hoogfrequente

Elektronische handel heeft zich sinds de jaren 60, toen de netwerken begonnen met het routeren van koersen naar computerterminals, drastisch ontwikkeld op het gebied van mogelijkheden, volume, dekking van activaklassen en geografische gebieden.
   - [Dark Pool Trading & Finance](https://www.cfainstitute.org/en/advocacy/issues/dark-pools), CFA Institute
   - [Dark Pools in Equity Trading: Policy Concerns and Recent Developments](https://crsreports.congress.gov/product/pdf/R/R43739), Congressional Research Service, 2014
   - [High Frequency Trading: Overview of Recent Developments](https://fas.org/sgp/crs/misc/R44443.pdf), Congressional Research Service, 2016

# Factorbeleggen en smart beta-fondsen

Het rendement van een belegging is afhankelijk van de onzekerheid of het risico dat aan de financiële investering is verbonden. Een aandeleninvestering houdt bijvoorbeeld in dat men het bedrijfsrisico van een onderneming op zich neemt, terwijl een obligatieinvestering het risico op wanbetaling met zich meebrengt.

Voor zover specifieke risicokenmerken rendementen voorspellen, wordt het identificeren en voorspellen van het gedrag van deze risicofactoren een primaire focus bij het ontwerpen van een beleggingsstrategie. Dit levert waardevolle handelssignalen op en is de sleutel tot superieure resultaten bij actief beheer. Het inzicht van de sector in risicofactoren is in de loop der tijd aanzienlijk geëvolueerd en heeft invloed gehad op hoe Machine Learning wordt gebruikt voor algoritmische handel.

De factoren die rendementen verklaarden die verder gingen dan het CAPM (Capital Asset Pricing Model) werden opgenomen in beleggingsstijlen die portefeuilles in het voordeel van één of meer factoren kantelen, en activa begonnen te migreren naar factorgebaseerde portefeuilles. De financiële crisis van 2008 onderstreepte hoe misleidend de labels van activaklassen kunnen zijn en een vals gevoel van diversificatie kunnen creëren wanneer beleggers niet kijken naar de onderliggende factorrisico's, aangezien activaklassen tegelijkertijd instortten.

In de afgelopen decennia is kwantitatief factorbeleggen geëvolueerd van een eenvoudige aanpak gebaseerd op twee of drie stijlen naar **multifactor smart** of **exotische bèta-producten**. 
Smart beta-fondsen hebben in 2017 de grens van $ 1 biljoen aan beheerd vermogen (AUM/Assets Under Management) overschreden, wat getuigt van de populariteit van deze hybride beleggingsstrategie die actief en passief beheer combineert. 
Smart beta-fondsen hanteren een passieve strategie, maar passen deze aan op basis van een of meer factoren, zoals goedkopere aandelen of selectie op basis van dividenduitkeringen, om een beter rendement te genereren. Deze groei valt samen met toenemende kritiek op de hoge kosten die traditionele actieve beheerders in rekening brengen, evenals een grotere controle op hun prestaties.

De voortdurende ontdekking en succesvolle voorspelling van risicofactoren die, afzonderlijk of in combinatie met andere risicofactoren, een significante impact hebben op toekomstige rendementen in verschillende activaklassen, is een belangrijke drijfveer achter de opkomst van Machine Learning in de beleggingssector en zal een belangrijk thema zijn in dit boek.

### Algoritmische pioniers presteren beter dan mensen en groeien in omvang

De trackrecords en de groei van het beheerd vermogen (AUM/Assets Under Management) van bedrijven die vooropliepen in algoritmische handel hebben een belangrijke rol gespeeld bij het genereren van interesse bij beleggers en de daaropvolgende inspanningen in de sector om hun succes te repliceren.

Systematische strategieën die grotendeels of uitsluitend gebaseerd zijn op algoritmische besluitvorming werden vooral bekend door wiskundige **James Simons**, die in 1982 Renaissance Technologies oprichtte en uitbouwde tot het toonaangevende kwantitatieve beleggingsbedrijf. Het geheimzinnige **Medallion Fund**, dat niet toegankelijk is voor buitenstaanders, heeft sinds 1982 een geschat jaarlijks rendement van 35% behaald.

**DE Shaw, Citadel en Two Sigma**, drie van de meest prominente kwantitatieve hedgefondsen die gebruikmaken van systematische strategieën op basis van algoritmes, stegen in 2017 voor het eerst naar de top 20 van best presterende fondsen aller tijden, gemeten naar het totale bedrag dat beleggers na aftrek van kosten hebben verdiend sinds de oprichting.

#### Door Machine Learning gedreven fondsen trekken $1 biljoen aan beheerd vermogen aan

Morgan Stanley schatte in 2017 dat algoritmische strategieën de afgelopen zes jaar met 15% per jaar zijn gegroeid en ongeveer $ 1,5 biljoen beheren, verdeeld over hedgefondsen, beleggingsfondsen en smart beta ETF's. Andere rapporten suggereren dat de kwantitatieve hedgefondssector op het punt stond de grens van $1 biljoen aan beheerd vermogen te overschrijden, bijna een verdubbeling ten opzichte van 2010, te midden van uitstroom uit traditionele hedgefondsen. Ter vergelijking: het totale kapitaal van de hedgefondssector bereikte $3,21 biljoen volgens het meest recente wereldwijde rapport van Hedge Fund Research.

  - [Wereldwijde markt voor algoritmische handel zal in 2026 de US$ 21.685,53 miljoen  overstijgen](https://www.bloomberg.com/press-releases/2019-02-05/global-algorithmic-trading-market-to-surpass-us-21-685-53-million-by-2026)
  - [De aandelenmarkt wordt nu beheerd door computers, algoritmes en passieve beheerders](https://www.economist.com/briefing/2019/10/05/the-stockmarket-is-now-run-by-computers-algorithms-and-passive-managers), Economist, 5 oktober 2019

### De opkomst van kwantitatieve beleggingsfondsen

Binnen actief beleggingsbeheer hebben zich twee verschillende benaderingen ontwikkeld: systematisch (of kwantitatief) en discretionair beleggen. Systematische benaderingen maken gebruik van algoritmes voor een herhaalbare en datagedreven aanpak om beleggingskansen in een groot aantal effecten te identificeren; een discretionaire aanpak daarentegen omvat een diepgaande analyse van een kleiner aantal effecten. Deze twee benaderingen gaan steeds meer op elkaar lijken naarmate fundamentele fondsen meer gebruikmaken van datawetenschap.

Zelfs fundamentele handelaren bewapenen zich nu met kwantitatieve technieken, goed voor $ 55 miljard aan systematisch vermogen, volgens Barclays. Kwantitatieve fondsen zijn niet gebonden aan specifieke bedrijven en handelen in patronen en dynamieken in een breed scala aan effecten. Kwantitatieve fondsen vertegenwoordigen nu ongeveer 17% van het totale vermogen van hedgefondsen, zo blijkt uit gegevens van Barclays.

### Machine Learning en alternatieve data

Hedgefondsen zijn al lange tijd op zoek naar alpha door middel van informatievoordeel en het vermogen om nieuwe, niet-gecorreleerde signalen te ontdekken. Historisch gezien omvatte dit zaken als eigen enquêtes onder consumenten of kiezers in de aanloop naar verkiezingen of referenda. Soms gaat, het gebruik van bedrijfsinsiders, artsen en expertnetwerken om de kennis over trends in de sector of bedrijven te vergroten, de wet over: een reeks vervolgingen van handelaren, portefeuillemanagers en analisten voor het gebruik van voorkennis na 2010 heeft de sector opgeschud.

Daarentegen is het informatievoordeel van het benutten van conventionele en alternatieve databronnen met behulp van Machine Learning niet gerelateerd aan netwerken van experts en de industrie of toegang tot het bedrijfsmanagement, maar eerder aan het vermogen om grote hoeveelheden data te verzamelen en deze in realtime te analyseren.

Drie trends hebben een revolutie teweeggebracht in het gebruik van data in algoritmische handelsstrategieën en kunnen de beleggingssector verder verschuiven van discretionaire naar kwantitatieve stijlen:
- De exponentiële toename van de hoeveelheid digitale data
- De toename van rekenkracht en dataopslagcapaciteit tegen lagere kosten
- De vooruitgang in Machine Learning-methoden voor het analyseren van complexe datasets
- [Kunnen we de financiële markten voorspellen op basis van zoekopdrachten van Google?](https://onlinelibrary.wiley.com/doi/abs/10.1002/for.2446), Perlin et al., 2016, Journal of Forecasting

## Het ontwerpen en uitvoeren van een Machine Learning-gestuurde strategie

Machine Learning kan waarde toevoegen in meerdere fasen van de levenscyclus van een handelsstrategie en is afhankelijk van belangrijke infrastructuur en dataresources. Dit boek behandelt daarom hoe Machine Learning-technieken passen in het bredere proces van het ontwerpen, uitvoeren en evalueren van strategieën.

Een algoritmische handelsstrategie wordt aangestuurd door een combinatie van alfafactoren die één of meerdere databronnen omzetten in signalen die op hun beurt toekomstige rendementen van activa voorspellen en koop- of verkooporders genereren. 

**Hoofdstuk 2, Markt- en fundamentele data**, en **hoofdstuk 3, Alternatieve data voor de financiële wereld**, behandelen het verzamelen en beheren van data, de grondstof en de belangrijkste drijfveer achter een succesvolle handelsstrategie.
**Hoofdstuk 4, Alfafactoronderzoek**, beschrijft een methodologisch verantwoorde aanpak om het risico op valse positieven te beheersen, een risico dat toeneemt met de hoeveelheid data. 
**Hoofdstuk 5, Strategie-evaluatie**, biedt de context voor de uitvoering en prestatiemeting van een handelsstrategie.

De volgende subsecties beschrijven deze stappen, die we in de rest van het boek uitgebreid zullen bespreken.

### Gegevens verzamelen en beheren

De drastische schematische evolutie van de beschikbaarheid van gegevens in termen van volume, variëteit en snelheid is een belangrijke aanvulling op de toepassing van Machine Learning in de handel, wat op zijn beurt de uitgaven van de sector aan de verwerving van nieuwe gegevensbronnen heeft aangewakkerd. Het steeds groter wordende aanbod aan gegevens vereist echter een zorgvuldige selectie en beheer om de potentiële waarde te ontsluiten, inclusief de volgende stappen:

   1. Identificeer en evalueer markt-, fundamentele en alternatieve gegevensbronnen die alpha-signalen bevatten die niet te snel afnemen.

   2. Implementeer of gebruik een schaalbare cloudgebaseerde data-infrastructuur en **analytische tools zoals Hadoop of Spark** om snelle en flexibele toegang tot gegevens mogelijk te maken.
   
   3. Beheer en selecteer gegevens zorgvuldig om vertekening door vooruitkijken te voorkomen door ze aan te passen aan de gewenste frequentie op een bepaald moment. Dit betekent dat gegevens alleen informatie mogen weerspiegelen die op een bepaald moment beschikbaar en bekend is. Machine Learning-algoritmen die getraind zijn op vertekende historische gegevens zullen vrijwel zeker falen tijdens live trading.

We zullen deze aspecten in detail behandelen in hoofdstuk 2, Markt- en fundamentele gegevens: bronnen en technieken, en hoofdstuk 3, Alternatieve gegevens voor de financiële sector: categorieën en toepassingsvoorbeelden.

### Van alfa-factoronderzoek tot portefeuillebeheer

Alfa-factoren zijn ontworpen om signalen uit data te halen en zo het rendement van activa te voorspellen voor een bepaald beleggingsuniversum over de handelshorizon. Een factor krijgt één waarde voor elk onderdeel/bezit wanneer deze wordt geëvalueerd, maar kan één of meerdere inputvariabelen combineren. Het proces omvat de stappen die in de volgende afbeelding worden weergegeven:

De onderzoeksfase van de workflow voor de handelsstrategie omvat het ontwerpen, evalueren en combineren van alfa-factoren. Machine Learning speelt een grote rol in dit proces, omdat de complexiteit van factoren is toegenomen doordat beleggers reageren op zowel de afname van het signaal van eenvoudigere factoren als de veel rijkere data die tegenwoordig beschikbaar zijn.

Alfa-factoren genereren instap- en uitstapsignalen die leiden tot koop- of verkooporders, en de uitvoering van orders resulteert in portefeuilleposities. De risicoprofielen van individuele posities werken samen om een specifiek portfolio-risicoprofiel te creëren. Portefeuillebeheer omvat het optimaliseren van de positiegewichten om het gewenste portfolio-risico- en rendementsprofiel te bereiken dat aansluit bij de algemene beleggingsdoelstellingen. Dit proces is zeer dynamisch om continu veranderende marktdata te kunnen verwerken.

### Backtesting van strategieën

De integratie van een beleggingsidee in een algoritmische strategie vereist uitgebreide tests met een wetenschappelijke aanpak. Deze aanpak probeert het idee te verwerpen op basis van de prestaties in alternatieve, niet-gesimuleerde marktscenario's. Tests kunnen gebruikmaken van gesimuleerde data om scenario's vast te leggen die mogelijk worden geacht, maar niet terug te vinden zijn in historische data.

## Machine Learning voor trading in de praktijk: strategieën en use cases

In de praktijk passen we Machine Learning toe op trading in de context van een specifieke strategie om een bepaald bedrijfsdoel te bereiken. In dit gedeelte beschrijven we kort hoe handelsstrategieën zijn geëvolueerd en gediversifieerd, en schetsen we praktijkvoorbeelden van Machine Learning-toepassingen, waarbij we benadrukken hoe deze relevant zijn voor de inhoud van dit boek.

### De evolutie van algoritmische strategieën

Kwantitatieve strategieën zijn geëvolueerd en verfijnder geworden in drie fasen:

   1. In de jaren 80 en 90 kwamen signalen vaak voort uit academisch onderzoek en maakten ze gebruik van één of slechts enkele inputs afgeleid van markt- en fundamentele data. AQR, een van de grootste kwantitatieve hedgefondsen van vandaag, werd in 1998 opgericht om dergelijke strategieën op grote schaal te implementeren. Deze signalen zijn nu grotendeels gestandaardiseerd en beschikbaar als ETF, zoals eenvoudige mean-reversion-strategieën.

   2. In de jaren 2000 nam factorbeleggen een enorme vlucht, gebaseerd op het **baanbrekende werk van Eugene Fama en Kenneth French** en anderen. Fondsen gebruikten algoritmes om activa te identificeren die blootgesteld waren aan risicofactoren zoals waarde of momentum om arbitragekansen te zoeken. Terugtrekkingen in de beginfase van de financiële crisis veroorzaakten de kwantitatieve aardbeving van augustus 2007, die zich als een domino-effect door de factorbeleggingssector verspreidde. Deze strategieën zijn nu ook beschikbaar als long-only smart beta-fondsen die portefeuilles kantelen op basis van een bepaalde set risicofactoren.

   3. Het derde tijdperk wordt gedreven door investeringen in Machine Learning-capaciteiten en alternatieve data om winstgevende signalen te genereren voor herhaalbare handelsstrategieën. Factorverval is een grote uitdaging: het is aangetoond dat de extra rendementen van nieuwe anomalieën met een kwart dalen tussen de ontdekking en de publicatie, en met meer dan 50 procent na publicatie als gevolg van concurrentie en verdringing.

Tegenwoordig streven handelaren verschillende doelen na bij het gebruik van algoritmes om regels uit te voeren:
   - Handelsuitvoeringsalgoritmes die gericht zijn op het bereiken van gunstige prijzen
   - Korte termijnhandel die gericht is op het profiteren van kleine prijsbewegingen, bijvoorbeeld door arbitrage
   - Gedragsstrategieën die gericht zijn op het voorspellen van het gedrag van andere marktdeelnemers
   - Handelsstrategieën gebaseerd op absolute en relatieve prijs- en rendementsvoorspellingen

### Toepassingen van ML voor trading

ML haalt signalen uit een breed scala aan markt-, fundamentele en alternatieve data en kan worden toegepast in alle stappen van het proces van algoritmische handelsstrategieën. Belangrijke toepassingen zijn onder andere:
   - Datamining om patronen te identificeren, kenmerken te extraheren en inzichten te genereren
   - Supervised learning om risicofactoren of alfa's te genereren en handelsideeën te creëren
   - Aggregatie van individuele signalen tot een strategie
   - Allocatie van activa op basis van risicoprofielen die door een algoritme zijn geleerd
   - Het testen en evalueren van strategieën, onder andere door gebruik te maken van synthetische data
   - De interactieve, geautomatiseerde verfijning van een strategie met behulp van reinforcement learning

We lichten enkele van deze toepassingen kort toe en geven aan waar we het gebruik ervan in latere hoofdstukken zullen demonstreren.

### Datamining voor feature-extractie en inzichten

De kosteneffectieve evaluatie van grote, complexe datasets vereist het detecteren van signalen op grote schaal. Er zijn diverse voorbeelden in het boek:

   - **Informatietheorie** helpt bij het schatten van de signaalinhoud van kandidaat-features en is daarom nuttig voor het extraheren van de meest waardevolle inputs voor een Machine Learning-model. In hoofdstuk 4, Financial Feature Engineering: How to Research Alpha Factors, gebruiken we wederzijdse informatie om de potentiële waarden van individuele features te vergelijken voor een supervised learning-algoritme om activarendementen te voorspellen. Hoofdstuk 18 in De Prado (2018) schat de informatie-inhoud van een prijsreeks als basis voor het kiezen tussen alternatieve handelsstrategieën.

  - **Unsupervised learning** biedt een breed scala aan methoden om structuren in data te identificeren om inzichten te verkrijgen of een vervolgtaak op te lossen. We geven verschillende voorbeelden:
  
  - In hoofdstuk 13, [Ongecontroleerd leren: Van datagestuurde risicofactoren tot hiërarchische risicopariteit](../13_unsupervised_learning/README.md), introduceren we clustering en dimensionaliteitsreductie om kenmerken te genereren uit hoogdimensionale datasets.
  
  - In hoofdstuk 15, [Onderwerpmodellering voor winstgesprekken en financieel nieuws`](../15_topic_modeling/README.md), passen we Bayesiaanse waarschijnlijkheidsmodellen toe om financiële tekstdata samen te vatten.
  
  - In hoofdstuk 20: [Auto-encoders voor conditionele risicofactoren](../20_auto-encoders_for_conditional_risk_factors), gebruikten we deep learning om niet-lineaire risicofactoren te extraheren, geconditioneerd op activakenmerken, en voorspelden we aandelenrendementen op basis van [Kelly et al. al.](https://www.aqr.com/Insights/Research/Working-Paper/Autoencoder-Asset-Pricing-Models) (2020).

  - **Modeltransparantie**: we benadrukken modelspecifieke manieren om inzicht te krijgen in de voorspellende kracht van individuele variabelen en introduceren een nieuwe speltheoretische benadering genaamd SHapley Additive exPlanations (SHAP). We passen deze toe op gradient boosting machines met een groot aantal invoervariabelen in hoofdstuk 12, Boosting your Trading Strategy en de Appendix.

#### Begeleid leren voor het creëren en aggregeren van alfafactoren

De meest bekende reden om Machine Learning toe te passen op trading is het verkrijgen van voorspellingen over de fundamentele kenmerken van activa, prijsbewegingen of marktomstandigheden. Een strategie kan gebruikmaken van meerdere Machine Learning-algoritmen die op elkaar voortbouwen:

   - **Downstream-modellen** kunnen signalen genereren op portfolioniveau door voorspellingen over de vooruitzichten van individuele activa, verwachtingen van de kapitaalmarkt en de correlatie tussen effecten te integreren.

   - Als alternatief kunnen ML-voorspellingen informatie verschaffen voor **discretionaire transacties**, zoals in de eerder beschreven kwantitatieve benadering.

   -  ML-voorspellingen kunnen ook **specifiek risicofactoren** targeten, zoals waarde of volatiliteit, of technische benaderingen implementeren, zoals trendvolging of regressie naar het gemiddelde.

   - In hoofdstuk 3, [Alternatieve data voor financiën: categorieën en gebruiksscenario's](../03_alternative_data/README.md), illustreren we hoe je met fundamentele data kunt werken om input te creëren voor ML-gestuurde waarderingsmodellen.

  - In hoofdstuk 14, [Tekstgegevens voor trading:sentimentanalyse](../14_working_with_text_data/README.md), 
  
  - hoofdstuk 15, [Onderwerpmodellering voor winstgesprekken en financieel nieuws](../15_topic_modeling/README.md), en 
  
   - hoofdstuk 16, [Betere kenmerken extraheren: woordembedding voor winstgesprekken en SEC-documenten](../16_word_embeddings/README.md), gebruiken we alternatieve gegevens over bedrijfsrecensies die kunnen worden gebruikt om de omzet van een bedrijf te projecteren als input voor een waarderingsoefening.
  
  - In hoofdstuk 9, [Van volatiliteitsvoorspellingen tot statistische arbitrage: tijdreeksmodellen](../09_time_series_models/README.md), laten we zien hoe macro-economische variabelen als input voor marktverwachtingen kunnen worden voorspeld en hoe risicofactoren zoals volatiliteit kunnen worden voorspeld.
  
  - In hoofdstuk 19, [RNN's voor trading: multivariate rendementsreeksen en tekstdata](../19_recurrent_neural_nets/README.md), introduceren we terugkerende neurale netwerken die superieure prestaties leveren met niet-lineaire tijdreeksdata.

#### Vermogensallocatie
ML is gebruikt om portefeuilles te alloceren op basis van beslissingsboommodellen die een hiërarchische vorm van risicopariteit berekenen. Hierdoor worden risicokenmerken bepaald door patronen in activaprijzen in plaats van door activaklassen, wat resulteert in superieure risico-rendementskenmerken.

  - In hoofdstuk 5, [Portfolio-optimalisatie en prestatie-evaluatie](../05_strategy_evaluation/README.md), en hoofdstuk 13, [Ongecontroleerd leren: van data gestuurde risicofactoren naar hiërarchische risicopariteit](../13_unsupervised_learning/README.md), illustreren we hoe hiërarchische clustering data gestuurde risicoklassen extraheert die correlatiepatronen beter weerspiegelen dan de conventionele definitie van activaklassen (zie hoofdstuk 16 in De Prado, 2018).

# Testen van handelsideeën

Backtesting is een cruciale stap bij het selecteren van succesvolle algoritmische handelsstrategieën. Kruisvalidatie met behulp van synthetische data is een belangrijke Machine Learning-techniek om betrouwbare out-of-sample resultaten te genereren, mits gecombineerd met geschikte methoden om te corrigeren voor meervoudige testen. 

Het tijdreekskarakter van financiële data vereist aanpassingen aan de standaardaanpak om look-ahead bias te voorkomen of om de data die gebruikt wordt voor training, validatie en testen op andere wijze te vervuilen. 

Daarnaast heeft de beperkte beschikbaarheid van historische data geleid tot alternatieve benaderingen die gebruikmaken van synthetische data.
We zullen verschillende methoden demonstreren om Machine Learning-modellen te testen met behulp van markt-, fundamentele en alternatieve data die betrouwbare schattingen van out-of-sample fouten opleveren.

In hoofdstuk 21, [Generative Adversarial Networks for Synthetic Training Data](../21_gans_for_synthetic_time_series/README.md), presenteren we generatieve adversariële netwerken (GAN's) die in staat zijn om synthetische data van hoge kwaliteit te produceren.

#### Reinforcement Learning

Handel vindt plaats in een competitieve, interactieve marktplaats. Reinforcement Learning is erop gericht agenten te trainen om een beleidsfunctie te leren op basis van beloningen; het wordt vaak beschouwd als een van de meest veelbelovende gebieden binnen financiële Machine Learning. **Zie bijvoorbeeld Hendricks en Wilcox (2014) en Nevmyvaka, Feng en Kearns (2006) voor toepassingen in de uitvoering van transacties.**

  - In hoofdstuk 22, [Deep Reinforcement Learning: Building a Trading Agent](../22_deep_reinforcement_learning/README.md), presenteren we belangrijke reinforcement learning-algoritmen zoals Q-learning om de training van reinforcement learning-algoritmen voor de handel te demonstreren met behulp van OpenAI's Gym-omgeving.

## Referenties

### Academisch onderzoek

  - [De fundamentele wet van actief beheer](http://jpm.iijournals.com/content/15/3/30), Richard C. Grinold, The Journal of Portfolio Management, voorjaar 1989, 15 (3) 30-37
  
  - [De relatie tussen rendement en marktwaarde van gewone aandelen](https://www.sciencedirect.com/science/article/pii/0304405X81900180), Rolf Banz, Journal of Financial Economics, maart 1981
  
  - [De arbitrageprijstheorie: enkele empirische resultaten](https://onlinelibrary.wiley.com/doi/abs/10.1111/j.1540-6261.1981.tb00444.x), Marc Reinganum, Journal of Finance, 1981
  
  - [De relatie tussen winstrendement, marktwaarde en rendement] [voor gewone aandelen van de NYSE](https://pdfs.semanticscholar.org/26ab/311756099c8f8c4e528083c9b90ff154f98e.pdf), Sanjoy Basu, Journal of Financial Economics, 1982

### Industrienieuws

  - [De opkomst van het kunstmatig intelligente hedgefonds](https://www.wired.com/2016/01/the-rise-of-the-artificially-intelligent-hedge-fund/#comments), Wired, 25-01-2016
  
  - [Crowdsourced kwantitatief netwerk wijst meer dan ooit toe aan één algoritme](https://www.bloomberg.com/news/articles/2018-08-02/crowd-sourced-quant-network-allocates-most-ever-to-single-algo), Bloomberg, 08-02-2018
  
  - [De lessen van Goldman Sachs uit de �quant quake�](https://www.ft.com/content/fdfd5e78-0283-11e7-aa5b-6bb07f5c8e12), Financial Times, 03-08-2017
  
  - [De lessen van de Quant Quake klinken tien jaar later nog steeds door](https://www.ft.com/content/a7a04d4c-83ed-11e7-94e2-c5b903247afd), Financial Times, 18-08-2017
  
  - [Smart beta-fondsen bereiken een vermogen van meer dan $1 biljoen](https://www.ft.com/content/bb0d1830-e56b-11e7-8b99-0191e45377ec), Financial Times, 27-12-2017
  
  - [BlackRock zet in op algoritmes om fondsmanagers te verslaan](https://www.ft.com/content/e689a67e-2911-11e8-b27e-cc62a39d57a0), Financial Times, 20-03-2018
  
  - [Smart beta: wat zit er in een naam?](https://www.ft.com/content/d1bdabaa-a9f0-11e7-ab66-21cc87a2edde), Financial Times, 27-11-2017
  
  - [Computergestuurde hedgefondsen behoren tot de top van de sector](https://www.ft.com/content/9981c870-e79a-11e6-967b-c88452263daf), Financial Times, 01-02-2017
  
  - [Quants domineert Alpha's Hedge Fund 100] Lijst](https://www.institutionalinvestor.com/article/b1505pmf2v2hg3/quants-rule-alphas-hedge-fund-100-list), Institutional Investor, 26-06-2017
  
  - [De kwantitatieve analisten beheersen Wall Street nu](https://www.wsj.com/articles/the-quants-run-wall-street-now-1495389108), Wall Street Journal, 21-05-2017
  
  - ['We nemen geen MBA's aan': De nieuwe winnaars in de hedgefondssector zullen de betere datasets analyseren](https://www.cbinsights.com/research/algorithmic-hedge-fund-trading-winners/), cbinsights, 28-06-2018
  
  - [Kunstmatige intelligentie: Technologie en mens samensmelten](https://www.institutionalinvestor.com/research/algorithmic-hedge-fund-trading-winners/), cbinsights, 28-06-2018
  
  - [Kunstmatige intelligentie: Technologie en mens samensmelten](https://www.institutionalinvestor.com/article/b1505pmf2v2hg3/quants-rule-alphas-hedge-fund-100-list), Institutional Investor, 26-06-2017 ... Oordeel?](https://blogs.cfainstitute.org/investor/2017/09/25/artificial-intelligence-fusing-technology-and-human-judgment/), CFA Institute, 25-09-2017
  
  - [De nieuwe hype in hedgefondsen is 'kwantum'](https://www.bloomberg.com/news/articles/2017-08-25/the-hot-new-hedge-fund-flavor-is-quantamental-quicktake-q-a), Bloomberg, 25-08-2017
  
  - [Robots snoepen van de winst van vermogensbeheerders](https://www.bloomberg.com/news/articles/2017-06-20/robots-are-eating-money-managers-lunch), Bloomberg, 20-06-2017
  
  - [Opkomst van robots: [Inside the World's Fastest Growing Hedge Funds](https://www.bloomberg.com/news/articles/2017-06-20/rise-of-robots-inside-the-world-s-fastest-growing-hedge-funds), Bloomberg, 20-06-2017
  
  - [Toen Silicon Valley naar Wall Street kwam](https://www.ft.com/content/ba5dc7ca-b3ef-11e7-aa26-bb002965bce8), Financial Times, 28-10-2017
  
  - [BlackRock breidt onderzoek naar kunstmatige intelligentie uit](https://www.ft.com/content/4f5720ce-1552-11e8-9376-4a6390addb44), Financial Times, 19-02-2018
  
  - [AQR onderzoekt gebruik van �big data� ondanks verleden twijfels](https://www.ft.com/content/3a8f69f2-df34-11e7-a8a4-0a1e63a52f9c), Financial Times, 12-12-2017
  
  - [Two Sigma stijgt snel naar de top van de kwantitatieve hedgefondswereld](https://www.ft.-om/content/dcf8077c-b823-11e7-9bfb-4a9c83ffa852), Financial Times, 24-10-2017
  
  - [Toen Silicon Valley naar Wall Street kwam](https://www.ft.com/content/ba5dc7ca-b3ef-11e7-aa26-bb002965bce8), Financial Times, 28-10-2017
  
  - [Kunstmatige intelligentie (AI) in de financi�le wereld - zes waarschuwingen van een centrale bankier](https://www.bundesbank.de/en/press/speeches/artificial-intelligence--ai--in-finance--six-warnings-from-a-central-banker-711602), Deutsche Bundesbank, 27-02-2018
  
  - [Fintech: Zoektocht naar een superalgoritme](https://www.ft.com/content/5eb91614-bee5-11e5-846f-79b0e3d20eaf), Financial Times, 20-01-2016
  
  - [Barron�s Top 100 Hedge Funds](https://www.barrons.com/articles/top-100-hedge-funds-1524873705)
  
  - [Hoe high-frequency trading een snelheid bereikte [bump](https://www.ft.com/content/d81f96ea-d43c-11e7-a303-9060cb1e5f44), FT, 01-01-2018

### Boeken

  - [Advances in Financial Machine Learning](https://www.wiley.com/en-us/Advances+in+Financial+Machine+Learning-p-9781119482086), Marcos Lopez de Prado, 2018
  
  - [Quantresearch](http://www.quantresearch.info/index.html) door Marcos L�pez de Prado
  
  - [Quantitative Trading](http://epchan.blogspot.com/), Ernest Chan

### Machine Learning

  - [Machine Learning](http://www.cs.cmu.edu/~tom/mlbook.html), Tom Mitchell, McGraw Hill, 1997
  
  - [An Introduction to Statistical Learning](http://www-bcf.usc.edu/~gareth/ISL/), Gareth James et al.
  
  - Uitstekend naslagwerk voor essenti�le Machine Learning-concepten, gratis online beschikbaar
  
  - [Bayesian Reasoning and Machine Learning](http://web4.cs.ucl.ac.uk/staff/D.Barber/textbook/091117.pdf), Barber, D., Cambridge University Press, 2012 (bijgewerkte versie beschikbaar op de website van de auteur)

### Cursussen

  - [Algorithmic Trading](http://personal.stevens.edu/~syang14/fe670.htm), Prof. Steve Yang, Stevens Institute of Technology
  
  - [Machine Learning](https://www.coursera.org/learn/machine-learning), Andrew Ng, Coursera
  
  - [](http://deeplearning.ai/), Andrew Ng
  
  - Andrew Ng's introductiecursus deep learning

### ML-competities en -handel

  - [IEEE Investment Ranking] Uitdaging](https://www.crowdai.org/challenges/ieee-investment-ranking-challenge)
  
  - [Uitdaging voor het rangschikken van beleggingen: De best presterende aandelen identificeren op basis van hun halfjaarlijkse rendementen](https://arxiv.org/pdf/1906.08636.pdf)
  
  - [Uitdaging voor financieel modelleren met Two Sigma](https://www.kaggle.com/c/two-sigma-financial-modeling)
  
  - [Two Sigma: Nieuws gebruiken om aandelenbewegingen te voorspellen](https://www.kaggle.com/c/two-sigma-financial-news)
  
  - [De Winton-aandelenmarktuitdaging](https://www.kaggle.com/c/the-winton-stock-market-challenge)
  
  - [Uitdaging voor algoritmische handel](https://www.kaggle.com/c/AlgorithmicTradingChallenge)

### Python-bibliotheken

  - matplotlib [docs]( <https://github.com/matplotlib/matplotlib)
  - numpy [docs](https://github.com/numpy/numpy)
  - pandas [docs](https://github.com/pydata/pandas)
  - scipy [docs](https://github.com/scipy/scipy)
  - seaborn [docs](https://github.com/mwaskom/seaborn)
  - statsmodels [docs](https://github.com/statsmodels/statsmodels)
  - [Boosting numpy: Why BLAS Matters](http://markus-beuckelmann.de/blog/boosting-numpy-blas.html)


### PARTS&Chapters from book: Machine Learning for Trading Second Edition by Stefan Jansen
# PART 1 - Data, alfa factors, and portfolios
## Chapter  1 - Machine Learning for Trading - From Idea to Execution
## Chapter  2 - Market and Fundamental Data - Sources and Techniques
## Chapter  3 - Alternative Data for Finance- Categories and Use Cases
## Chapter  4 - Financial Feature Engineering - How to Research Alpha Factors 
## Chapter  5 - Portfolio Optimization and Performance Evaluation

# PART 2 - ML for Trading - Fundamentals
## Chapter  6 - The Machine Learning Proces
## Chapter  7 - Linear Models
## Chapter  8 - The ML4T Workflow
## Chapter  9 - Time-Series Models for Volatility and Statistical Arbitrage
## Chapter 10 - Bayesian ML - Dynamic Sharpe Ratios and Pairs Trading 
## Chapter 11 - Random Forests - A Long-Short Stratigy for Japanese Stocks
## Chapter 12 - Boosting Your Trading Strategy
## Chapter 13 - Data-Driven Risk Factors and Asset Allocation with Unsupervised Learning

# PART 3 - Natural Language Processing
## Chapter 14 - Text Data for Trading
## Chapter 15 - Topic Modeling
## Chapter 16 - World Embeddings for Earnings Calls and SEC Filings

# PART 4 - Deep and Reinforcement Learning
## Chapter 17 - Deep Learning for Trading
## Chapter 18 - CNN's for Finacial Time Series and Satelite Images
## Chapter 19 - RNN's for Multivariate Time Series and Sentiment Analysis
## Chapter 20 - Autoencoders for Conditional Risk Factors and Asset Pricing 
## Chapter 21 - Generative Adversarial Networks for Synthetic Time-Series Data
## Chapter 22 - Deep Reinforcement Learning - Building a Trading Agent
## Chapter 23 - Conclusions and Next Steps

# To get the most out of this book
# The GitHub Repository
# Data Sources
# Anaconda and Docker images
# Download the example code files
# Download the color images
# Conventions used
# Get in touch
# Reviews