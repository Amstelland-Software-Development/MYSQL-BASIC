# MYSQL-BASIC-TAAK-02

## SELECT WHERE

## Uitleg

In een voorgaande taak heb je geleerd hoe je met het SELECT en FROM keyword de gegevens van één of meerdere kolommen van een tabel uit de database haalt.

Vaak wil je echter niet alle rijen uit een tabel halen maar juist alleen diegene die voldoen aan een bepaalde voorwaarde, bijvoorbeeld als we de `worldhappiness` database nemen alleen de landen uit een bepaalde regio of de landen met een score boven de 7000.

Je gebruik hiervoor het `WHERE` keyword.

### WHERE Clausule

Binnen een SQL statement noem je het WHERE gedeelte ookwel de WHERE clausule of WHERE *clause* in het engels.

De SQL syntax is als volgt:
```SQL
SELECT kolom1, kolom2, ... FROM tabel_naam WHERE conditie
```
Net als in andere programeer talen waarbij je een conditie gebruikt bij een if/else statement kun je die ook gebruiken met SQL. Het werkt in principe hetzelfde, stel we nemen de onderstaande tabel die een aantal rijen bevat van de `worldhappiness` database.
   country | region | rank | score |
   --------| -------| -----| ------|
   Switzerland | Western Europe | 1 | 7587 |
   Iceland | Western Europe | 2 | 7561 |
   New Zealand | Australia and New Zeeland | 9 | 7286|

De SQL statement `SELECT * FROM jaar2015 WHERE country="Iceland"` geeft het volgende terug:
   country | region | rank | score |
   --------| -------| -----| ------|
   Iceland | Western Europe | 2 | 7561 |

En de SQL statement `SELECT * FROM jaar2015 WHERE rank=1` geeft dus:
   country | region | rank | score |
   --------| -------| -----| ------|
   Switzerland | Western Europe | 1 | 7587 |

Klinkt logisch toch? Mischien zie je al hoe je dus condities schrijft maar nog even voor de duidelijkheid wat staat er nu in gewone taal bij een SQL statement met een WHERE clausule?

Taal | SELECT statement | Keyword | kolom naam | operator | waarde |
----|---------|----------|---------|---------- | ---- | --- | --- | --- |
SQL | `SELECT * FROM jaar2015` | WHERE | country | = | "Iceland" 
Vrij vertaald: | Geef mij alle kolommen van de tabel jaar2015 | waar | de inhoud van de kolom country | gelijk is aan | de string "Iceland"

Of nog even het tweede voorbeeld:

Taal | SELECT statement | Keyword | kolom naam | operator | waarde |
----|---------|----------|---------|---------- | ---- | --- | --- | --- |
SQL | `SELECT * FROM jaar2015` | `WHERE` | rank | = | 1 |
Vrij vertaald: | Geef mij alle kolommen van de tabel jaar2015 | waar | de inhoud van de kolom rank | gelijk is aan | het getal 1



Je kan behalve de `=` operator ook de andere operators die je al kent gebruiken: `<` `>` maar ook `>=` en `<=`. Zie onderstaande tabel:

Operator SQL | Betekent | Operator Javascript
--- | --- | --- |
`=` | Is gelijk aan | `==` |
`>` | Is groter dan | `>` |
`<` | Is kleiner dan | `<` |
`>=` | Is groter of gelijk aan | `>=` |
`<=` | Is kleiner of gelijk aan | `<=` |
`<>` *of* `!=` | is niet gelijk aan | `!=`

> LETOP! Er is wel één heel duidelijk verschil met de condities zoals je die kent bij Javascript en PHP: je gebruikt binnen een SQL statement **nooit** `==` 

En net als bij andere programmeer talen kun een getal schrijven zonder aanhalingstekens maar moet je als je binnen een conditie een string vergelijkt wél aanhalingstekens gebruiken.


## Leerdoelen

1. [ ] Ik kan specifieke rijen ophalen uit een database door een WHERE clausule toe te voegen aan een SQL select statement.
2. [ ] Ik kan een conditie schrijven die gebruikt word binnen een WHERE clausule.

## Opdracht

1. Open PhpMyAdmin in je browser en selecteer de `worldhappiness` database die je bij de vorige taak hebt aangemaakt. (als je deze database nog niet hebt aangemaakt doe dit dan en import het sql export bestand uit de `dp-export` map daarin).
2. Open het SQL tabblad in PhpMyAdmin en schrijf SQL queries om de gevraagde gegevens te tonen:  
   **(vergeet niet na elke beantwoorde vraag de SQL statement die je geschreven hebt te copy/pasten in `antwoorden.sql` en een bookmark met een logisch genaamd label aan te maken)**

> LETOP! Gebruik gewoon SELECT * FROM bij deze eerste opdrachten
1. **Opdracht**: Schrijf een SQL statement die het land uit 2015 toont dat op de 7de plek stond dat jaar. 
2. **Opdracht**: Schrijf een SQL statement die de rank toont van nederland in 2016.
3. **Opdracht**: Schrijf een SQL statement die de score toont van nederland in 2015.
4. **Opdracht**: Schrijf een SQL statement die de score toont van nederland in 2016.
5. **Opdracht**: Schrijf een SQL statement die alleen alle landen in de regio Noord Amerika in 2015 toont.

Je krijgt bij bovenstaande opdrachten telkens alle kolommen terug, dus een hele rij met informatie terwijl je soms alleen een specifieke kolom terug wilt hebben. Je kunt dit doen door ipv `*` de kolomnamen aan te geven gescheiden door een `,`

6. **Opdracht**: Schrijf een SQL statement die *alleen* de naam van het land teruggeeft met een rank van 25 in 2016.
7. **Opdracht**: Schrijf een SQL statement die *alleen* de namen terug geeft van alle landen met een score groter dan 7087 in 2016.
8. **Opdracht**: Schrijf een SQL statement die *alleen* de namen van de landen en de regio toont van de landen met een rank kleiner of gelijk aan 5 in 2016.
9.  **Opdracht**: Schrijf een SQL statement die *alleen* de score toont van Ierland in 2015.
10. **Opdracht**: Schrijf een SQL statement die *alleen* de namen van de landen in de regio latijns amerika en het caribisch gebied in 2016. 

## Eindresultaat

Kijk goed of het resultaat dat je terug krijgt wel voldoet aan de opdracht. Als er staat schrijf een SQL statement die *alleen* dit of dat toont dan is het ook de bedoeling dat je geen onnodige andere gegevens terugkrijgt bij het uitvoeren van de query.

## Bronnen
[W3 Schools - SQL WHERE Clause](https://www.w3schools.com/sql/sql_where.asp)  
[W3 Schools - SQL SELECT Statement](https://www.w3schools.com/sql/sql_select.asp)  

