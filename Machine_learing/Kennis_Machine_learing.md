Kennens per netwerk
- [x] KNN  
k-Nearest Neighbor.
We hebben data zeg dat we mensen vragen gaan stelen over star wars en star trek.<br />
  aan de hand van de vragen kunnen we verspelen of dat je een star wars fan bent of star trek fan. <br />
  We ploten deze data met wat data van mensen die niet hebben opgegeven wat hun favarieten show is van de twee.
  Als we om die mensen een cirkel teken de word zo grot tot dat K aantal mensen binnen de cirkel vallen 
  laten we zegen dat k=5 dus dan kunnen we de afstant meten tussen de mensen dit kan op verschillenden manieren zie hier onder.
  Aan de data die we door krijgen kunnen zegen hoe veel kans de on bekeden persone per show fan zou zijn en het op deze manier kunnen voor spellen.
  
**Proximity metrics we can use**  

Er zijn meer metrics maar ik ben een soort van lui en deze 3 worde volgens mij het mesten gebruikt
- Euclidean distance<br />
Dit is de defaul metric dat sklearn voor knn gebruikt. Euclidean Disctane is da afstant tussen 2 punten 
  de 2 punten. Als we een dierektenlijn tussen de 2 punten trekken zou de lijn de Euclidean Disctane zijn
  De berekeing here voor is 
wortel van (q1-p1)^2+(p2-q2)^2 =d(p,q)^2 = (q1-p1)^2+(p2-q2)^2 <br />
  
- Hamming distance<br />
De Hamming distance is het verschil tussen 2 strings van de zelften langten.<br />
  het verschil tussen deze strings is de Hamming distance<br />
  Voorbeeld: string 1 ='10110' en string 2 ='10011' de lang van de strings zijn het zelften
   allen van string 1 staat op positsie  2 en 4 zijn anders dus de Hamming distance = 2  
  <br />
  
- chebychev distance<br />
Stel dat we een schaak board hebben met a tot h en 1 tot 8.  
  De koning kan alde kanten op maar kan maar een square per buurt bewegen. De chebychev distance werkt op 
  de zelften manier dus de chebychev distance van A1 en B3 = 2.
  de formulen die we kunnen gebruiken hier voor is. 
  D(x,y) = max(|x2-x1|,|y2-y1|).  
<br />
  
**Voordelen**<br />
- Relatief makelijk te gebruiken om dat je alleende k moet instellen mestal<br />
- efficient voor kleinen dataset<br />

**Nadelen**<br />

- Groten datasets duuren iets van lang<br />
- Je hebt best wel mooien data nodig om over-fitting en under-fitting tegen tegaan<br />

**applications of knn**<br />
  Text mining<br />
Agriculture<br />
Finance<br />
Medical<br />
Facial recognition<br />
Recommendation systems (Amazon, Hulu, Netflix, etc)<br />
<br />

- [x] SVM
Support vector machine.  
  
Een lineaire scheiding aan die de twee klassen zo goed mogelijk van elkaar scheidt (die scheiding is een hypervlak; in twee dimensies is het een rechte lijn).  
  Nadien kan de SVM dan voor een nieuw te klasseren object beslissen tot welke klasse het behoort door te kijken langs welke kant van het hypervlak het corresponderende punt in de ruimte ligt.   

**Use cases**  
  For het onderscheidend van groepen of classes.  

**Voordelen**    

  Veel features, Hoge accuraatheid<br />

**Nadelen**<br />

er is niet altijd een mooie lijn te vinden die de groepen perfect scheidt. <br />

Vers is het ook minder geschikt voor dataset met veelk ruis, om dat ruis er voor kan zorgen dat datapunten van verschilende groepenmet elkaar
overlappen en doorkruisen.

  <br /> 
    
