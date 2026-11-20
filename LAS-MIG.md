# ABO Elinstallation – premium-redesign

Öppna `index.html` i en modern webbläsare. Allt ingår: bilder, typsnitt, stilar och funktioner. Ingen installation behövs. `redigerbar.html` är samma webbplats med separata assets- och fonts-mappar; behåll mapparna bredvid filen. Navigationen når alla vyer. Gamla sidnamn finns som omdirigeringar i ZIP-paketet.

## Innehåll
Stor fotografisk fullskärmshero, tio tjänstevyer, jourkontakt, företaget och tre namngivna delägare, bildgalleri med åtta originalbilder, filtrering och bildvisare, arbetssätt, registreringsinformation, pris/offert för privatperson och företag, FAQ, kontakt och bokningsförfrågan. Mobilanpassning, tangentbordsstöd, färgtema och reducerad rörelse. Designed by Ekom länkar till ekom.se.

## Kontakt och bokning
Formulären validerar uppgifter och sammanställer en förfrågan i besökarens mejlprogram, adresserad till info@aboelinstallation.se. Besökaren granskar, bifogar bilder och skickar själv. Ingen server, automatisk sändning eller mottagningsbekräftelse finns. Ingen tid reserveras; ett uppdrag kräver överenskommelse med ABO. Akuta ärenden hänvisas till telefon 0411-26 26 00. Inget nytt svarstids- eller inställelselöfte läggs till.

Telefon, adress och datum är frivilliga. Datum är önskemål. Text kan kopieras som alternativ till mejllänken. Formulärdata finns bara i den öppna sidan och behålls vid intern navigation; omladdning rensar dem. Ingen lokal lagring, spårning, analys, externa kartinbäddningar eller automatiska meddelanden. Integritetstexten behöver uppdateras om någon senare kopplar på ett formulärsystem eller annan datalagring.

## Fakta och bilder
Företagsuppgifter och tjänster kommer från aboelinstallation.se. Elsäkerhetsverkets offentliga register gav 20 november 2026 en träff på ABO Elinstallation AB, org.nr559140-0618, med matchande kontakter. Registrering i företagsregistret påstås; ingen personlig auktorisation eller myndighetscertifiering av all verksamhet påstås. Länk till aktuell myndighetssökning finns på webbplatsen.

Alla bilder är verkliga originalfoton från ABO:s webbplats. Åtta arbetsbilder och tre personporträtt har verifierade källor och namnkopplingar. Arbetsbilderna har inga verifierade kund-/projektnamn, resultat eller platsuppgifter. Därför presenteras de med beskrivande aktivitetsnamn, utan fabricerade projektfall. Logotypen är originalets gula/vita bild med redan befintlig transparens, endast beskuren till alfagräns och skalad. Den visas på mörk bakgrund så att den vita texten syns.

Inga fabricerade recensioner, betyg, kundantal, erfarenhetsräknare, garantier eller gratis offertlöften. Originalets odaterade prislistor skiljer sig från äldre sökindex; inga belopp, ROT-satser eller överlappande jourdebiteringstider kopieras som aktuella priser. I stället uppmanas besökaren att stämma av aktuellt pris och villkor. Länkar till ursprungliga prislistor finns kvar. Ingen instruktion om hur besökaren själv ska utföra elarbete ges.

Källor och avgränsningar finns i research/SOURCES.md och facts.json. Bildfiler, ursprungsadresser, dimensioner och SHA256 redovisas i bildkallor.json och research/assets.json.

## Redigera och bygga
Källor: qa/template.html, qa/site.css, qa/site.js, qa/content.json samt research/media.json. Med Python3, BeautifulSoup och Node kan du bygga om genom `python3 qa/build.py` och kontrollera genom `python3 qa/verify.py`.

Vyerna använder hash-navigation för att fungera i en fristående fil. Titlar och beskrivningar uppdateras vid navigation; lösningen är ingen serverrenderad separat HTML-sida för varje sökmotorindex. Typsnitten är Exo2 och Manrope från Google Fonts. Öppna SIL-licenser finns i fonts och källor i typsnitt.json.

## Kontroll och leverans
Paketets CRC och filinnehåll kontrolleras, liksom inbäddade bilder/typsnitt, giltig JavaScript, alla vyer och länkar, företagsuppgifter, Ekom-länk och metadata. Verklig mobil- och datorgranskning görs i lokal webbläsare. Mejllänkar provas utan sändning; inget kontaktas och ingen bokning genomförs. Native öppning av filer eller mejlprogram automatiseras inte. Webbplatsen är inte publicerad och ersätter inte ABO:s ordinarie webbplats.

### Utförd kontroll
23 vyer provade vid1440,1024,768,390 och320px, totalt115 faktiska webbläsarvisningar utan horisontellt överflöde, saknade vyer eller trasiga inlästa bilder. Heron provad i åtta skärmformat med minst full första skärmhöjd, läsbart innehåll och synliga handlingar; korta mobilskärmar får naturligt växande sektion. Tjänstefilter, bildfilter/sökning/tomt resultat, bildvisarens knappar/piltangenter/Escape/fokus, mobilmeny och FAQ med tangentbord provade. Formulärens serviceförval, krav, frivillig telefon/adress/datum, e-post, postnummer och datumordning kontrollerade. HTML i inmatad text visas bokstavligt utan injektion. Mejllänkens avkodade text matchar sammanställningen och kopieringsknappen fungerar. Ingen mejlklient öppnas eller förfrågan skickas vid testet. Ljust/mörkt tema fungerar. Bild- och faktaunderlag har granskats separat.
