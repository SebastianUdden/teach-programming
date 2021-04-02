# Utmaning

- Öppna iTerm
- Öppna .zshrc i VS Code
- Skapa en funktion för att göra en google-sökning från terminalen

Tips 1: Använd url http://www.google.com/search?q= och lägg till argument för sökning
Tips 2: $1, $2 etc. är argument som kan passas in i en funktion, så om du har en funktion som ser ut så här

dubbel-eko() {
    echo $1 $1
}

kan du sen använda funktionen så här: "dubbel-eko pang"
Det kommer skriva ut "pang pang"

Om du istället skulle skriva exempelvis så här

dubbel-eko() {
    echo $2 $1
}

kan du sen använda funktionen så här: "dubbel-eko pang boom"
Det kommer skriva ut "boom pang"