# MYSQL-BASIC-TAAK-01

## Een eerste query

## Uitleg

In deze taak gaan we voor het eerst echt oefenen met SQL! 

Een simpel SQL statement (ookwel query) zoals `SELECT * FROM movies;` is opgebouwd uit SQL keywords en de namen van kolommen en tabellen die je wilt ophalen. Je gebruikt het SELECT keyword om gegevens op te halen. Je kunt de bovenstaande SQL statement als volgt interpreteren: Geef mij de informatie uit alle kolommen van de tabel movies.

Taal | Keyword | kolommen namen | keyword | tabel naam | 
----|---------|----------|---------|---------- |
SQL | `SELECT` | `*`  | `FROM`  | `movies;`  
Vrij vertaald: | Geef mij  | alle kolommen | van de tabel | movies

> LETOP! We gebruiken voor alle SQL code die we schrijven de volgende conventies:  
1. Net als bij andere programmeer talen sluit je elke regel code af met `;`
2. SQL keywords zoals `SELECT` en `FROM` schrijf je in hoofdletters.

> PhpMyAdmin is heel vergevingsgezind en zal het toelaten dat je SQL keywords in kleine letters schrijft of een `;` vergeet aan het einde van je SQL statement maar net als inspringing in je code zorgt het aanhouden van deze conventies voor leesbaardere code en vermijdt je fouten als je straks met PHP SQL code gaat uitvoeren.

Zoals je bij het bovenstaande voorbeeld misschien al bedacht had kun je ook aangeven in je SQL statement dat je niet *alle* kolommen maar alleen *bepaalde* kolommen terugkrijgt. Je doet dit door de namen van de kolommen op te geven gescheiden door een `,`

in onderstaand voorbeeld worden de kolommen genaamd `title` en `rating` opgehaald uit de tabel `movies`.
```sql
SELECT title, rating FROM movies
```

## Leerdoelen

1. [ ] Ik kan 

## Opdracht

1. [ ] We gebruiken een nieuwe database export genaamd `mod-mysql-basic-worldhappiness.sql`. Deze vind je in de `db-export` map.
2. [ ] Om te beginnen open PhpMyAdmin in je browser, maak een nieuwe database aan (noem deze `mod-mysql-basic-worldhappiness`) en importeer het `.sql` bestand. Vergeet niet de database eerst te selecteren voor je de import doet.
3. [ ] Open het SQL tabblad in PhpMyAdmin en schrijf SQL queries om de onderstaande vragen te kunnen beantwoorden:   
   **(vergeet niet na elke beantwoorde vraag de SQL statement die je geschreven hebt te copy/pasten in `antwoorden.sql` en een bookmark met een logisch genaamde label aan te maken)**
   1. [ ] 

## Eindresultaat

Duidelijk maken hoe het succesvol maken van de taak eruit ziet. Dit kan tekstueel of liever als mogelijk met gebruik van screenshots / filmpjes  
> Voorbeeld:  
> Als je de functie goed uitvoert wordt de volgende tekst getoond in je browser: "functie uitgevoerd"  

## Bronnen

Een lijstje van links naar externe bronnen
> Bijvoorbeeld:  
>[W3 Schools - PHP Functions](https://www.w3schools.com/php/php_functions.asp)  
>[Jaap van der Veen - PHP Basiscursus Les3: Functies](https://phpbasis.jaapvdveen.nl/basiscursus-php/les-3-inleiding-functies/)  
