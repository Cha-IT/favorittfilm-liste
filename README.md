## **Oppgave: Lag en Favorittfilmer-liste**

### **Mål:**
- Lære hvordan man oppretter og manipulerer arrays i JavaScript.
- Øve på å legge til og fjerne elementer fra en array.
- Forstå hvordan man kobler arrays til et enkelt brukergrensesnitt i HTML.

### **Oppgavebeskrivelse:**

Du skal lage en liten applikasjon der brukeren kan legge til sine favorittfilmer i en liste og se listen oppdatert på skjermen. Bruk arrays i JavaScript for å lagre filmene, og vis dem i HTML.

### **Krav til applikasjonen:**

1. **App Struktur:**
   - **Input-felt:** Et tekstfelt der brukeren kan skrive inn navnet på en film.
   - **Legg til knapp:** En knapp for å legge til filmen fra input-feltet til favorittfilmer-listen.
   - **Liste:** En liste som viser alle filmene som er lagt til.
   - **Slett knapp:** En knapp for å slette hele listen.

2. **Funksjonalitet:**
   - Brukeren skal kunne skrive inn filmnavn i et input-felt og legge filmen til i en liste ved å klikke på "Legg til"-knappen.
   - Når en film blir lagt til, skal listen med favorittfilmer oppdateres i brukergrensesnittet.
   - Brukeren skal også kunne slette hele listen med favorittfilmer ved å klikke på "Slett listen"-knappen.

### **HTML & CSS-oppgave:**

1. **HTML-struktur:**

   Start med en enkel HTML-fil som gir brukeren et input-felt for å skrive inn filmnavn, en knapp for å legge til film, og et område for å vise listen med filmer.

   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>Favorittfilmer</title>
     <style>
       body {
         font-family: Arial, sans-serif;
         max-width: 600px;
         margin: 0 auto;
         padding: 20px;
         text-align: center;
       }
       ul {
         list-style-type: none;
         padding: 0;
       }
       li {
         margin: 5px 0;
       }
     </style>
   </head>
   <body>
     <h1>Favorittfilmer</h1>
     <input type="text" id="movieInput" placeholder="Skriv inn en film" />
     <button id="addButton">Legg til</button>
     <button id="clearButton">Slett listen</button>

     <h2>Din filmliste:</h2>
     <ul id="movieList"></ul>

     <script src="app.js"></script>
   </body>
   </html>
   ```

2. **JavaScript-oppgave:**

   Opprett en JavaScript-fil (`app.js`) for å håndtere logikken bak appen. Her skal du opprette en array for å lagre filmene, og bruke enkle funksjoner for å legge til elementer i arrayen og vise dem i HTML.


### **Trinn for trinn:**

1. **Legg til en film:**
   - Brukeren skriver inn navnet på en film i input-feltet.
   - Når brukeren klikker på "Legg til"-knappen, legges filmen til i en array.
   - Listen vises umiddelbart i nettleseren.

2. **Slett listen:**
   - Når brukeren klikker på "Slett listen"-knappen, tømmes hele arrayen, og visningen av listen oppdateres for å vise at den er tom.

3. **Vis arrayen:**
   - Bruk JavaScript til å iterere gjennom arrayen og vise hver film i HTML-listen.

---

### **Ekstra utfordringer:**
- Legg til validering som sørger for at du ikke kan legge til en tom film i listen.
- Vis en melding dersom listen er tom, som forsvinner når det legges til filmer.
- Gjør listen mer interaktiv ved å legge til en mulighet for å fjerne en enkelt film fra listen.

---

Denne oppgaven gir elevene en praktisk måte å forstå arrays på, samtidig som de lærer hvordan man bygger en enkel applikasjon ved hjelp av HTML, CSS og JavaScript.
