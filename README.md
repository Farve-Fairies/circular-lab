#Teknisk Dokumentation – Circular Lab

Dette website er udviklet med Astro, et moderne frontend-framework, som tillader en komponentbaseret og effektiv tilgang til udvikling af statiske og delvist dynamiske websites. Projektets fokus har været på struktur, æstetik og integration af eksterne data, snarere end mobiloptimering. Siden er dog responsiv og fungerer på tværs af skærmstørrelser.

##Projektstruktur

Projektet er organiseret i følgende mapper og filer:

/components: Her ligger genanvendelige komponenter såsom layout-struktur, tekstkort, CTA-knapper og dynamiske visninger.

/layouts: Layout-komponenter, der definerer det overordnede HTML-skelet for siderne.

/pages: Alle sider er opbygget som .astro-filer. Her struktureres HTML med import af relevante komponenter.

/public: Indeholder billeder, favicon og andre statiske assets.

/styles: Eksterne CSS-filer til global styling samt eventuel komponentstyling.

Astro tillader brug af både JSX-lignende komponentstruktur og ren HTML, hvilket giver fleksibilitet under opbygningen.

##Typografi og design

Vi har valgt Helvetica som gennemgående skrifttype for at understøtte Circular Labs æstetiske og professionelle profil. Designet er minimalistisk og tekstbåret med høj kontrast og struktureret grid-opsætning.

Farvepaletten er nedtonet og enkel, med sort, grå og enkelte fremhævede accenter som orange og blå for at skabe ro og fokus på indhold.

##Komponenter og struktur

Siden er opbygget ved hjælp af følgende nøglekomponenter:

Header.astro og Footer.astro: Kopieret direkte fra KEAs designskabelon for at skabe kontinuitet og genkendelighed.

Events.astro: Dynamisk side med komponent, som ArrowButtom.astro, der viser data fra Supabase om kommende events.

PracticalInfo.astro: Viser kontaktinformation og åbningstider.

Accordion.astro: Bruges til at vise ydelser i et sammenfoldeligt format.

Hero.astro: Viser billeder, indlæst dynamisk fra Supabase.

GlassButton.astro: En call-to-action-knap, fx “Kontakt os her”. Den har vi kodet ved hjælp og øvelse i CodePen.

Alle komponenter er tilpasset til at kunne bruges på tværs af flere sektioner.


##Dynamisk indhold via Supabase

Vi har integreret Supabase som database og backend-løsning. Her har vi selv oprettet tabeller og indhold, som hentes ind i Astro ved hjælp af fetch-funktioner i .astro-filer.

Data hentes dynamisk og vises i:

Kalender for kommende events (med billeder, datoer og tekst)

###Dynamisk Indhold via Supabase:

Programsiden og single events er bygget vha. indhold fra Supabase databasen. 
Den består af en tabel med kolonnerne ‘event_title’, ‘event_description’, ‘event_type’, ‘event_slug’, ‘event_img’, ‘event_location’, ‘event_date’, ‘event_start’ og ‘event_end’. 
Herfra er der importeret indhold via ‘url’ og ‘key’ fra Supabase projektet. De er defineret som konstanter i html-sidernes fences.

Det dynamiske setup gør det let at opdatere indhold direkte via Supabase UI uden at skulle deploye koden igen.

##Responsivitet og platformsfokus

Siden er responsiv og fungerer på både mobil og desktop, men mobilvisning har ikke været primært fokusområde. I stedet har vi designet siden til at fungere som et visuelt univers, der matcher Circular Labs udtryk på Instagram, og skaber sammenhæng mellem sociale medier og website.

##Funktionalitet

Der er ikke integreret filtrering eller avanceret brugerinteraktion. Fokus har været på at vise data visuelt, simpelt og elegant med en frontend, der er let at vedligeholde.

##Konklusion

Projektet demonstrerer en moderne frontend-løsning bygget med Astro og Supabase, med vægt på komponentstruktur, dynamisk dataintegration og designorienteret formidling. Resultatet er en præsentationsside, som understøtter Circular Labs identitet og samtidig gør brug af tidssvarende teknologier.

Forkortet/nøgleord:
Teknisk Dokumentation – Circular Lab

Framework: Astro – moderne, komponentbaseret frontend-framework til statiske/dynamiske websites. Fokus på struktur, æstetik, og integration af eksterne data. Responsivt design, men mobiloptimering ikke primært fokus.
Projektstruktur:

/components: Genanvendelige komponenter (layout, tekstkort, CTA-knapper, dynamiske visninger).
/layouts: Layout-komponenter, der definerer HTML-skelettet.
/pages: Sider som .astro-filer, med import af relevante komponenter.
/public: Billeder,favicon, statiske assets.
/styles: Eksterne CSS-filer til global og komponentstyling.
Astro Flexibilitet: Brug af både JSX-lignende komponentstruktur og ren HTML.

Typografi og Design:

Skrifttype: 'Helvetica Neue' og 'Helvetica LT STD Condensed' – understøtter æstetik og professionalisme.
Design: Minimalistisk, tekstbaseret med høj kontrast og struktureret grid.
Farvepalette: Nedtonet, sort, grå, med accenter i orange og blå.
Komponenter og Struktur:

Header.astro, Footer.astro: Kontinuitet og genkendelighed fra KEAs designskabelon.
Events.astro: Dynamisk side med Supabase-data (kommende events).
PracticalInfo.astro: Kontaktinfo og åbningstider.
Accordion.astro: Sammenfoldeligt format til ydelser.
Hero.astro: Dynamisk billeder, indlæst fra Supabase.
GlassButton.astro: CTA-knap ("Kontakt os her"), kodet med CodePen.
Dynamisk Indhold via Supabase:

#Supabase: 
Database og backend-løsning, data hentet dynamisk via fetch i .astro-filer.

Anvendelse: 
Programsiden og single events er bygget vha. indhold fra Supabase databasen.
Den består af en tabel med kolonnerne ‘event_title’, ‘event_description’, ‘event_type’, ‘event_slug’, ‘event_img’, ‘event_location’, ‘event_date’, ‘event_start’ og ‘event_end’. 
Herfra er der importeret indhold via ‘url’ og ‘key’ fra Supabase projektet. De er defineret som konstanter i html-sidernes fences. 


Responsivitet og Platforms Fokus:

Responsivitet: Fungerer på både mobil og desktop. Fokus på visuelt univers, der matcher Circular Labs Instagram-udtryk.
Funktionalitet:

Ingen filtrering eller avanceret interaktion: Fokus på enkel og elegant visning af data, let vedligeholdelse.
Konklusion:

Frontend-løsning: Bygget med Astro og Supabase, med vægt på komponentstruktur, dynamisk dataintegration og designorienteret formidling.
Resultat: Præsentationsside, der understøtter Circular Labs identitet med tidssvarende teknologier.