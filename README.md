# Case4 JavaScript API

## Introduktion
I caset ska ni arbeta individuellt och skapa en applikation (webbsida) som visualiserar data som hämtas från ett API. Applikation ska visualisera data som kan hämtas via ett API som ni själva väljer.

Att visualisera data innebär i praktiken att ni med HTML, CSS och JavaScript ska skapa ett dynamiskt flöde med det innehåll från det API ni väljer.

Det ska vara en applikation som har header, footer, nav och andra lämpliga sematiska element. Första gången applikationen visas ska den fungera som en landningssida som hanterar sökningar. Sidan ska också ha en genomgående design som passar till det API ni väljer. 

## Val av API
Ni väljer helt själva API:et. Ni kan välja ett som ni hittar på nätet men här finns några ni kan undersöka.

- https://api.nasa.gov/, NASAs API
- https://api.openweathermap.org/, OpenWeatherMap API
- https://api.unsplash.com/, Unsplash API
- https://pokeapi.co/, Pokemon API
- https://www.thecocktaildb.com/api.php, The Cocktail DB
- https://swapi.dev/, Star Wars API
- https://github.com/public-apis/public-apis?tab=readme-ov-file, alla API:er

## Grundläggande Krav
- Applikationen ska vara responsiv och fungera på **både desktop och mobil**.
- Applikationen ska vara en SPA (Single Page Application) och använda sig av JavaScript för att byta ut innehåll utan att ladda om sidan. Användaren upplever olika sidor men i bakgrunden är det en enda sida som skiftar innehåll (view).
- Minst 10 commits som visar kontinuerligt arbete under arbetsperioden
- En README.md med kort förklaring vilka funktioner applikationen stödjer och eventuell hur man får en API-nyckel om det krävs.
- Applikationen ska ha en header, footer, (nav) och andra lämpliga sematiska element.
- När applikationen startar ska sidan fungera som en startsida / landningssida. 
- En användare ska därefter interagera med sidan (submit, scroll, touch ...) för att hämta data via fetch.
- I det resultat som presenteras ska det därefter vara möjligt att visa detaljer om utvald data. Här ska ett nytt fetch anrop ligga till grund för det som presenteras

T.ex
```
// Listan med objekt
[{"name":"bulbasaur","url":"https://pokeapi.co/api/v2/pokemon/1/"},{"name":"ivysaur","url":"https://pokeapi.co/api/v2/pokemon/2/"},{"name":"venusaur","url":"https://pokeapi.co/api/v2/pokemon/3/"},{"name":"charmander","url":"https://pokeapi.co/api/v2/pokemon/4/"},{"name":"charmeleon","url":"https://pokeapi.co/api/v2/pokemon/5/"},{"name":"charizard","url":"https://pokeapi.co/api/v2/pokemon/6/"},{"name":"squirtle","url":"https://pokeapi.co/api/v2/pokemon/7/"},{"name":"wartortle","url":"https://pokeapi.co/api/v2/pokemon/8/"},{"name":"blastoise","url":"https://pokeapi.co/api/v2/pokemon/9/"},{"name":"caterpie","url":"https://pokeapi.co/api/v2/pokemon/10/"},{"name":"metapod","url":"https://pokeapi.co/api/v2/pokemon/11/"},{"name":"butterfree","url":"https://pokeapi.co/api/v2/pokemon/12/"},{"name":"weedle","url":"https://pokeapi.co/api/v2/pokemon/13/"},{"name":"kakuna","url":"https://pokeapi.co/api/v2/pokemon/14/"},{"name":"beedrill","url":"https://pokeapi.co/api/v2/pokemon/15/"},{"name":"pidgey","url":"https://pokeapi.co/api/v2/pokemon/16/"},{"name":"pidgeotto","url":"https://pokeapi.co/api/v2/pokemon/17/"},{"name":"pidgeot","url":"https://pokeapi.co/api/v2/pokemon/18/"},{"name":"rattata","url":"https://pokeapi.co/api/v2/pokemon/19/"},{"name":"raticate","url":"https://pokeapi.co/api/v2/pokemon/20/"}]

// Objektet vi har valt:
{"name":"ivysaur","url":"https://pokeapi.co/api/v2/pokemon/2/"}

// När användaren har klickat -> ny fetch hämta ytterligare information via fetch(https://pokeapi.co/api/v2/pokemon/2/)
{ "abilities": [...], "cries": [...], "sprites": [...],  .. }
```

- Applikationen ska ha en loading spinner medans data hämtas.

## Utmaningar
- Applikationen ska stödja "Sparade Favoriter". En en separat lista med sparade resurser (via LocalStorage) som finns kvar efter omstart.
- Applikationen ska stödja någon form av inställningsbar sortering. (T.ex Bokstavsordning, datum, antal, etc)

## Design Krav (Grundläggande)
- En HI-FI design i Figma
- Applikationen ska ha en genomgående design som passar till det API ni väljer
- Designa med minst en Komponent och en Auto Layout 

## Design Krav (Utmaningar)
- Interaktiv prototyp i Figma som visar hela flödet
- Komponent med varianter

## Namngivningsprinciper när du kodar
använd latinska tecken för variabelnamn och funktioner (camelCase)
skriv kommentarer med egna ord i din kod (så vi vet att ni förstår er egen kod)
korrekt formaterat kod

## Om koden i applikationen
Applikationen får inte använda externa ramverk, utan det är "vanilla" JavaScript och CSS som gäller. Dela upp struktur, innehåll, design och logik. Använd externa filer för CSS och JavaScript.

## Så börjar du
Börja med er Figma-skiss och dela den med Mattais. Sedan skapa ett privat repo på GitHub och koppla det till din lokala utvecklingsmiljö. Under projektet - senast 27 januari bjuder du in dina lärare. Se Settings -> Manage access -> Add people

Bjud in följande användare till ert case repo:

- frozenbanana (Henry)
- andsju (Anders)
- addkolon (Mattias)

Länka er Figma skiss till README.md

## Angående AI
- AI verktyg som ChatGPT är tillåtet att använda under kravet att alla frågor som bidrar till kod i er inlämning ska dokumenteras i en fil: `prompts.md`.
- Vi förutsätter att ni har djupgående förståelse över all kod i er inlämning. En godkänd modul innebär att ni kan ge goda svar på de frågor vi lärare har angående koden. 

## Inlämning och redovisning
- Halvtidsredovisning för redovisning av Hi-fi skiss med Mattias 27 janauari kl 08:45.
- Redovisning av caset är onsdagen den 4 februari kl 10:25. Feedback följer under vecka 7
- Caset ska finnas färdigt i ett Gihub repo i samband med redovisningen
- Tänk på att inte visa console.log() i ett färdigt projekt.
- Länka in er figma-skiss i er README.md fil

Förbered 5 minuters redovisning enligt följande mall:

- Visa er Figma Design
- demonstrera applikationen
- visa exempel på annan funktionalitet (ex ngn av utmaningarna)
- visa hur AI har stöttat ert arbete (visa upp `log.md`) 
- berätta vad du är mest nöjd med (design, kod, struktur...)
- berätta vad du skulle vilja att applikationen kan göra, men inte hunnit att koda
- redovisning sker i bokstavsordning (förnamn A-Ö)
