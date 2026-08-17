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

W treści używaj, gdy jest to istotne:

- **SOURCE CLAIM** — to rzeczywiście twierdzi źródło;
- **INTERPRETATION** — tak rekonstruujemy znaczenie;
- **EXTERNAL EVIDENCE** — niezależne źródła wspierają/korygują twierdzenie;
- **SYNTHESIS** — wniosek agenta z wielu materiałów;
- **OPEN QUESTION** — brak rozstrzygnięcia.

## 4. Dodatkowe wartości `source_access`

Oprócz standardu v16 dopuszcza się:

- `discussed-only` — materiał był omawiany, ale nie było dostępu do jego treści;
- `project-synthesis` — artefakt powstał w projekcie z kilku źródeł i nie jest źródłem pierwotnym.

## 5. Nie atomizuj mechanicznie

Nowa notatka powstaje wtedy, gdy będzie rzeczywistym węzłem wielokrotnego użytku. Nie rozbijaj jednej argumentacji na dziesiątki trzyzdaniowych plików tylko po to, aby graf wyglądał gęsto.

## 6. Autor nie jest jednostką prawdy

Nie przenoś automatycznie `autor twierdzi X` do `X jest prawdą`. Notatka kanoniczna powinna umożliwiać jednoczesne przechowanie tezy autora, korekty, kontrargumentu i aktualnego stanu dowodów.

## 7. Synteza ma mieć granice

Notatka `Syntheses/` powinna jasno pokazywać, które połączenie jest wkładem vaultu. Nie wkładaj własnej syntezy w usta jednego autora.

## 8. Kanoniczne repozytorium i wersjonowanie

Repozytorium `shaggybyte/Idee-vault`, gałąź `main`, jest **kanoniczną roboczą wersją vaultu**.

Przy każdej kolejnej pracy nad vaultem:

1. zacznij od odczytania aktualnego stanu `main`, zamiast bazować na wcześniejszym ZIP-ie lub kopii z Biblioteki;
2. wprowadzaj zmiany do wersji githubowej;
3. po zakończeniu spójnego etapu pracy wykonaj commit i zapisz go na `main`;
4. merytoryczne wydania oznaczaj kolejnymi wpisami `v2`, `v3`, ... w [[Vault Changelog]]; drobne poprawki techniczne lub workflow mogą pozostać w bieżącej wersji, jeśli nie zmieniają stanu wiedzy;
5. nie generuj kolejnych ZIP-ów ani kopii do Biblioteki ChatGPT, chyba że użytkownik wyraźnie o nie poprosi;
6. w podsumowaniu pracy podaj krótko, co zmieniono, numer wersji (jeśli wzrósł) oraz SHA końcowego commita.

## 9. Kotwice źródłowe i mosty między ideami

Interesujące cytaty i krótkie fragmenty źródeł są **ważnym elementem vaultu**, ponieważ pozwalają później wrócić do rzeczywistego języka autora zamiast pamiętać wyłącznie syntezę agenta.

Dla dobrze opracowanej książki lub ważnego materiału:

1. dodawaj sekcję `Kotwice źródłowe — cytaty i fragmenty` z krótkimi, charakterystycznymi fragmentami; wybieraj fragmenty, które rzeczywiście niosą tezę, rozróżnienie, metaforę albo ważne zastrzeżenie;
2. przy każdej kotwicy podawaj możliwie precyzyjną lokalizację: rozdział / podrozdział, a gdy format na to pozwala także stronę; nie wymyślaj numerów stron dla EPUB/MOBI;
3. pod cytatem dodawaj krótkie `Dlaczego ważne:` oraz wikilinki do powiązanych `Concepts`, `Debates`, `Syntheses`, innych książek lub `Thinkers`;
4. **cytat nie może wisieć sam** — ma być wejściem do grafu wiedzy, nie ozdobnikiem;
5. aktywnie szukaj **mostów między źródłami**: podobnych mechanizmów opisanych innym językiem, napięć między autorami, zgodności na różnych poziomach oraz pozornych sprzeczności wynikających z różnych pytań;
6. gdy połączenie między książkami jest wkładem vaultu, oznacz je jako **SYNTHESIS** i nie przypisuj go pojedynczemu autorowi;
7. zachowuj ważne kontrfragmenty i zastrzeżenia autora, zwłaszcza gdy chronią jego stanowisko przed zbyt prostą interpretacją;
8. nie zamieniaj notatki źródłowej w antologię. Cytaty mają wzmacniać mapę argumentu i połączenia, a nie zastępować streszczenie, krytykę i syntezę.

Dobrą praktyką jest, aby pełnotekstowo dostępna książka miała kilka do kilkunastu mocnych kotwic, zależnie od jej znaczenia dla vaultu.

## Szablony

- [[Concept Template]]
- [[Debate Template]]
- [[Synthesis Template]]
- [[Source Book Template]]
- [[Thinker Template]]

Up: [[Home]]
