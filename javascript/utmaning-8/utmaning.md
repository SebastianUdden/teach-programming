# Utmaning

Javascript har förutom de enkla typerna två komplexa typer som är väldigt viktiga: 
- array (en lista), skrivs med []
- object (ett objekt), skrivs med {}

Kortfattat används array för att spara flera saker, kan vara av samma typ eller olika och använder , för att separera dem (ex. const names = ["Sebastian", "Sofia", "Estelle"]). Objekt används för att spara komplexa saker, de består av flera "properties" som skrivs ut som property: value och använder också , för att separera (ex. const partner = {firstName: "Sebastian", lastName: "Uddén", age: 33})

För att ta ut ett värde från en array används "indexnotation" med elementets position (index), där 0 är första elementet, 1 är andra etc. Om vi tar exemplet med names ovanför kommer names[0] ge värdet "Sebastian" och värder names[2] ge värdet "Estelle".

För att ta ut ett värde från ett objekt används "punktnotation" med properties. Om vi tar exemplet med partner ovanför kommer partner.firstName ge "Sebastian" och partner.age ge värdet 33.

Objekt kan innehålla listor och listor kan innehålla objekt, det kan kännas komplext i början men gör att man kan spara bra datastrukturer som exempelvis: 

const family = [
    {
        firstName: "Sofia",
        lastName: "Carlsson",
        favoriteExercise: ["Running", "Skiing", "Gym", "Golf"]
    },
    {
        firstName: "Sebastian",
        lastName: "Uddén",
        favoriteExercise: ["Basketball", "Running", "Golf", "Tennis"]
    },
    {
        firstName: "Estelle",
        lastName: "Uddén",
        favoriteExercise: ["Crawling", "Arm and leg waving", "Bouncing"]
    }
]

För att ta ut värde från komplexa object kan vi kombinera punkt och indexnotation i valfritt djup. Så om vi vill få ut det sista värdet från dina träningstyper dvs. "Golf" skriver vi family[0].favoriteExercise[3]

- Skapa ett nytt skript och använd objektet family.
- När skriptet körs ska det logga ut en mening per familjemedlem som kombinerar förnamn, efternamn och träningsaktiviteter