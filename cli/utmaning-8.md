# Utmaning

- Öppna iTerm
- Hitta filen .zshrc och öppna den i VS Code
- I botten av den kan du lägga till egna bash-funktioner, börja med att lägga till följande funktion
- En genväg till repositories-mappen, så du enbart behöver skriva ett ord för att komma dit tömma terminalen och visa vad som finns i mappen

repos() {
    cd Documents/Repositories
    clear
    ls -1
}

- Öppna ett nytt iTerm-fönster med CMD+D och prova skriv commandot "repos"
- Skapa sedan en liknande funktion som går till dokument-mappen och en för att gå till skrivbordet