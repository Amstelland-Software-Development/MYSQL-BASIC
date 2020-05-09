# MYSQL-BASIC-TAAK-01

## Werkwijze

## Uitleg

Als het goed is heb je Xampp al geinstalleerd en weet je hoe je de database server (MySQL) opstart. Daarnaast weet je hoe je de web server binnen Xampp (Apache) opstart zodat je gebruik kan maken van PhpMyAdmin.

## Leerdoelen

1. [ ] Ik kan via het Xampp Controlepaneel de MySQL database server opstarten
2. [ ] Ik kan via het Xampp Controlepaneel de Apache web server opstarten
3. [ ] Ik kan PhpMyAdmin openen in een browser
4. [ ] Ik kan een export van een database importeren in een nieuwe database in PhpMyAdmin.
5. [ ] Ik kan een SQL query uitvoeren in PhpMyAdmin
6. [ ] Ik kan een uitgevoerde SQL query bookmarken in PhpMyAdmin

## Opdracht

1. [ ] Start via het Xampp Controlepaneel MySQL en Apache op.
2. [ ] Ga in je browser naar [http://localhost/phpmyadmin ](http://localhost/phpmyadmin/)
3. [ ] Maak een nieuwe database aan. 
   > Je zal veel verschillende databases aanmaken dus het slim om een logische naam te kiezen zodat je het overzicht behoudt. Noem de database voor deze taak: `mod_mysql_basic_imdb_movies`.  
4. [ ] Selecteeer je nieuwe database: als het goed is zie je de onderstaande regel staan boven in PhpMyAdmin: ![](img/db-selected.jpg)
5. [ ] We gaan nu een export van de database importeren in de nieuw aagemaakte database. Voor je dat doet, open het bestand `imdb_movies.sql` dat in de `db-export` map staat bij deze taak in VS Code en bekijk de inhoudt. 
    > Het ziet er misschien ingewikkeld uit en er zijn veel termen die misschien niet duidelijk zijn maar als je goed kijkt zie je wel zien dat er een tabel wordt aangemaakt (CREATE TABLE) en dat er gegevens in die tabel worden gezet later (INSERT INTO). Deze code is letterlijk de SQL code die wordt uitgevoerd als je de datbase importeert.

6. [ ] Importeer de database: kies uit het menu de knop `Import` en dan in het scherm dat wordt geladen `Choose File` en selecteer het bestand `imdb_movies.sql` in de `db-export` map en kies `Go`.  
   ![PhpMyAdmin bookmark query](img/phpmyadmin-options-import.jpg)  

    > Als het gelukt is dan zie je dat bovenaan staan: Import has been succesfully finished... (imdb_movies.sql) Als je foutmeldingen krijgt: kijk of je database waarin je gaat importeren wel hebt geselecteerd.
1. [ ]  We gaan nu een eerste SQL query uitvoeren en gegevens ophalen uit de database. Kies uit het menu de optie `SQL`.
![PhpMyAdmin bookmark query](img/phpmyadmin-options-sql.jpg)  

2. [ ]  Je ziet een code venster waarin je SQL code kan schrijven. Schrijf de ondestaande SQL code in dat venster: (als er al iets staat haal dit dan weg)   
   ```SELECT * FROM movies ``` 

   klik op de `Go` knop rechtsonder om de query uit te voeren.

3.  [ ] Als het goed is krijg je een overzicht van de inhoud van de tabel `movies` te zien. Om nu te laten zien dat je de taak hebt volbracht doe je het volgende:
    Copy/Paste de gemaakte query is het `antwoorden.sql` bestand op regel 2 en sla deze op. 
4.  [ ] Als laatste onderdeel van deze taak gaan we de query bookmarken. 
    > Dit is handig voor als je dezelfde query nog een keer wilt gebruiken maar is ook de manier om snel een querry op te halen zodat je deze met een docent kan bespreken.
    
> **LETOP!** Een docent kan je vragen om de querries in je bookmarks te laten zien, zorg er dus voor dat je elke query opslaat in je bookmarks en gebruik een logische naam voor de label van de query.

11. [ ] Voer bij de het invulveld label de volgende naam in: `mod-mysql-basic-taak01` in en klik op de `Bookmark this SQL query` knop.  
![PhpMyAdmin bookmark query](img/bookmark-query.jpg)


## Eindresultaat



## Bronnen

Een lijstje van links naar externe bronnen
> Bijvoorbeeld:  
>[W3 Schools - PHP Functions](https://www.w3schools.com/php/php_functions.asp)  
>[Jaap van der Veen - PHP Basiscursus Les3: Functies](https://phpbasis.jaapvdveen.nl/basiscursus-php/les-3-inleiding-functies/)  
