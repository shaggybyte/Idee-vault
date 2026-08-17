---
title: "Ideas Profile Extension"
type: meta
tags: [meta, standard]
reviewed: "2026-08-17"
---

# Ideas Profile Extension

Ta instrukcja **uzupełnia**, a nie zastępuje, `Instrukcja_agenta_bazy_wiedzy-v16.md` dla profilu Idee.

## 1. Jednostka organizacji
> **Podstawową jednostką organizacji vaultu Idee nie jest autor ani źródło, lecz pytanie, pojęcie lub spór.** Autorzy i książki są warstwą źródłową.

## 2. Cztery warstwy
1. `Concepts/` — względnie trwałe pojęcia.
2. `Debates/` — mapy sporów, rozróżnień i konkurencyjnych stanowisk.
3. `Syntheses/` — jawne wnioski łączące kilka źródeł.
4. `Sources/` + `Thinkers/` — warstwa pochodzenia i nawigacji.

## 3. Znaczniki pochodzenia
- **SOURCE CLAIM** — to rzeczywiście twierdzi źródło;
- **INTERPRETATION** — rekonstrukcja znaczenia;
- **EXTERNAL EVIDENCE** — niezależne źródła wspierają/korygują;
- **SYNTHESIS** — wniosek vaultu z wielu materiałów;
- **OPEN QUESTION** — brak rozstrzygnięcia.

## 4. Dodatkowe wartości `source_access`
- `discussed-only` — materiał omawiany bez dostępu do treści;
- `project-synthesis` — artefakt powstały w projekcie z kilku źródeł.

## 5. Nie atomizuj mechanicznie
Nowa notatka powstaje wtedy, gdy będzie rzeczywistym węzłem wielokrotnego użytku. Nie rozbijaj jednej argumentacji na dziesiątki trzyzdaniowych plików tylko po to, aby graf wyglądał gęsto.

## 6. Autor nie jest jednostką prawdy
Nie przenoś automatycznie `autor twierdzi X` do `X jest prawdą`. Notatka kanoniczna powinna przechowywać tezę, korekty, kontrargumenty i stan dowodów.

## 7. Synteza ma mieć granice
`Syntheses/` ma jawnie pokazywać, które połączenie jest wkładem vaultu. Nie wkładaj syntezy agenta w usta pojedynczego autora.

## 8. Kanoniczne repozytorium i wersjonowanie
Repozytorium `shaggybyte/Idee-vault`, gałąź `main`, jest kanoniczną roboczą wersją vaultu.

1. Zaczynaj od aktualnego `main`.
2. Wprowadzaj zmiany do wersji githubowej.
3. Po spójnym etapie wykonaj commit i zapisz go na `main`.
4. Merytoryczne wydania oznaczaj `v2`, `v3`, ... w [[Vault Changelog]].
5. Nie generuj ZIP-ów ani kopii do Biblioteki bez wyraźnej prośby.
6. W podsumowaniu podaj wersję i końcowy SHA.

## 9. Kotwice źródłowe i mosty między ideami
Interesujące cytaty i krótkie fragmenty źródeł są ważnym elementem vaultu.

1. Dodawaj `Kotwice źródłowe — cytaty i fragmenty` z krótkimi charakterystycznymi fragmentami.
2. Podawaj precyzyjną lokalizację; nie wymyślaj stron dla EPUB/MOBI.
3. Dodawaj `Dlaczego ważne:` i wikilinki do grafu.
4. Cytat ma być wejściem do grafu, nie ozdobnikiem.
5. Aktywnie szukaj mostów, napięć i podobnych mechanizmów między źródłami.
6. Własne połączenie oznacz jako **SYNTHESIS**.
7. Zachowuj kontrfragmenty i zastrzeżenia chroniące autora przed uproszczeniem.
8. Nie zamieniaj notatki w antologię.

## 10. Cykl integracji nowego źródła
**Dodanie pliku do `Sources/` nie kończy importu.**

### Etap A — identyfikacja i dostęp
1. Ustal autora, tytuł, wydanie i zakres dostępu.
2. Sprawdź duplikaty/hash, gdy możliwe.
3. Jawnie zapisz `source_access`.

### Etap B — rekonstrukcja
4. Zrekonstruuj argument, strukturę i rozróżnienia.
5. Wybierz kotwice i kontrkotwice.
6. Oddziel twierdzenia empiryczne, metafory, prognozy i normy.

### Etap C — zderzenie z grafem
7. Najpierw sprawdź istniejący `Concept`.
8. Twórz nowy tylko dla realnie nowego mechanizmu.
9. Sprawdź wpływ na `Debates`.
10. Szukaj mostów także wstecz i aktualizuj starsze notatki.

