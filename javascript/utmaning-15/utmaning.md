# Utmaning

På samma sätt som funktioner kan ta parametrar kan Node hantera parametrar som skickas in till skriptet, de kallas för arguments eller parameters. De är värden som skickas vidare för användning inom skriptet och skrivs ut med mellanslag efter filnamnet, exempelvis så här: node test.js "Hello" "World" (skickar två parametrar för användning till skriptet test.js)

- Skapa en ny fil som heter logMyArguments.js 
- Lägg in följande värde
let triplets = process.argv.slice(2); (anledningen till att det är process.argv är att argv är array som är en property på objektet process, och slice() kanske du känner igen från förra övningen, i det här fallet tar den bort de första två värdena från argv, för dom skapar vi inte själva.)
console.log('triplets: ', triplets);
- Köra scriptet med tre parametrar "Knatte", "Fnatte", "Tjatte" för att se dem loggas av filen.

