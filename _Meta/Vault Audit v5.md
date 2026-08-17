---
title: "Vault Audit v5"
type: audit
status: pass-differential
tags: [meta, audit, v5]
reviewed: "2026-08-17"
---

# Vault Audit v5

## Wynik
**PASS — audyt różnicowy + audyt zakresu.**

## Stan plików
- v4: **181** plików Markdown;
- v5 przed metaplikami wydania: **220** plików Markdown;
- po dodaniu niniejszego audytu i [[YouTube Source Import v5]]: **222** pliki Markdown.

Przyrost merytoryczny względem v4:
- **39 nowych notatek**: 29 `youtube-source`, 6 Concepts, 2 Debates, 2 Syntheses;
- **16 zmodyfikowanych notatek** merytorycznych/nawigacyjnych;
- następnie 2 nowe metapliki wydania i aktualizacja wersji/changelogu.

## Import transkrypcji
- wejście: **49** transkrypcji;
- 29 notatek źródłowych pokrywa 31 transkrypcji dzięki 2 deduplikacjom;
- 18 materiałów odrzucono przed kanonizacją;
- 8 odrzuceń `out-of-scope-it`;
- 10 odrzuceń `low-ideational-value`.

Pełny wykaz: [[YouTube Source Import v5]].

## Audyt zakresu całego vaultu
Nowa zasada [[Ideas Profile Extension#12. Brama tematyczna — czym Idee nie są]] została zastosowana także wstecz.

- Przejrzano istniejącą strukturę, MOC-y i warstwę AI/algorytmów z v4.
- **Nie stwierdzono istniejących samodzielnych notatek czysto IT, które wymagałyby usunięcia.** Dotychczasowe węzły AI/algorytmiczne dotyczą prywatności, autonomii, decyzji, inteligencji albo filozofii nauki i pozostają w zakresie.
- Nie wykonano więc sztucznych usunięć „po słowie kluczowym”.
- Nowe materiały techniczne zostały zatrzymane przed `Sources/YouTube/` i istnieją wyłącznie jako wpisy odrzucenia w logu importu.

## Deduplikacja
- `BeLG9B9AJeQ` → scalony z `d8gEbST-bdQ`;
- `S0sW4rDDcxs` → scalony z `9LtMAww1Vr0`.

## Kontrola grafu — różnicowa
- wszystkie nowe Concepts mają wejście z odpowiedniego MOC-u;
- oba nowe Debates są osiągalne z głównych MOC-ów;
- obie nowe Syntheses są linkowane z [[Idee MOC]] i MOC-ów domenowych;
- wszystkie 29 nowych `youtube-source` jest osiągalne z [[YouTube źródła MOC]];
- źródła książkowe i YouTube pozostają rozdzielone;
- nowe wikilinki zostały sprawdzone względem istniejących i nowo tworzonych basenames;
- nie wprowadzono świadomych duplikatów basename.

## Kontrola epistemiczna
- automatyczne transkrypcje nie zostały podniesione do rangi źródeł pierwotnych;
- kontrowersyjne lub czasowo zmienne twierdzenia AI pozostają `SOURCE CLAIM` / stanowiskiem;
- szerokie twierdzenia o wieku końca mielinizacji nie zostały kanonizowane jako ustalony fakt;
- *Smocze Jajo* jest jawnie oznaczone jako fikcyjny eksperyment myślowy;
- materiał o biorezonansie został wykorzystany do modelu pseudonauki i jakości dowodów, nie jako źródło porad medycznych;
- wątek „ChatGPT odkrył fizykę” został rozłożony na konkretne etapy pracy zamiast powtórzenia medialnego hasła.

## Ograniczenie audytu
Środowisko robocze nie miało bezpośredniego checkoutu repozytorium, dlatego v5 używa **audytu różnicowego na drzewie GitHub i porównaniu commitów**, a nie ponownego lokalnego parsera wszystkich 222 plików. Pełny audyt v4 był PASS; v5 kontroluje zmieniony podzbiór i jego połączenia. Przy następnym lokalnym checkoutcie warto ponownie uruchomić pełny parser wikilinków całego vaultu.

Up: [[Home]]
