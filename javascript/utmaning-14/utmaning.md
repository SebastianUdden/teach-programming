# Utmaning

Arrayer har ett antal färdiga funktioner som är väldigt användbara, några vanliga är exempelvis .forEach() .filter() .find() .slice(), .sort(), .reverse() och .map()

Vi kommer använda exemplet const fruits = ["apple", "pineapple", "banana", "pear"]

## .forEach()
Används för att gå igenom arrayen och för varje element göra något. 

Exempel:
fruits.forEach(fruit => {
    console.log(fruit)
})

Kommer logga ut:
"apple"
"pineapple"
"banana"
"pear"

## .filter()
Används för att filtrerar element i arrayen. 

Exempel:
const noBananas = fruits.filter(fruit => fruit !== "banana")
console.log(noBananas)

Kommer logga ut:
["apple", "pineapple", "pear"]

## .find()
Används för att filtrerar element i arrayen. 

Exempel:
const banana = fruits.filter(fruit => fruit === "banana")
console.log(banana)

Kommer logga ut:
"banana"

## .slice()
Returnerar en del av arrayen.

Exempel:
const someFruits = fruits.slice(1)
console.log(someFruits)

Kommer logga ut:
["pineapple", "banana", "pear"]

## .sort()
Sorterar arrayens värden

Exempel:
const sortedFruits = fruits.sort()
console.log(sortedFruits)

Kommer logga ut:
["apple", "banana", "pear", "pineapple"]

## .reverse()
Sorterar arrayens värden

Exempel:
const reversedFruits = fruits.reverse()
console.log(reversedFruits)

Kommer logga ut:
["pear", "banana", "pineapple", "apple"]

## .map()
En personlig favorit, går igenom samtliga värden och ger möjlighet att manipulera det innan en ny array skapas

Exempel:
const uppercaseFruits = fruits.map(fruit => {
    return fruit.toUpperCase()
})
console.log(uppercaseFruits)

Kommer logga ut:
["APPLE", "PINEAPPLE", "BANANA", "PEAR"]

## Kombination
Array-funktioner går att sätta ihop i olika kombinationer (så kallad chaining), detta görs genom att man sätter punkt och skriver nästa funktion. Exempel:

const reversedUppercaseFruits = fruits.map(fruit => {
    return fruit.toUpperCase()
}).reverse().slice(2)
console.log(reversedUppercaseFruits)

Kommer logga ut:
["PEAR", "BANANA"]

- Med dina nya arraykunskaper, skapa en ny fil som heter formated-fruits.js
- Lägg in följande variabel "const fruits = ["duran", "apple", "banana", "pear", "mango"]"
- Gör så att arrayen blir sorterad, att varje frukt skrivs med stor text, har texten "a yummy " före sig och att duran-frukten inte är med, för den luktar illa. Avslutningsvis ska varje "frukt-värde" loggas ut var för sig.