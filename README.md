# frontend-applications

## De Opdracht
De Tech Track gaat dit jaar over "auto's in de stad". Het doel van de opdracht is om interessante patronen te vinden in de data en deze te transformeren in een interactieve datavisualisatie. Het datalab van de Volkskrant kan deze visualisaties vervolgens gebruiken om artikelen te schrijven over dit onderwerp.

Mijn **onderzoeksvraag** luidt als volgt: 

**Wat is de parkeercapaciteit van parkeergelegenheden in steden en dorpen gedurende de week?**

## Het Project
Om inzicht te geven in het aantal parkeerplaatsen in Nederlandse plaatsen is het parkeercapaciteit-platform ontwikkeld: een informatieve web app gericht op Nederlandse steden en dorpen. Het aantal parkeerplaatsen wordt visueel weergegeven in de vorm van een interactieve bar chart en toont data van alle gemeentes waarvan dit beschikbaar is.

## Features
In de responsive interactieve barchart zijn een aantal input fields. Bovenin kun je kiezen of je het aantal parkeerplaatsen wil bekijken in getallen of in procenten. Hiernaast, bij 'Dag' kun je de dag van de week selecteren. Bij 'Tijd' kun je bepalen op welk moment van de dag je de parkeercapaciteit wil bekijken. Vervolgens kun je bij 'Gemeentes' alle steden of dorpen selecteren die je in de staafdiagram wil visualiseren.

## Live Preview
[This link](https://pensive-wozniak-f915b8.netlify.app/)

![Video](https://im6.ezgif.com/tmp/ezgif-6-77b4ab8a465a.gif)

## Data
Alle data die ik heb gebruikt komt van het RDW. 

### **Dataset:** [RDW Open Data Geometrie Gebied](https://opendata.rdw.nl/Parkeren/Open-Data-Parkeren-GEOMETRIE-GEBIED/nsk3-v9n7)

_Hiermee kan ik kijken welke areaID in welke stad ligt._

**Belangrijke kolommen:**
* AreaID
* GeoDataAsText

### **Dataset:** [RDW Open Data Parking Toegang](https://opendata.rdw.nl/Parkeren/Open-Data-Parkeren-PARKING-TOEGANG/edv8-qiyg)

_Hier kun je per AreaID kijken wanneer je hier wel of niet in kunt._

**Belangrijke kolommen:**
* AreaID
* Days (day of the week) 
* EnterFrom (tijd in 24h)
* EnterUntil  (tijd in 24h)

### **Dataset:** [RDW Open Data Parkeren Specificaties Parkeergebied](https://opendata.rdw.nl/Parkeren/Open-Data-Parkeren-SPECIFICATIES-PARKEERGEBIED/b3us-f26s)


_Deze dataset bevat een capaciteit per parkeeradres. Hierin staat ook of het laadpalen bevat. Misschien is het ook leuk om hier een toggle voor te maken in de uiteindelijke visualisatie._

**Belangrijke kolommen:**
* Capacity
* ChargingPointCapacity

## Installation Guide
Ga in een terminal naar je gewenste directory. Zet dan de volgende code in de terminal.
```
git clone https://github.com/itsguus/frontend-applications

cd frontend-applications

npm install

npm run serve
```

De site staat nu lokaal op localhost:8080