- [x] Naive Bayes  
Naive bates is een "Probabilistic classification" het model kijk hoe groot de kans is om bijvoorbeeld naar het starand te gaan.
  De formullen die we gebruiken is als volgt Ck = de class bijvoorbeeld: is het zoning.  
  x = de features en P staat voor de probability.  
  p(ck|X)[posterior probability]=(P(x|ck) [Likelihood] P(c)[classprior probability])/ P(x)[predictor prior probability]  
  Uit eindelijk krijgen we een helen langen berekeing waar in de probability van all de mee gegeven class bij elkaar worden vermenigvuldigd.  
  Waar uit kome 2 procenten een van hoe groot de probability is dat ik naar het strand zou gaan of niet welken het   
  grotsten is geeft het model dan aan.
    

**Voordelen**    
- het presteert goed in het geval van categorische invoervariabelen in vergelijking met numerieke labels
- Het is snell  
- Kan goed om gaan met multy class  

**Nadelen**<br />
- Naive bayes gaat er van uit dat all de categorische het zelften gewicht hebben. Dit is niet altijd waar   

**Use cases**  
-  Real time prediction om dat het so snel is.  
-  spam filtering  

   
- [x] Logistic Regression    
  Logistic Regression is een supervised learning algorithm dit word gebruikt om classification problems op telossen.  
  Logistic Regression is een model dat de logistic function squeeze de uitgang van een linear.

  **gebruik**<br/>
  Bij data senst waar dood vs levend of rooker of geen rooker etc. Vorspelt moeten worden daar is dit model goed in.<br/>
  - mail is spam of geen spam
  
  **Voordelen**<br/>
  - Doet het bezonder goed op binary problems

  **nadelen**
  - Logistische regressie probeert te voorspellen resultaten op basis van een aantal onafhankelijke variabelen, maar logit modellen zijn kwetsbaar voor zelfoverschatting. Dat wil zeggen, kunnen de modellen lijken te hebben meer voorspellende kracht dan ze eigenlijk doen als gevolg van sampling bias.(Overfiting) <br/>

  - Kan alleen maar for binary problemen worden gebruikt.
  - is gevoeling voor ruis
  - Hoge corr is niet altijd het besten om dat de kans grooter word dat het gaat overfitten.

  ![for](https://wikimedia.org/api/rest_v1/media/math/render/svg/5ce173b2e22cfa635a86b1af3ea0c3eb0641cb88)<br/>
  Hier zijn Xi1 xik de onafhankelijke variabelen is β0 de constante en zijn de βn de logistiche regressiecoëfficiënten.
- [x] Decision Tree(s)  
Een Decision Tree is niet meer dan een flow chart die het algeritme heeft gemaakt. Hij kan er als volgt uit zien om bij voor belt het geslacht te vorspelen.
  waar bijvoorbeeld een van de featers is lengten manenen zijn in het algemeen langer dan vrouwen. Dus als we een onbekenden hebben en we weten dat dezen on der het trase hold voor de man is dan is het waarschijnlijk een vrouw.
  Dit is maar een voorbeeld normaal zouden we veel meer featers hebben en kan zou tree aarding in gewilkeld worden.<br /> 
  
**Voordelen**<br />
- Werkt ook goed met non-linear relationship.  

**Nadelen**<br />
- Zijn heel gevoeling en kunnen makelijk veranderen als he een klein variantie op de data doen.(variance)   
- Makelijk om te over fitten (Greedy)
- Om een goede tree te maken heb je een gebalanseerden dataset noding.   
  <br />  
     
- [x] Random Forest

In Random forest maken we meerderen bommen.   
  Elken boom is iets anders het als we bijvoorbeeld: Een soort fruit willen herkennen kan krijgen aan de bomen een wat we weten over dat fruit.
  door 'Majority voting' kijken we op welk fruit het meesten is gestempt. Dan het dan kiest het model die dat fruit.
  
**Voordelen**<br />
- kan classificatie- en regressietaak  
- Kan nog steets een hoggen accuracy hebben zelfs met missing data.
- Je moet echt je best doen als he het will een model wilt overfiten. 
- Kan groten data sets met veel opsies aan.  

**Nadelen** <br />  
- is niet zo goed in regrassietaaken als hij is in classificatie
- Je hebt geen controlen over het model met what hij doen met de data.
- Overfit  kan geburen als je te veel 'noise' hebt in een dataset.  

  
- [x] Performance measures  
  Er zijn verschillenden manieren om te kijken hoe goed je model werkt.  
  
  
   - Classification Accuracy  
  Dit is de meest gebruikten manier. acc = (correct prediction/nummber of predictions) *100  


   - ROC curve  
    Is een plot dat The true possitve rate tegen de fals positve rate plot  
     Here me kunnen we dus snel zien hoe goed ons model werkt en hoe veel erros er zijn.  
     als we alleen maar fals posjtve krijgen weten we dat we ons model moeten verandern of kijken of onze data wel good is.  
     
     
  
  
- [x] ROC curve
  
- [x] Clustering  
  Is een unsupervised learning method. Clustering is de data punten die dicht bijmakaar staan in groepen verdelen.Dus een groep bestaat uit data punten die om makaar lijken.  
  Er zijn meerderen methodes voor het gebruik van clustering:  
  - Density-based   
    Deze methoden beschouwen de clusters als het dichte gebied dat enige gelijkenis vertoont en verschilt van het lagere 
    dichte gebied van de ruimte.  
    Deze methoden hebben een goede nauwkeurigheid en het vermogen om twee clusters samen te voegen.  
      
  - Hierarchical based  
    De clusters die bij deze methode worden gevormd, vormen een boomachtige structuur op basis van de hiërarchie.   
    Nieuwe clusters worden gevormd met behulp van de eerder gevormde. Het is onderverdeeld in twee categorieën  
    Agglomeratief (bottom-up benadering).  
    Verdeeld (top-down benadering).  
    
  - partitioning     
  Deze methoden verdelen de objecten in k clusters en elke partitie vormt één cluster. Deze methode wordt gebruikt om een ​​objectieve criteriumovereenkomstfunctie te optimaliseren,   
    zoals wanneer de afstand een belangrijk parametervoorbeeld K-betekent
    
  - Grid-besed  
Bij deze methode wordt de dataruimte geformuleerd in een eindig aantal cellen die een rastervormige structuur vormen. Alle clusteringbewerkingen die op deze rasters worden uitgevoerd,   
zijn snel en onafhankelijk van het aantal gegevensobjecten  
    
- [x] Regressie  
  Regressien analysis een een manier om de relatsie tussen je target en je voorspeling variabelen.  
  Die aan meerderen variabelen af hangen. Dus even kort gezegt en duidelijk  een regrassie analysis  
  laat meestal duidelijk zien hoe een variabelen die af hangt van andere   
  variabelen verandert na reactie van een independent variabelen.
  

  
- [x] Supervised learning  
  Is als een model iets moet leren waar het antwoord al bekent bij is bij de train data.  
  
   
- [x] Unsupervised learning  
  Unsupervised learning is een metoden waar in we datasets zonder labelled response hebben.  
  Dus als we bijvoor beeld afbeldingen laat zien van een hond en een cat zonder te zegen wat het zijn.  
  zou het model na een tijd kunnen zegen wat een hond en een cat is maar dat zou het dan kunnen herkenen aan features  
  bijvoorbeeld lengte, gewicht , vorm.  
- [x] Cross validation   
  Cross validation is data we all onze data opdelen in stukjes een van fold = aantal_opsplitingen.  
  dus laten we zegen dat ik mijn data in 4 splits dan heb ik 4 folds.  
  Voor de eersten split zou dan de eerste fold de test data worden en de rest de train.  
  Voor de tweede split zou dan fold 2 de test worden en de rest de train enzo voored.  
  
  
- [x] Overfitting, underfitting   
 Overfitting  
  Overfiting gebeurt als je uit komt te goed is dat het eigenlijk niet zou kloppen.  
  Dit kan je controleren door nieuwe het model op nieuwe data te testen dat niet   
  op de data lijkt waar op je het hebt getraint maar de zelften relatie heeft met elkaar.  

  Underfitting  
  Underfitting gebeurt wanneer een model niet complex genoeg is waar door het de relatie tussen  
  features en target niet te zien is. Het resotaat heer van is dat het mode het vaak niet goed doet op nieuwe   
  data en vaak ook niet goed werkt op de train data zelf.  
  
    
- [ ] Kiezen van de juiste methode
  
- [ ] Ensemble methods



