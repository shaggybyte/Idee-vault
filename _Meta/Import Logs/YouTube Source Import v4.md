---
title: "YouTube Source Import v4"
type: import-log
tags: [meta, import, youtube]
reviewed: "2026-08-17"
---

# YouTube Source Import v4

## Zakres

- wejście: **33 transkrypcje YouTube** z Biblioteki ChatGPT;
- wynik: **32 kanoniczne notatki `youtube-source`** w `Sources/YouTube/`;
- deduplikacja: `2uMkThXsNoM` (częściowa) i `ISpyOvrMYuQ` (pełna) opisują ten sam wykład Artura Ekerta i zostały scalone w [[Informacja jest fizyczna — Artur Ekert]];
- książki pozostały w `Sources/Books/`; korpus YouTube ma osobny [[YouTube źródła MOC]].

## Metoda

Każdy materiał przeszedł kolejno: identyfikację → ocenę dostępu i jakości transkrypcji → rekonstrukcję argumentu → zderzenie z istniejącym grafem → decyzję `update / new concept / debate / support / catalogue` → weryfikację ważnych lub spornych twierdzeń.

Transkrypcja automatyczna była traktowana jako warstwa dostępu, nie jako źródło bezbłędnych cytatów technicznych.

## v4 — partia pierwsza

| # | Materiał | Dyspozycja |
|---|---|---|
| 1 | [[Czy istnieje prawdziwy przypadek — Michał Eckstein]] | **high** — aktualizacja nieprzewidywalności; nowe Bell + pomiar |
| 2 | [[Czym jest świadomość — Copernicus]] | **high** — nowy Concept + Debate o wielości świadomości |
| 3 | [[Czy nasz mózg jeszcze ewoluuje — Marek Kaczmarzyk]] | medium — koewolucja / niedopasowanie; prognozy oznaczone ostrożnie |
| 4 | [[Co zmieniło bieg ewolucji ludzkiego mózgu — Marek Kaczmarzyk]] | **high** — aktualizacja [[Mózg społeczny]]; most do Dunbara |
| 5 | [[Dojrzały mózg — Marek Kaczmarzyk]] | medium — plastyczność vs stabilizacja |
| 6 | [[Szum — Kahneman, Sibony i Sunstein — omówienie]] | **high** — szum, higiena decyzyjna; przykład sędziów zweryfikowany z kontrkrytyką |
| 7 | [[Obliczanie, inteligencja i społeczeństwo — Michael Rovatsos]] | **high** — operacjonalizacja inteligencji |
| 8 | [[W sieci algorytmów — Copernicus]] | **high** — pętla użytkownik–algorytm; aktualizacja autonomii |
| 9 | [[Teoria kwantowa vs czarne dziury — Andrzej Dragan]] | medium — wsparcie sporu kwanty–grawitacja |
| 10 | `Information is physical` `2uMkThXsNoM` | **duplicate/partial** — scalono z #23 |
| 11 | [[Stany splątane — Copernicus]] | medium — wsparcie informacji kwantowej i AI/nauki |
| 12 | [[Mechanika kwantowa i upadek starej fizyki — Andrzej Dragan]] | medium — formalizm vs ontologia; retoryka oznaczona jako interpretacyjna |
| 13 | *Andrzej Dragan — bezczelny fizyk* *(usunięto z kanonu w v6: redundancja)* | low–medium — źródło stanowiska o praktyce nauki; wysoka redundancja |
| 14 | [[Co nam daje nauka — Andrzej Dragan]] | **high** — model, formalizm, skuteczność i rozumienie |
| 15 | [[Fizyka cząstek elementarnych]] | medium–high — teoria efektywna, inferencja z detektora, estetyka vs dane |
| 16 | [[Z czym płaskoziemcy mają rację — Andrzej Dragan]] | medium — rozumienie, formalizm, epistemiczna pokora |

## v5 — partia druga

| # | Materiał | Dyspozycja |
|---|---|---|
| 17 | [[Dlaczego fizyka kwantowa działa — Andrzej Dragan]] | medium — **sporne stanowisko**, utworzono Debate i kontrźródło Lake’a |
| 18 | [[Fizyka a wiara — Krzysztof Meissner]] | medium–high — [[Nauka a metafizyka]] |
| 19 | [[Mechanika kwantowa dla humanistów — Tomasz Stebel]] | **high** — formalizm, obserwable, granica popularyzacji |
| 20 | [[Małe mózgi vs duże mózgi — Copernicus]] | medium — modele zwierzęce, świadomość, 3R |
| 21 | [[Czy AI zastąpi fizyków — Dragan i Janowski]] | medium–high — [[AI a odkrycie naukowe]]; prognozy pozostawione jako OPEN QUESTION |
| 22 | *Psychologia tłumu — Analizy Live* *(usunięto z kanonu w v6: niski przyrost ideowy / słaba jakość źródła)* | **low** — skatalogowano; uproszczonego modelu „trzech mózgów” nie propagowano |
| 23 | [[Informacja jest fizyczna — Artur Ekert]] | **high** — kanoniczny pełny zapis wykładu, scalenie z #10 |
| 24 | [[Paradoks Newcomba — Veritasium]] | **high** — teoria decyzji i precommitment |

