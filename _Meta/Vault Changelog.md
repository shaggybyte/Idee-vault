---
title: "Vault Changelog"
type: meta
tags: [meta, changelog]
reviewed: "2026-08-17"
---

# Vault Changelog

## v6 — 2026-08-17

Pełny raport: [[Vault Audit v6]].

- wykonano **pełny lokalny audyt całego `main`**, a nie audyt różnicowy: snapshot GitHuba został odtworzony lokalnie i zweryfikowany Git blob SHA dla wszystkich 225 plików przed zmianami;
- poprawiono historyczne niedoszacowanie liczby Markdown: snapshot v5 miał **223 pliki `.md`** (222 niepuste/treściowe + pusty placeholder `_Inbox`), a nie 222 ogółem;
- pełny parser potwierdził przed poprawkami: 0 błędów YAML, 0 duplikatów basename, 0 niedomkniętych fence'ów i 0 nierozwiązanych wikilinków; ujawnił natomiast 5 nieosiągalnych plików i niepełny [[YouTube źródła MOC]];
- podłączono do kanonu trzy zewnętrzne źródła sporu o decyzje komisji zwolnień warunkowych przez [[Szum w osądach i higiena decyzyjna]];
- [[README]] i [[Notes to integrate]] są teraz osiągalne od [[Home]], a `_Inbox` ma poprawny frontmatter i jasną funkcję;
- przebudowano [[YouTube źródła MOC]] jako **kompletny indeks 56 zachowanych źródeł YouTube**;
- w pełnym audycie zakresu usunięto 5 starszych materiałów, które nie przechodziły obecnej bramy retencji: *Psychologia tłumu — Analizy Live*, *Czytamy naturę 146*, *Dragan i Stanowski*, *Andrzej Dragan — bezczelny fizyk* oraz *Nerwowe labradory — stereotyp rasy i projekt badania*; historyczne logi zachowują nazwy i powody bez martwych wikilinków;
- audyt zakresu potwierdził, że w aktywnym kanonie nie ma samodzielnych notatek czysto IT; pozostałe wątki AI dotyczą inteligencji, autonomii, epistemologii, prywatności, nauki lub społeczeństwa;
- dodano do [[Ideas Profile Extension]] trwałą regułę **retencji źródeł**: `Sources/` jest kuratowanym zapleczem grafu, nie archiwum wszystkiego, co obejrzano/przeczytano; zaktualizowano [[Source YouTube Template]] i [[README]];
- po poprawkach pełny parser daje **0 nierozwiązanych linków, 0 duplikatów, 0 błędów frontmatteru, 0 niedomkniętych bloków i 0 nieosiągalnych notatek**.

## v5 — 2026-08-17

Pełny log: [[YouTube Source Import v5]]. Audyt: [[Vault Audit v5]].

- wprowadzono **twardą bramę tematyczną**: vault Idee wyklucza IT, programowanie, cybersecurity, infrastrukturę i tutoriale; AI pozostaje tylko dla pytań o inteligencję, świadomość, autonomię, naukę, prywatność, władzę, społeczeństwo i filozofię technologii;
- przetworzono **49 nowych transkrypcji**: 29 kanonicznych notatek YouTube obejmuje 31 materiałów dzięki 2 deduplikacjom; 18 materiałów odrzucono przed kanonizacją;
- 8 odrzuconych pozycji było czystym IT/technicznym AI/cyber; 10 dalszych nie wnosiło wystarczająco trwałej idei i zostało zatrzymanych przez bramę „nie-ciekawostka”;
- dodano Concepts: [[Granice wiedzy naukowej]], [[Wiedza z pośrednich śladów]], [[Prywatność inferencyjna]], [[Starzenie jako problem ewolucyjny]], [[Rezerwa poznawcza i uczenie się przez całe życie]], [[Pseudonauka, nadzieja i asymetria dowodowa]];
- dodano Debates: [[Paradoks Fermiego — cisza jako dane czy błąd założeń]] oraz [[AI — narzędzie, agent czy podmiot]];
- dodano Syntheses: [[Od śladu do wiedzy — inferencja bez bezpośredniego dostępu]] i [[Od śladów cyfrowych do prywatności inferencyjnej — Kosiński, Wylie i Harari]];
- Kosiński został połączony w jeden ciąg z Wylie'em i Hararim: **dane jawne → inferencja cech → profil → możliwa asymetria wpływu**, bez skrótu inferencja = kontrola;
- Meissner, Szybka i nowe materiały kosmologiczne rozbudowały epistemologię o rozróżnienie granic aktualnych/paradygmatycznych/zasadniczych oraz o [[Wiedza z pośrednich śladów|inferencję ze śladów]];
- materiały o świadomych snach i astrocytach rozszerzyły [[Świadomość — poziomy i perspektywy badania]], ale bez utożsamiania sieci astrocytów z „drugim podmiotem”;
- materiały o starzeniu i Kaczmarzyku rozszerzyły rozwój w biegu życia; konkretna teza o „pełnej mielinizacji po 40–50” została jawnie zatrzymana przed kanonizacją bez niezależnej weryfikacji;
- przypadek komarów włączono do [[Łańcuch przyczyn środowiskowo-historycznych]] i [[Od środowiska do instytucji — Diamond, Dunbar i Harari]] jako konkretny mediator ekologiczno-historyczny;
- case „ChatGPT odkrył fizykę” został w [[AI a odkrycie naukowe]] rozłożony na etapy procesu naukowego zamiast przyjęcia medialnej etykiety;
- wykonano audyt zakresu całego istniejącego vaultu: nie znaleziono samodzielnych notatek v4 będących czystym IT, więc nie usuwano poprawnych węzłów AI/algorytmicznych tylko z powodu nazwy;
- po v5 vault liczy **222 pliki Markdown**.

