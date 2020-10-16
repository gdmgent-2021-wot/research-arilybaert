# iPhone App
Na ons onderzoek naar RFID en NFC was het tijd om de tags uit te testen 
Eerst hebben apps voor op de iphone gebruikt. Deze waren heel gebruiksvriendelijk. We konden gemakkelijk een tag lezen. 
Hiermee konden we ook gemakkelijk verschillende zaken zoals bv tekst, url, gsm nummer naar een tag schrijven.
Maar niet alle tags werkten met de applicatie. Dit kan liggen aan het feit dat de app voor nfc tags is en de andere mss RFID tags zijn → dit staat niet op de tag. 

## Windows reader
Daarna hebben we allebei ook de reader aangesloten op windows laptop, aangezien deze enkel werkt met windows. 
Bij het aansluiten van de reader werd er automatisch een software gedownload om de reader in werking te stellen.
Om te checken of de reader werkte hebben we via notities de tags proberen lezen → bij het lezen van de kaart kwam er een id tevoorschijn, dit kan je zien op de bovenste foto. 
De andere tags werken niet → kan ook zijn omdat het geen RFID is of omdat de tag niet werkt. 

## GUI-software voor de Windows-reader
Nu we hebben vastgesteld dat de reader werkte zijn we opzoek gegaan naar de bijbehorende software voor deze reader. Als je op de sites kijkt waar deze worden aangeboden kan je zien dat het voornamelijk wordt gebruikt met IDRW en IDRW-3. Deze bijde varianten hebben we dan gedownload. Jammer genoeg konden we geen van beide varianten aan de praat krijgen. Noch voor het lezen noch bij het schrijven. Het apparaatje piept als hij in contact komt met een tag maar dit gebeurde niet.

## Alternatieve scripts
Gezien alle software die we online kunnen vinden niet werkte met de lezer, noch voor het lezen, noch voor het schrijven. Zijn we opzoek gegaan naar een alternatief. Dit leidde ons naar een Github repo van een gebruiker die alle Windows software had omgezet naar een Python Script om het zo werkend te krijgen. Nu ik er zo op terugkijk hadden we kunnen zien aankomen dat het niet ging werken gezien de software waarop het gebaseerd was niet functioneerde maar toch. De software herkent de lezer wel maar gaf ons nooit het gewenste respons

## A New Hope
Vorige week kregen we dan een NFC-lezer voor de Raspberry PI. Aangezien al onze vorige opzoekingen niet werkten, zijn we beginnen zoeken naar documentatie hierover, hopende dat we hiermee wel iets zouden kunnen schrijven naar de nfc tags.

## Bijhorende software
Als eerste hebben we een software van nxp geïnstalleerd op onze Raspberry Pi. Bij het installeren kregen we geen errors dus we dachten dat het deze keer wel ging werken. Maar in onze terminal bleef er staan “waiting for tag or device…” ook al legden we er verschillende tags op.

## Alternatieve scripts
Gezien de meegeleverde software niet werkte zijn we beginnen kijken naar alternatieven. Zo zijn we terecht gekomen op de Github van een zeker Tom. Deze stelde een soort schil rond de originele software beschikbaar. Geschreven in python zodat het gemakkelijk te gebruiken is met een Raspberry. Jammer genoeg hebben we die ook niet werkend gekregen. Het is lastig om het precieze probleem te lokaliseren gezien je moeilijk kunt nagaan of de randapparatuur werkt of juist is aangesloten, er is geen lichtje dat brand of geluidje die afspeeld. Ook kregen we geen errors te zien in onze terminal, dus zo konden we het probleem ook niet detecteren. 

## Conclusie
Jammer genoeg hebben we dus niets kunnen schrijven naar de tags. We hebben heel wat verschillende zaken geprobeerd. Vooral bij de laatste mogelijkheden was het moeilijk om te achterhalen waar het probleem zit. We konden niet nagaan of de tags werkten, welke soort tag het was, welke versie,... Bij de raspberry Pi kregen we zoals we daarnet vertelden ook niet veel output, waardoor we niet verder konden onderzoeken waar het probleem precies ligt. 