## v6 — partia trzecia

| # | Materiał | Dyspozycja |
|---|---|---|
| 25 | [[Od Kopernika do kwantowej grawitacji]] | medium–high — modele, prostota, historia testów |
| 26 | *Dragan i Stanowski* *(usunięto z kanonu w v6: redundancja)* | low–medium — źródło pomocnicze; sporny program nie awansował do faktu |
| 27 | [[Historia kosmologii]] | medium — modele kosmologiczne i falsyfikacja stanu stacjonarnego |
| 28 | [[Mózg nie psuje się sam — Marek Kaczmarzyk]] | medium — modele świata, niedopasowanie; szerokie tezy ostrożnie |
| 29 | [[Czas — Krzysztof Meissner]] | medium — pomiarowa strzałka czasu zachowana jako **stanowisko** |
| 30 | [[Model CCC]] | medium — **hipoteza alternatywna**; dodano publikacje CCC i negatywne reanalizy CMB |
| 31 | [[Czy materia nieorganiczna może być żywa]] | medium — nowy spór definicji życia poza substratem |
| 32 | *Czytamy naturę 146* *(usunięto z kanonu w v6: materiał typu roundup bez unikalnego węzła)* | low–medium — przede wszystkim przykład dobrej komunikacji ograniczeń badań |
| 33 | [[A Simple Diagram — Space and Time]] | medium — relatywność jednoczesności; jawna granica wynik ↔ wizualizacja autora |

## Główne nowe węzły

### Concepts

Dodano 14: [[Szum w osądach i higiena decyzyjna]], [[Koewolucja gen–kultura i niedopasowanie ewolucyjne]], [[Plastyczność i stabilizacja mózgu w biegu życia]], [[Świadomość — poziomy i perspektywy badania]], [[Informacja jest fizyczna]], [[Twierdzenie Bella i lokalność]], [[Problem pomiaru kwantowego]], [[Relatywność jednoczesności]], [[Strzałka czasu]], [[Model, formalizm i rzeczywistość]], [[Operacjonalizacja inteligencji]], [[Paradoks Newcomba i precommitment]], [[Granice popularyzacji i epistemiczna pokora]], [[Teoria efektywna]].

### Debates

Dodano 11, m.in. [[Kwanty a grawitacja — zgodność opisów]], [[Czy rozszerzona względność wyjaśnia strukturę kwantową]], [[Kosmologia standardowa a CCC]], [[Formalizm a ontologia mechaniki kwantowej]], [[Skąd bierze się strzałka czasu]], [[AI a odkrycie naukowe]], [[Nauka a metafizyka]] i [[Standaryzacja decyzji a swoboda eksperta]].

### Syntheses

Dodano [[Od szumu do procedury — struktura decyzji]] i [[Granice intuicji — umysł, fizyka i modele]]; zaktualizowano [[Trzy granice nieprzewidywalności]].

## Zewnętrzna weryfikacja

Do `Sources/External/` dodano 10 krótkich notatek weryfikacyjnych dla:

- Bella i eksperymentu loophole-free;
- programu nadświetlnych obserwatorów Dragana oraz bezpośredniej krytyki Lake’a;
- CCC (nowsza praca Meissnera/Penrose’a + dwie negatywne reanalizy sygnatur CMB);
- sporu o badanie decyzji komisji zwolnień warunkowych (oryginał, krytyka i odpowiedź).

## Reguły dodane do profilu

[[Ideas Profile Extension#11. Źródła YouTube i transkrypcje]] ustanawia m.in.:

- oddzielny `Sources/YouTube/`;
- jawny typ transkrypcji i zakres dostępu;
- niższy domyślny status dowodowy względem publikacji pierwotnej;
- obowiązek oddzielania wypowiedzi eksperta, prowadzącego, ASR i interpretacji;
- deduplikację alternatywnych uploadów;
- timestampy jako kotwice;
- zakaz ukrywania w Concepts/Debates, że ważna teza pochodziła pierwotnie z YouTube.

Audyt: [[Vault Audit v4]].

Up: [[Vault Changelog]]