### Etap D — synteza
11. Twórz `Syntheses/` tylko dla wniosku z wielu źródeł.
12. Oznaczaj **SYNTHESIS**.
13. Nie mieszaj poziomów analizy.

### Etap E — propagacja
14. Aktualizuj MOC-y.
15. Sprawdź wpływ na starszy graf.
16. `Thinkers/` tylko dla trwałego indeksu intelektualnego.

### Etap F — kontrola jakości
17. Sprawdź wikilinki, duplikaty, frontmatter i osiągalność od [[Home]].
18. Duże importy zapisuj w `_Meta/Import Logs/`.
19. Aktualizuj [[Vault Changelog]], [[Vault Version]] i raport audytu.
20. Zakończ commitem do `main`.

### Pytania kontrolne
- Co źródło wnosi, czego wcześniej nie było?
- Które stare notatki zmienia?
- Z czym się nie zgadza lub mówi o innym poziomie problemu?
- Które fragmenty przywracają rzeczywisty głos autora?
- Czy powstał graf wiedzy, czy tylko streszczenie?

## 11. Źródła YouTube i transkrypcje

### Architektura
1. Kanoniczne notatki filmów przechowuj w `Sources/YouTube/`.
2. Nie mieszaj ich z `Sources/Books/`.
3. Utrzymuj [[YouTube źródła MOC]].
4. `Concepts/`, `Debates/` i `Syntheses/` mogą łączyć typy źródeł, ale pochodzenie ma być czytelne.

### Transkrypcja nie jest klasą dowodu
5. Transkrypcja jest warstwą dostępu do wypowiedzi, nie automatycznie publikacją naukową.
6. Rozdzielaj wypowiedź eksperta, pytanie prowadzącego, rekonstrukcję i błąd ASR.
7. `caption_type: manual` zwiększa wiarygodność brzmienia, nie prawdziwość tezy.
8. W automatycznych napisach nazwy, symbole i liczby są podatne na błąd.
9. Nie cytuj ASR jako wiernego technicznego sformułowania bez kontroli.

### Waga epistemiczna
10. Ważne twierdzenie empiryczne z filmu pozostaje **SOURCE CLAIM**, dopóki nie ma mocniejszego wsparcia.
11. Materiał ekspercki może być mapą problemu bez bycia dowodem pierwotnym.
12. Hipotezy, prognozy i stanowiska trafiają do `Debates/` / **OPEN QUESTION**.
13. Uproszczoną popularyzację można zachować z niskim priorytetem bez propagowania twierdzeń.
14. Głośne badania sprawdzaj pod kątem późniejszych korekt, jeśli są kluczowe dla kanonu.

### Kotwice i deduplikacja
15. Używaj timestampów zamiast stron.
16. Nie przechowuj pełnych transkrypcji bez osobnego powodu.
17. Duplikaty tego samego wykładu scalaj w jedną notatkę z alternatywnymi ID/URL.
18. Redundantne rozmowy tego samego eksperta mają linkować do lepszego źródła zamiast mnożyć Concepts.

### Minimalny frontmatter
`type`, `video_id`, `source_url`, `channel`, `caption_type`, `source_access`, `evidence_role`, `integration_weight`, `status`.

## 12. Brama tematyczna — czym Idee nie są

Ta reguła jest **twardą bramą przed importem**, a nie sugestią porządkową.

### 12.1. IT jest poza zakresem
Nie importuj do vaultu jako źródeł ani wiedzy kanonicznej materiałów, których główną wartością jest:
- programowanie, kod, API, biblioteki, frameworki;
- systemy operacyjne, sieci, infrastruktura, DevOps, konfiguracja;
- cybersecurity, pentesting, kryptografia wdrożeniowa i administracja bezpieczeństwem;
- tutoriale narzędziowe, workflow, benchmarki produktów;
- techniczne instrukcje budowania agentów AI, trenowania/kwantyzacji modeli lub używania generatorów obrazów.

Takie materiały należą do osobnego vaultu IT, nie do `Idee`.

### 12.2. Wyjątek AI jest wąski
AI może wejść do Idee tylko wtedy, gdy materiał wnosi **trwały problem ideowy**, np.:
- czym jest inteligencja lub świadomość;
- różnica między narzędziem, agentem i podmiotem;
- autonomia, sprawczość, odpowiedzialność i alignment jako problem filozoficzny;
- wpływ AI na epistemologię i proces odkrycia naukowego;
- asymetria wiedzy, prywatność, profilowanie, władza i instytucje;
- konsekwencje dla obrazu człowieka, kultury, polityki lub organizacji społeczeństwa.

