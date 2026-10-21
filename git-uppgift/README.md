# Git-uppgift - Individuell Examination

Detta projekt innehåller tre JavaScript-funktioner samt en Git-workflow-demonstration.

## Svar på analysfrågor

### 1. Vad är skillnaden mellan working directory, staging area och repository i Git?
* **Working Directory (Arbetsytan):** Det är mappen där du arbetar och redigerar dina filer i din kodredigerare (t.ex. VS Code). Ändringar här spåras inte av Git förrän du väljer att lägga till dem.
* **Staging Area (Förberedelseområdet):** Här hamnar filer när du kör `git add`. Det fungerar som en mellanlandning eller "packsedel" där du väljer exakt vilka ändringar som ska ingå i din nästa commit.
* **Repository (Arkivet):** Det är Gits databas där alla sparade commits, historik och versionsändringar lagras permanent när du kör `git commit`.

### 2. Varför är det användbart att använda `.gitignore`?
En `.gitignore`-fil används för att berätta för Git vilka filer och mappar som inte ska spåras eller skickas upp till GitHub. Det är användbart för att:
* Undvika att ladda upp känslig information (som API-nycklar eller lösenord i `.env`-filer).
* Slppa att ladda upp tunga eller temporära filer (som `node_modules` eller loggfiler).
* Hålla repositoryt rent och professionellt.

### 3. Vad innebär ett "fast-forward merge" i Git?
En fast-forward merge sker när du slår ihop en gren (branch) med en annan, och den grenen du slår ihop med inte har fått några nya commits sedan du förgrenade dig. Git flyttar då bara fram pekaren direkt till den senaste committen utan att behöva skapa en ny "merge commit".