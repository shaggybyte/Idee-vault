---
title: "Vault Audit v2"
type: meta
tags: [meta, audit]
reviewed: "2026-08-17"
---

# Vault Audit v2

## Zakres

Audyt wykonano po ponownym opracowaniu całej warstwy `Sources/Books/` według reguły [[Ideas Profile Extension|kotwic źródłowych i mostów między ideami]]. Kontrola obejmowała strukturę Markdown, linki wewnętrzne, dostępność notatek z `Home`, status źródeł oraz obecność kotwic w książkach pełnotekstowych.

## Wynik

**PASS**

- 89 plików Markdown po dodaniu tego raportu;
- 0 duplikatów nazw notatek;
- 0 nierozwiązanych rzeczywistych wikilinków;
- 0 plików bez poprawnie domkniętego frontmatter;
- 0 notatek nieosiągalnych ścieżką wikilinków od [[Home]];
- 12 notatek książkowych poddanych ponownemu przeglądowi;
- 8 książek ze statusem `full-text` ma sekcję `Kotwice źródłowe — cytaty i fragmenty`;
- każda z 8 książek pełnotekstowych ma 5–6 kotwic, łączących cytaty i fragmenty parafrazowane z `Dlaczego ważne` i `Mosty`;
- 4 książki `discussed-only` pozostają jawnie bez cytatów, ponieważ podczas v2 nie odnaleziono ich pełnych tekstów w dostępnej Bibliotece;
- bezpośrednie cytaty zostały celowo ograniczone do kilku krótkich kotwic; pozostałe fragmenty są parafrazowane, aby vault zachowywał funkcję mapy wiedzy, a nie kopii źródła.

## Książki pełnotekstowe sprawdzone w v2

1. [[Antykruchość — Nassim Nicholas Taleb]]
2. [[Zdeterminowany — Robert M. Sapolsky]]
3. [[Pułapki myślenia — Daniel Kahneman]]
4. [[Człowiek. Biografia — Robin Dunbar]]
5. [[21 lekcji na XXI wiek — Yuval Noah Harari]]
6. [[Niepowstrzymani — Yuval Noah Harari]]
7. [[Wywieranie wpływu na ludzi — Robert Cialdini]]
8. [[Otoczeni przez idiotów — Thomas Erikson]]

## Książki o ograniczonym dostępie

- [[Sapiens — Yuval Noah Harari]] — `discussed-only`;
- [[Homo deus — Yuval Noah Harari]] — `discussed-only`;
- [[Przyjaciele — Robin Dunbar]] — `discussed-only`;
- [[Nowa historia ewolucji człowieka — Robin Dunbar]] — `discussed-only`.

Nie rekonstruowano ich argumentów ani cytatów z pamięci. Zamiast tego notatki wskazują najbliższe pełnotekstowe źródła i istniejące węzły wiedzy.

## Kontrola jakości połączeń

Dodano przekrojową [[Mosty między książkami — mapa przekrojowa|mapę mostów między książkami]]. Szczególnie sprawdzono, czy notatki źródłowe nie kończą się na autoreferencyjnej liście pojęć, lecz prowadzą do innych warstw vaultu. Najważniejsze osie v2 to:

- Taleb ↔ Sapolsky ↔ Kahneman: nieprzewidywalność, pewność i decyzje bez jednej trafnej prognozy;
- Kahneman ↔ Cialdini ↔ Harari: skróty poznawcze, sygnały wpływu i infrastruktura danych;
- Dunbar ↔ Harari: ograniczenia sieci społecznej, mentalizacja, język, narracja i koordynacja dużych grup;
- Sapolsky ↔ Harari: metafizyczna wolna wola a model sprawczości zakładany przez instytucje;
- Erikson ↔ Kahneman: praktyczna heurystyka komunikacyjna a ryzyko nadmiernie spójnej typologii;
- Taleb ↔ Dunbar: korzyść systemu ze zmienności a koszt ponoszony przez jednostkę.

## Otwarte zadania

- Gdy pełny tekst którejś książki `discussed-only` pojawi się w Bibliotece, jej status powinien zostać podniesiony dopiero po rzeczywistym odczycie i opracowaniu kotwic.
- Przy nowych książkach stosować od razu regułę kotwic i mostów, zamiast odkładać integrację przekrojową na późniejszy refactoring.

Up: [[Vault Changelog]]
