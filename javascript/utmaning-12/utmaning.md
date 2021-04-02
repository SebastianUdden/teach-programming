
# Utmaning

if-statements kan även göra något om värdet blir false, då skriver man ut else och hanterar logiken där. Exempelvis:

if (false) {
    Det här kommer aldrig hända
} else {
    Det här kommer alltid hända
}

Det går även att skriva flere if-kollar på rad. Då försöker if satsen tills den stöter på den första conditional som blir true och avslutar sedan utan att kolla resterande, exempelvis:

if (false) {
    Det här kommer aldrig hända
} else if (false) {
    Det här kommer aldrig hända
} else if (true) {
    Det här kommer alltid hända
} else if (true) {
    Det här kommer aldrig hända
} else {
    Det här kommer aldrig hända
}

- Skapa en fil som heter else-if.js
- Lägg in en array med färger let weather = ["sunny", "cloudy", "rainy", "thunderstorm", "snowy"]
- För varje väder, kolla om det är soligt, skriv i så fall ut "Running is easy".
- Om det inte är soligt, kolla om det är molnigt, skriv i så fall ut "Running is all right".
- Om det inte heller är molnigt, kolla om det är åskväder, skriv i så fall ut "Running is forbidden".
- Om ingen av de ovanstående gäller, skriv ut "Running is necessary".