# MYSQL-BASIC-TAAK-03

## SELECT rekenen met SQL  

## Uitleg

Bij de vorige taak kon je al veel vragen over de gegevens in de database beantwoorden. En als je zou willen deze ook in een applicatie tonen aan de gebruikers. Toch zijn er misschien nog meer vragen die je na het werken met de `fifa2018` database zou willen beantwoorden. Wat verdienen de spelers bij Ajax in totaal per maand? Hoeveel zijn ze gemiddeld waard volgens de FIFA? Of welke club betaald het beste of welke speler verdient het meest?

Nu kun je natuurlijk wat gegevens ophalen en daarna een berekening uitvoeren met bijvoorbeeld PHP maar SQL heeft zelf ook allemaal functies om berekeningen te doen. Deze worden dan uitgevoerd op de database server. Vaak is het handig om de gegevens die je ophaalt uit de database zo terug te krijgen dat ze meteen binnen je applicatie getoont kunnen worden.

SQL kent hiervoor een aantal handig functies:
Functie | Doel
--- | ---
Count() | Telt het aantal rijen die een SQL query teruggeeft
AVG() | Geeft een gemiddelde van de inhoud van een kolom met getallen
SUM() | Telt de inhoud van een kolom met getallen bij elkaar op
Min() | Geeft de kleinste waarde terug in een kolom
Max() | Geeft de grootste waarde terug in een kolom

Hoe maak je nu gebruik van deze functies? Bijna op dezelfde manier als dat je een functie in Javascript of PHP gebruikt. Stel dat we van de `fifa2018` het gemiddelde inkomen van alle spelers bij Ajax willen weten dan kunnen we de onderstaande query schrijven:
```SQL
SELECT AVG(wage) FROM players WHERE club = "Ajax"
```
De WHERE clausule blijft dus hetzelfde, die geeft alleen maar aan dat je alleen de rijen wilt hebben waarvan de waarde "Ajax" is in de `club` kolom. Je voert de rekenkundige functies dus altijd uit op een bepaalde kolom.

Wat je dan terugkrijg als je deze query uitvoert ziet er als volgt uit:

AVG(wage) | 
--- |
9034.4823 |

Het gemiddelde inkomen van de spelers ligt dus rond de 9000 duizend. 

De syntax is als volgt:
```SQL
SELECT functie(kolom) FROM tabel_naam WHERE conditie AND/OR conditie
```




## Leerdoelen

1. Ik kan de `Count()` functie gebruiken om het aantal
   
## Opdracht

1. We maken weer gebruik van de `Fifa2018` database. Als je deze nog niet hebt staan in PhpMyAdmin maak dan een nieuwe database aan (met een duidelijke naam, bv. `mod-mysql-basic-fifa2018`) en import het `.sql` bestand in de `db-export` map van deze taak.
2. Open het SQL tabblad in PhpMyAdmin en schrijf SQL queries om de gevraagde gegevens te tonen:  
   **(vergeet niet na elke beantwoorde vraag de SQL statement die je geschreven hebt te copy/pasten in `antwoorden.sql` en een bookmark met een logisch genaamd label aan te maken)**

Schrijf voor de onderstaande vragen een SQL query die de vraag beantwoord.

1. 


## Eindresultaat

 

## Bronnen

Een lijstje van links naar externe bronnen
> Bijvoorbeeld:  
>[W3 Schools - PHP Functions](https://www.w3schools.com/php/php_functions.asp)  
>[Jaap van der Veen - PHP Basiscursus Les3: Functies](https://phpbasis.jaapvdveen.nl/basiscursus-php/les-3-inleiding-functies/)  