## v4 — 2026-08-17

Pełny log importu: [[YouTube Source Import v4]].

- przetworzono **33 transkrypcje YouTube** i utworzono **32 kanoniczne notatki źródłowe**; dwie wersje wykładu Artura Ekerta zostały poprawnie zdeduplikowane;
- zgodnie z decyzją użytkownika wprowadzono twardy rozdział `Sources/Books/` ↔ `Sources/YouTube/` oraz utworzono [[YouTube źródła MOC]];
- rozszerzono [[Ideas Profile Extension]] o osobny standard pracy z filmami i transkrypcjami;
- dodano **14 Concepts**, **11 Debates**, 2 nowe syntezy i [[Fizyka, informacja i rzeczywistość MOC]];
- nie podniesiono automatycznie materiałów popularnych do rangi dowodu;
- wykonano audyt: [[Vault Audit v4]].

## v3 — 2026-08-17

Pełny log importu: [[Source Import v3]].

- zaimportowano trzy nowe pełnotekstowe książki: [[Mindfck — Christopher Wylie]], [[Strzelby, zarazki, maszyny — Jared Diamond]] i [[Życie, piękna katastrofa — Jon Kabat-Zinn]];
- ponownie przesłane pliki Cialdiniego i Eriksona zweryfikowano jako identyczne z wcześniejszymi źródłami i nie utworzono duplikatów;
- dodano pojęcia [[Mikrotargeting i profilowanie psychologiczne]], [[Prywatyzacja dyskursu publicznego]], [[Uważność]] i [[Łańcuch przyczyn środowiskowo-historycznych]];
- dodano spory [[Czy mikrotargeting podważa autonomię polityczną]] oraz [[Geografia a sprawczość w historii]];
- utworzono syntezy [[Od danych do zachowania — Kahneman, Cialdini, Harari i Wylie]], [[Od środowiska do instytucji — Diamond, Dunbar i Harari]] oraz [[Autopilot, narracyjne ja i przestrzeń reakcji]];
- dodano [[Dane, algorytmy i władza MOC]] i obowiązkowy cykl integracji nowego źródła;
- wykonano audyt: [[Vault Audit v3]].

## v2 — 2026-08-17

- ustanowiono regułę kotwic źródłowych i aktywnych mostów między książkami i folderami;
- ponownie przejrzano wszystkie książki obecne w vaulcie pod kątem tych zasad;
- dodano [[Mosty między książkami — mapa przekrojowa]];
- wykonano audyt: [[Vault Audit v2]].

## v1 — 2026-08-13

Pełny raport importu: [[Project Import v1]].

- utworzono od zera problemowo-ideową architekturę vaultu;
- zaimportowano pełnotekstowo dostępne książki i źródła `discussed-only`;
- odtworzono główne wątki projektu Idee;
- utworzono warstwy Concepts / Debates / Syntheses / Thinkers;
- dodano lokalne [[Ideas Profile Extension]];
- wykonano pełny audyt techniczny: [[Vault Audit v1]].

Up: [[Home]]
