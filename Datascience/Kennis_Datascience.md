kennis file
- [x] Scatter Matrix  
  Zijn meerderen gravieken waar 2 variabelen tegen elkaar worden geplot  
  
- [x] Data-aquisitie  
  Is het verzamelen van gegevens, in datasets kun je zomingen column extra data uit krijgen bijvoorbeeld:  
  Laten we zegen dat ik in een column de stroomsterkte bijhou en in een anderen column de spanning  
  (U x I = P) door deze data met elkaar te medevuldingen krijgen we het vermogen berekkenen.  
  Dus hebben we data die we eerst niet hadden nu well.
  

- [x] Dataselectie, opschoning
  
- [x] Visualisatie, interpretatie data
Gebruik gemnaakt van [ploty](https://plotly.com/). <br />


  
- [x] Correlatiematrix(Pearson)  
Een correlatiematrix heeft een ranges van 1 tot -1.  
  Een 1 betekent dat de lineaire vergelijking relatsie tussen x en y het zelften is.  
  Een 0 betekent dat de geen correlation is tusssen x en y.  
  Een -1 betekent dat het om gedrijden van 1 is dus als bijvoorbeelt Y-1 krijgt dan heeft X+1.  
  
 Dus aan de hand van een correlatie matrix kunnen we snel correlaties tussen column zien.  
Dit is een manier om het te doen in python  
`sns.heatmap(data[data.columns[data]].corr(),annot=True,cmap='RdYlGn')`  
`fig=plt.gcf()`  
`fig.set_size_inches(12,10)`  
`plt.show()`  
berekkenen
![png](https://hulpbijonderzoek.nl/wp-content/upload_folders/hulpbijonderzoek.nl/2015/03/pm-corr-formule-21-452x135.jpg?v=1522531647356)
- [ ] Normaliseren
