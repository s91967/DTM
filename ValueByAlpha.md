# Value By Alpha Maps in QGIS

## Datenquelle (Waahlgeometreien & Wahlergebnisse)
[Bundestagswahl 2021](https://www.bundeswahlleiterin.de/bundeswahlleiter.html)

Tabelle (kergl.csv) mit Wahlergebnissen bereinigen 
![image](https://github.com/s91967/DTM/assets/134683996/aeac85db-6382-48c8-9d45-2da39003ed53)

## QGIS 

1.) Vergleich der Parteien SPD und CDU: Stimmenstärkere Partei regelbasiert darstellen

Regel Olaf
```
 "SPD" > "CDU"
```
Regel Armin
```
 "CDU" >  "SPD" 
 ```
 
 2) Ebene Alpha ergänzen und auf Symbolebene 1 setzen
 ![image](https://github.com/s91967/DTM/assets/134683996/a787c433-bfc7-4520-8614-9b0ee622cb6a)

3.) Regel für Ebene 'Alpha': Über "Einfache Füllung" unter "Füllfarbe"  > "Datendefinierte Übersteuerung" > "Bearbeiten" 
```
```

![image](https://github.com/s91967/DTM/assets/134683996/7d51c638-0db7-4434-b0f5-36dcbf134932)

Grundprinzip:

```
set_color_part (
'black',
'alpha', 
126)
```

4.) Statt einem festen Alpha Wert, wird dieser wertebasiert aus einem anderen Attribut für jede Bezugseinheit berechnet 
```
```
![image](https://github.com/s91967/DTM/assets/134683996/239b0ee9-cfa0-41a9-88f5-1a8b719839cb)

5.)
```
```
![image](https://github.com/s91967/DTM/assets/134683996/fb8c3b17-7057-4faf-a296-e97bda3cd4b7)


