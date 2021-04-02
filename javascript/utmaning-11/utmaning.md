# Utmaning

Förutom function, array och object så vilar JavaScript på en fjärde grundpelare och det är if-statement (eller if-sats på svenska), de ställer frågan "Är det här sant?" Ifall svaret är ja utför de en viss logik. If-satser tar ett boolean-värde, dvs. true eller false. Exempelvis:

if (true) {
    Det här kommer alltid hända
}

if (false) {
    Det här kommer aldrig hända
}

De ovanstående exemplen är inte så användbara, utan det som gör if-satser så bra är att de kan använda conditionals, dvs. beräkningar i slutändan blir true eller false. Här är exempel på några olika conditionals:

=== Blir true om något är lika med (ex. "blue" === "blue" är true, "blue" === "red" är false)
!== Blir true om något inte är lika med (ex. "blue" !== "blue" är true, "blue" !== "red" är true)
> Blir true om det vänstra talet är mer än det högra (ex. 5 > 3 är true, 3 > 5 är false)
>= Blir true om det vänstra talet är mer eller lika mycket som det högra (ex. 5 >= 5 är true, 5 >= 6 är false)
< Blir true om det högra talet är mer än det vänstra (ex. 5 < 3 är false, 3 < 5 är true)
<= Blir true om det högra talet är mer eller lika mycket som det vänstra (ex. 5 <= 5 är true, 5 <= 4 är false)

Här är ett vanligt exempel där vi har en variabel som vi sedan kollar om den har ett visst värde:

let color = "red"

if (color === "red") {
    console.log(color)
}

- Skapa en fil som heter if.js
- Lägg in en array med färger let colors = ["green", "yellow", "red"]
- För varje färg, kolla om färgen är röd, logga värdet i så fall.