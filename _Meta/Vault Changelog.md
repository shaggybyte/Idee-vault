---
title: "Vault Changelog"
type: meta
tags: [meta, changelog]
reviewed: "2026-08-17"
---

# Vault Changelog

## v4 — 2026-08-17

Pełny log importu: [[YouTube Source Import v4]].

- przetworzono **33 transkrypcje YouTube** i utworzono **32 kanoniczne notatki źródłowe**; dwie wersje wykładu Artura Ekerta zostały poprawnie zdeduplikowane;
- zgodnie z decyzją użytkownika wprowadzono twardy rozdział `Sources/Books/` ↔ `Sources/YouTube/` oraz utworzono [[YouTube źródła MOC]];
- rozszerzono [[Ideas Profile Extension]] o osobny standard pracy z filmami i transkrypcjami: jakość napisów, jawny typ źródła, timestampy, deduplikacja, weryfikacja twierdzeń technicznych i oddzielenie wypowiedzi eksperta od interpretacji;
- dodano **14 Concepts**, w tym [[Świadomość — poziomy i perspektywy badania]], [[Szum w osądach i higiena decyzyjna]], [[Informacja jest fizyczna]], [[Twierdzenie Bella i lokalność]], [[Problem pomiaru kwantowego]], [[Model, formalizm i rzeczywistość]], [[Operacjonalizacja inteligencji]] i [[Granice popularyzacji i epistemiczna pokora]];
- dodano **11 Debates**, m.in. [[Kwanty a grawitacja — zgodność opisów]], [[Czy rozszerzona względność wyjaśnia strukturę kwantową]], [[Kosmologia standardowa a CCC]], [[Skąd bierze się strzałka czasu]], [[AI a odkrycie naukowe]] i [[Standaryzacja decyzji a swoboda eksperta]];
- dodano syntezy [[Od szumu do procedury — struktura decyzji]] i [[Granice intuicji — umysł, fizyka i modele]] oraz istotnie rozszerzono [[Trzy granice nieprzewidywalności]];
- utworzono [[Fizyka, informacja i rzeczywistość MOC]] i zaktualizowano istniejące MOC-y, dzięki czemu nowe źródła nie są osobnym „magazynem filmów”, tylko zasilają istniejący graf;
- zaktualizowano m.in. [[Mózg społeczny]], [[Losowość, nieoznaczoność i niewiedza]], [[Chaos deterministyczny]] oraz [[Algorytmy a samowiedza i autonomia]];
- dodano **10 notatek `Sources/External/`** dla krytycznych weryfikacji: Bell, loophole-free Bell, spór o superluminalnych obserwatorów, CCC oraz badanie decyzji komisji zwolnień warunkowych;
- nie podniesiono automatycznie materiałów popularnych do rangi dowodu: CCC, program Dragana, pomiarowa strzałka czasu i uproszczona psychologia tłumu mają jawnie ograniczony status;
- wykonano audyt: [[Vault Audit v4]].

## v3 — 2026-08-17

Pełny log importu: [[Source Import v3]].

- zaimportowano trzy nowe pełnotekstowe książki: [[Mindfck — Christopher Wylie]], [[Strzelby, zarazki, maszyny — Jared Diamond]] i [[Życie, piękna katastrofa — Jon Kabat-Zinn]];
- ponownie przesłane pliki Cialdiniego i Eriksona zweryfikowano SHA-256 jako identyczne z wcześniejszymi źródłami i **nie utworzono duplikatów**;
- dodano pojęcia [[Mikrotargeting i profilowanie psychologiczne]], [[Prywatyzacja dyskursu publicznego]], [[Uważność]] i [[Łańcuch przyczyn środowiskowo-historycznych]];
- dodano spory [[Czy mikrotargeting podważa autonomię polityczną]] oraz [[Geografia a sprawczość w historii]];
- utworzono syntezy [[Od danych do zachowania — Kahneman, Cialdini, Harari i Wylie]], [[Od środowiska do instytucji — Diamond, Dunbar i Harari]] oraz [[Autopilot, narracyjne ja i przestrzeń reakcji]];
- dodano [[Dane, algorytmy i władza MOC]] oraz zaktualizowano istniejące MOC-y, aby nowe źródła nie pozostały bibliograficznymi wyspami;
- rozszerzono [[Algorytmy a samowiedza i autonomia]], [[Od heurystyki do wpływu]] oraz [[Mosty między książkami — mapa przekrojowa]];
- dopisano do [[Ideas Profile Extension]] obowiązkowy **cykl integracji nowego źródła**: identyfikacja → rekonstrukcja → zderzenie z grafem → synteza → propagacja → audyt;
- zaktualizowano [[Source Book Template]], aby nowe importy od początku zawierały kontrkotwice, zderzenie z grafem i wpływ na starsze notatki;
- wykonano audyt: [[Vault Audit v3]].

## v2 — 2026-08-17

- ustanowiono regułę **kotwic źródłowych**: interesujące cytaty/fragmenty mają być krótkie, zlokalizowane, opisane i podłączone do grafu wiedzy;
- ustanowiono zasadę aktywnego budowania **mostów między książkami i folderami** bez osłabiania rozdziału Source / Interpretation / Synthesis;
- ponownie przejrzano wszystkie 12 książek obecnych w vaulcie pod kątem nowych zasad;
- osiem książek z pełnym dostępem tekstowym rozbudowano o kotwice, kontrfragmenty i połączenia przekrojowe;
- cztery pozycje `discussed-only` sprawdzono i jawnie pozostawiono bez cytatów, ponieważ ich pełnych tekstów nie odnaleziono w dostępnej Bibliotece;
- *Człowiek. Biografia* ma odnotowany dostęp zarówno do PDF, jak i MOBI; ważne kotwice PDF otrzymały numery stron;
- dodano [[Mosty między książkami — mapa przekrojowa]];
- wykonano audyt techniczny i źródłowy: [[Vault Audit v2]].

## v1 — 2026-08-13

Pełny raport importu: [[Project Import v1]].

- utworzono od zera problemowo-ideową architekturę vaultu;
- zaimportowano osiem pełnotekstowo dostępnych książek jako warstwę źródłową;
- dodano cztery książki tylko poruszone w projekcie jako jawne `discussed-only`;
- odtworzono główne wątki rozmów projektu Idee;
- zintegrowano artefakty `granice.html`, JSON ewolucji i wcześniejsze grafiki;
- utworzono warstwę Concepts / Debates / Syntheses / Thinkers;
- sprawdzono aktualną paleoantropologię dla problemu radiacji australopiteków i początku Homo;
- dodano lokalne [[Ideas Profile Extension]];
- wykonano pełny audyt techniczny: [[Vault Audit v1]].

Up: [[Home]]
