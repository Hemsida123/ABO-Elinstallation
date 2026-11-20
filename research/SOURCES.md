# Källor och avgränsningar

Kontrollerat 20 november 2026. Alla kundtexter är omskrivna. Originalrecensioner och långa originalpassager återges inte.

## Originalwebbplatsen

- [Startsida](https://www.aboelinstallation.se/): verksamhet i Skåne, telefon, jour dygnet runt, tjänsteöversikt och sociala länkar.
- [Tjänster](https://www.aboelinstallation.se/tjanster/): samtliga 10 tjänster som ligger till grund för de nya tjänstevyerna. Ingen ny produkt, produktpartner eller installationstyp har hittats på.
- [Om oss](https://www.aboelinstallation.se/om-oss/): André Nilsson, Björn Persson och Ola Holmberg, roller och yrkesbakgrund; verksamhetens rötter i NP El & teknik 2017.
- [Kontakt](https://www.aboelinstallation.se/kontakt/): ABO Elinstallation AB, Koppargatan 19, 271 39 Ystad,0411-26 26 00,info@aboelinstallation.se. Kontaktsidans ruta i ny design bör använda dessa uppgifter. Den exakta originalrutten är `/kontakt/`, inte `/kontakta-oss/`.
- [Boka elektriker](https://www.aboelinstallation.se/boka-elektriker/): namn, mejl, meddelande och samtycke är obligatoriska i den faktiska HTML-strukturen. Telefon, adressuppgifter och datum är frivilliga. Originalet har fyra bilduppladdningar. Den fristående redesignen förbereder mejlutkast och låter besökaren bifoga bilder i sitt mejlprogram; den påstår inte att en bokning är mottagen.
- [Prislista](https://www.aboelinstallation.se/prislista/) med [företagspriser](https://www.aboelinstallation.se/kopia-av-prislista-privat/) och [privatpriser](https://www.aboelinstallation.se/kopia-av-prislista/): källor för att det finns offert, löpande arbete, utkörning och jour. Inga belopp eller skattesatser förs över som nya aktuella erbjudanden.
- [Instagram](https://www.instagram.com/aboelinstallation/) och [Facebook](https://www.facebook.com/ABO-Elinstallation-106887794661907/): exakta länkar hämtade från originalets aktuella HTML. Inga stjärnbetyg, omdömesantal eller svar från dessa plattformar påstås.

Dessa åtta originalsidor är sparade som HTML i `research/pages/`. Hashmanifest med URL, kontrolltidpunkt, storlek och SHA256 finns i `research/pages/manifest.json`.

## Verifierad registrering hos Elsäkerhetsverket

Den offentliga [Kolla elföretaget-sökningen på organisationsnummer 5591400618](https://elsakerhetsverket.se/kolla-elforetaget?query=5591400618&searchType=company&sortOrder=az&page=1) gav 20 november 2026 en träff: **ABO Elinstallation AB**, organisationsnummer **559140-0618**, Koppargatan 19, 271 39 Ystad. Posten innehåller samma webbplats, e-post och telefon som originalet. Resultatet ligger i myndighetens serverlevererade `AppRegistry.registerInitialState` med `numHits:1` och rätt organisationsnummer. Exakt HTML är sparad som `registry-company.html`, dessutom sparas den allmänna söksidan som `registry-search.html`. Organisationsposten och kategorimappningen finns även i `research/facts.json`.

Detta stöder formuleringen **”Registrerat hos Elsäkerhetsverket.”** Det är en verifiering av företagsregistreringen vid kontrolltillfället, inte en personlig auktorisation, ett myndighetsgodkännande av all marknadsföring eller en garanti om framtida registrering. För projektets aktuella verksamhetstyper hänvisas till registret. Inga myndighetslogotyper används som certifieringsmärken.

Den äldre ursprungslänken `e-tjanster.elsakerhetsverket.se/foretag/kolla-elforetaget` omdirigerar till den nya tjänsten. Webbläsningsverktygets renderare kunde inte återge den parametriserade träffen, men den direkta offentliga HTTPS-hämtningen gav ovanstående faktiska myndighetsresultat; inga inloggningar, privata API:er eller säkerhetsundantag användes.

## Bolagsidentitet och motsägelser

[Ratsit](https://www.ratsit.se/5591400618-ABO_Elinstallation_AB) och [Allabolag](https://www.allabolag.se/foretag/abo-elinstallation-ab/ystad/byggm%C3%A4stare/2KGZ4BUI5YDDT) bekräftar juridiskt namn, organisationsnummer, adress och telefon via webbläsningsverktygets sökresultat/sidtext. Direkt arkivhämtning av dessa två stödregister gav 403 och har inte behandlats som lyckade HTML-källor. Myndighetsregistrets aktuella träff är den starkaste identitetskontrollen.

Originalets om-sida säger att NP El & teknik blev ABO 2021 när Ola anslöt. Ratsit anger registrering av firmanamnet 2020-10-07. Texterna använder därför verksamhetens rötter 2017 och beskriver att Ola senare anslöt, utan ett exakt namnbytesår. De tre delägarnas yrkesroller kommer från företagets egen aktuella om-sida; personlig auktorisationsklass verifieras inte.

## Pris- och jouravgränsning

Den direkt hämtade företagsprislistan har andra belopp än sökindexets äldre version. Beloppen är odaterade. Privatprislistan innehåller ROT-text och bokningsformuläret innehåller villkor för skatteavdrag som inte behövs för redesignens förfrågan. Inga skattesatser, avdragsbehörigheter, kampanjer eller fasta belopp reproduceras som nya utfästelser. Besökaren får beskriva arbetet och stämma av aktuellt pris och villkor direkt med ABO.

Jour dygnet runt och årets alla dagar är företagets egen uttryckliga uppgift på både startsidan och tjänstesidan. Inget exakt svarstids- eller inställelselöfte läggs till. Prislistans dagtidsintervall är en debiteringskategori och används inte som verifierade kontorsöppettider. Kvälls- och helgkategorierna överlappar i originalets fredagstider; inget nytt exakt jourschema skapas. Akuta ärenden hänvisas till telefonen, inte ett mejlutkast.

## Andra medvetna avgränsningar

- Inga fabricerade recensioner, projekt, kunder, betyg eller försäljningssiffror.
- Originalets 40+ år är ett odaterat gemensamt erfarenhetspåstående. Inga framräknade erfarenhetsräknare.
- Originalet erbjuder offert men säger inte uttryckligen att den är kostnadsfri; inget gratislöfte läggs till.
- Bildernas verkliga ursprung och gränsen mellan illustration och dokumenterat projekt hanteras i `research/assets.json` och `research/asset-notes.md`.
- Inga instruktioner om hur besökaren ska utföra elarbete själv, inga rättsliga eller skattemässiga råd.
- Integritetstexten gäller den levererade fristående filen: mejlutkast som besökaren själv skickar, ingen automatisk sändning eller bekräftad bokning, ingen webbläsarlagring, spårning eller inbäddad karta. Den behöver uppdateras om en server, lagring eller externa inbäddningar ansluts senare.
