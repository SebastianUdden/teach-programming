# Utmaning

Den tredje komplexa typen av javascript är på många sätt den allra viktigaste, "function" eller funktion på svenska. En funktion är en samling av logik som kan återanvändas, den körs genom att skriva namnet på funktionen och avsluta med (), exempel på färdiga funktioner vi redan använd är console.log() och alert().

Här är ett enkelt exempel på en funktion som visar värdet av 1 + 1.

function onePlusOne () {
    return 1 + 1
}

värdet "return" är väldigt vanligt för funktionen, det värdet betyder att man låter funktionen göra en viss logik, sen ger eller "returnerar" ett resultat. Ett lämpligt sätt att sedan använda funktionen onePlusOne skulle då vara att sätta det returnerade värdet i en ny variabel så här:

const result = onePlusOne()

Vi kan sedan logga värdet med console.log(result)

- Skapa en ny fil som heter sum.js
- Skapa funktioner i sum.js som summerar 1 + 1, 2 + 2, 3 + 3 etc. upp till 10 + 10.
- Kör sedan alla funktionerna och sätt deras värden i varsin variabel, addera variablerna och logga värdet.