Sama obecność słowa „AI” nie jest powodem importu.

### 12.3. Materiały mieszane
Jeżeli źródło zawiera zarówno warstwę techniczną, jak i ideową:
1. zachowaj tylko ideowo użyteczny argument i jego kontekst;
2. nie twórz notatek o implementacji tylko dlatego, że wystąpiły w tym samym filmie;
3. mały fragment ideowy nie usprawiedliwia archiwizowania całego technicznego materiału w kanonie.

### 12.4. Brama „nie-ciekawostka”
Nawet materiał naukowy spoza IT nie musi trafić do vaultu. Odrzuć go, jeśli wnosi wyłącznie jednorazowy fakt, demonstrację lub nowinkę bez trwałego mechanizmu, sporu, pytania epistemicznego albo mostu do istniejącego grafu.

### 12.5. Jak dokumentować odrzucenie
Przy dużym imporcie odrzucone materiały zapisuj **tylko w logu importu** z krótkim powodem (`out-of-scope-it`, `low-ideational-value`, `duplicate`, `too-technical`). Nie twórz dla nich osobnego MOC ani notatek-śmieci.

### 12.6. Audyt wsteczny
Po zmianie zakresu sprawdź istniejący vault. Usuń pliki czysto techniczne, popraw wikilinki i MOC-y, a materiały mieszane zredukuj do warstwy ideowej. Historia Git jest wystarczającą ścieżką odzyskania usuniętej treści.

## 13. Retencja źródeł — kanon nie jest archiwum

`Sources/` przechowuje **źródła użyteczne dla grafu**, nie wszystko, co kiedykolwiek przeczytano lub obejrzano. Import i retencja są dwoma osobnymi decyzjami: materiał może być początkowo zachowany, a późniejszy pełny audyt może wykazać, że nie zasługuje na stałe miejsce.

### 13.1. Kiedy źródło powinno zostać
Zachowaj źródło, jeżeli spełnia co najmniej jeden mocny warunek:
- dostarcza unikalnej kotwicy lub kontrkotwicy dla ważnego twierdzenia;
- realnie zmienia `Concept`, `Debate` lub `Synthesis`;
- jest wielokrotnie używanym źródłem pierwszego wyboru dla ważnego mechanizmu;
- jest szczególnie dobrym przykładem metody, błędu lub sposobu wnioskowania, którego nie zastępuje lepsze źródło;
- jest potrzebne do zachowania pochodzenia ważnego twierdzenia w kanonie.

### 13.2. Kiedy źródło można usunąć
Przy pełnym audycie rozważ usunięcie, gdy materiał:
- ma `integration_weight: low` / `low-medium` i jest redundantny wobec lepszego źródła;
- jest podłączony głównie przez MOC lub log importu, ale nie wnosi unikalnej treści do grafu;
- jest szerokim roundupem, jednorazową ciekawostką albo ilustracją bez trwałego mechanizmu;
- został zastąpiony pełniejszym materiałem tego samego autora / wykładu;
- po zmianie zakresu wpada pod [[Ideas Profile Extension#12. Brama tematyczna — czym Idee nie są|bramę tematyczną]].

Niski stopień grafu jest **sygnałem do przeglądu, nie automatycznym powodem kasowania**. Źródło może być ważne właśnie jako pojedyncza kontrkotwica.

### 13.3. Status `catalogued` jest tymczasowy
W trwałym kanonie nie przechowuj bez końca materiałów oznaczonych wyłącznie jako `catalogued*`. Przy najbliższym pełnym audycie podejmij decyzję: **integrate albo prune**.

### 13.4. Integralność po usunięciu
Po usunięciu źródła:
1. popraw MOC-y i wszystkie aktywne wikilinki;
2. w historycznych logach importu zachowaj nazwę i powód decyzji, ale nie zostawiaj martwego wikilinku;
3. ponownie sprawdź osiągalność i duplikaty;
4. nie twórz folderu „odrzucone” tylko po to, aby zachować treść — historię zapewnia Git.

### 13.5. Pełny audyt zakresu
Pełny audyt vaultu zawsze obejmuje również zakres semantyczny **wszystkich istniejących źródeł**, nie tylko najnowszego importu. Sprawdza w szczególności czyste IT, materiały AI bez warstwy ideowej, źródła `catalogued*`, niską wagę integracji, redundantne rozmowy i naukowe ciekawostki bez trwałego połączenia.

## Szablony
- [[Concept Template]]
- [[Debate Template]]
- [[Synthesis Template]]
- [[Source Book Template]]
- [[Source YouTube Template]]
- [[Thinker Template]]

Up: [[Home]]
