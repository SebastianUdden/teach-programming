# Utmaning

För att hantera data av diverse slag har JSON blivit en populär filtyp, JSON står för JavaScript Object Notation och påminner alltså starkt om hur man skriver en objekt-typ i javascript. Den enda egentliga skillnaden är att properties i JSON skrivs med citat-tecken runt sig. Här är ett exempel:

{
    "firstName": "Sofia",
    "lastName": "Carlsson",
    "onParentalLeave": true
}

- Skapa en fil som heter me.json som du kopierar in ovanstående exempel
- Skapa en till fil som heter readJSON.js
- Här ska vi använda oss av filsystemet för att Node ska kunna läsa filer, då behöver vi importera filesystem objektet med följande kod:
let fs = require('fs');
- Lägg sedan in funktionen för att läsa filer, den tar namnet på filen som en parameter samt en funktion med parametrarna error och data. Inuti funktionen kan vi hantera datan som läses in av filsystemet. I vårt fall har vi läst in JSON vilket betyder att vi behöver "avkoda" datan till vanlig javascript med hjälp av funktionen JSON.parse():
fs.readFile('me.json', function(err, data) {
    const me = JSON.parse(data)
    console.log(me)
});
- Prova att logga ut de tre properties som finns på me-objektet inuti readFile funktionen
- Skapa sedan en ny fil som heter them.json som också innehåller properties firstName, lastName och onParentalLeave för tre vänner
- Läs även in den filen och logga värdena från den (ta hjälp av en arraymetod), för propertyn onParentalLeave kan du använda en if-sats för att logga den mer läsbar strängen "Is on parental leave" ifall den är sann.