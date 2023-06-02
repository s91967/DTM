# DTM

Schritt zur Darstellung der Farben

BIP
```
CASE
WHEN "Logged GDP" > 10.2  THEN 3
WHEN "Logged GDP" > 9.1 THEN 2
ELSE 1
END
```

Freedom
```
CASE
WHEN "Freedom to" > 0.852 THEN 'C'
WHEN "Freedom to" > 0.76 THEN 'B'
ELSE 'A'
END
```

Verknüpfung beider Elemente 
```
"BIP_recl" || "F_recl"
 ```
 
 Farben abgreifen über Photoshop, indem man Muster einfügt oder über den Browser
 
