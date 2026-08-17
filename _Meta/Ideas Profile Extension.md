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

## 10. Cykl integracji nowego źródła

**Dodanie pliku do `Sources/` nie kończy importu.** Nowe źródło ma zostać przepuszczone przez istniejący graf wiedzy i — jeśli rzeczywiście wnosi nową treść — może zmienić starsze notatki.

### Etap A — identyfikacja i dostęp

1. ustal autora, tytuł, wydanie i faktyczny zakres dostępu;
2. przed utworzeniem notatki sprawdź, czy źródło lub identyczny plik nie jest już w vaulcie; przy podejrzeniu duplikatu porównaj hash, jeśli pliki są dostępne;
3. jawnie zapisz `source_access`; nie rekonstruuj brakującej treści z pamięci.

### Etap B — rekonstrukcja źródła

4. zrekonstruuj główny argument, strukturę oraz najważniejsze rozróżnienia;
5. wybierz kotwice źródłowe i **kontrkotwice**: fragmenty, które chronią autora przed zbyt prostą interpretacją;
6. oddziel twierdzenia empiryczne, metafory, prognozy i normatywne wnioski.

### Etap C — zderzenie z grafem

7. dla każdej ważnej idei sprawdź najpierw, czy istnieje już `Concept` opisujący ten sam mechanizm innym językiem;
8. jeśli źródło naprawdę wnosi nowe pojęcie, utwórz nowy `Concept`; jeśli tylko rozwija istniejące — aktualizuj stary;
9. sprawdź, czy nowe źródło wspiera istniejący `Debate`, dodaje stanowisko, ujawnia pozorną sprzeczność albo wymusza utworzenie nowego sporu;
10. szukaj mostów także **wstecz**: nowe źródło może wymagać dopisania linku lub korekty w starszej notatce.

### Etap D — synteza

11. twórz `Syntheses/` tylko wtedy, gdy z połączenia co najmniej dwóch źródeł powstaje użyteczny wniosek, którego nie należy przypisać pojedynczemu autorowi;
12. jawnie oznacz taki wkład jako **SYNTHESIS**;
13. nie wygładzaj realnych różnic między poziomami analizy — np. psychologia jednostki, sieć społeczna, instytucja i makrohistoria mogą opisywać różne warstwy tego samego procesu.

### Etap E — propagacja i nawigacja

14. zaktualizuj odpowiednie MOC-y;
15. sprawdź, czy nowa wiedza zmienia starsze Concepts / Debates / Syntheses / Sources;
16. dodaj autora do `Thinkers/` tylko wtedy, gdy ma wartość jako trwały indeks intelektualny, a nie wyłącznie metadane bibliograficzne.

### Etap F — kontrola jakości

17. sprawdź wikilinki, duplikaty nazw, frontmatter i osiągalność od [[Home]];
18. w imporcie większej partii źródeł zapisz krótki log w `_Meta/Import Logs/`;
19. zaktualizuj [[Vault Changelog]], [[Vault Version]] i — przy wydaniu merytorycznym — raport audytu;
20. zakończ pracę commitem do kanonicznego `main`.

### Pytania kontrolne przed zamknięciem importu

- **Co to źródło wnosi, czego wcześniej nie było?**
- **Które stare notatki zmienia?**
- **Z czym się nie zgadza albo mówi o innym poziomie tego samego problemu?**
- **Które cytaty/fragmenty najlepiej przywracają rzeczywisty głos autora?**
- **Czy stworzyliśmy graf wiedzy, czy tylko kolejne streszczenie książki?**

## 11. Źródła YouTube i transkrypcje

Źródła audiowizualne są w profilu Idee **osobną warstwą pochodzenia**, a nie rozszerzeniem folderu książek.

### Architektura

1. wszystkie kanoniczne notatki dotyczące filmów, wykładów, podcastów i rozmów YouTube przechowuj w `Sources/YouTube/`;
2. **nie mieszaj** ich z `Sources/Books/`, nawet gdy film omawia książkę;
3. utrzymuj wspólną mapę [[YouTube źródła MOC]], aby dało się przeglądać korpus źródeł audiowizualnych niezależnie od grafu pojęć;
4. w `Concepts/`, `Debates/` i `Syntheses/` można łączyć wiedzę z książek, YouTube i publikacji, ale typ źródła musi pozostać czytelny.

### Transkrypcja nie jest klasą dowodu

5. transkrypcja jest **warstwą dostępu do wypowiedzi**, nie automatycznie publikacją naukową ani dowodem równym książce akademickiej;
6. rozdzielaj co najmniej: wypowiedź eksperta, pytanie lub parafrazę prowadzącego, własną rekonstrukcję oraz ewentualny błąd rozpoznawania mowy;
7. `caption_type: manual` zwiększa wiarygodność brzmienia tekstu względem `automatic`, ale nie zwiększa samo z siebie wiarygodności merytorycznej tezy;
8. przy automatycznych napisach techniczne nazwy, symbole, nazwiska i wartości liczbowe traktuj jako podatne na błąd. Jeśli szczegół jest ważny, weryfikuj go w nagraniu albo źródle pierwotnym;
9. nie cytuj automatycznego ASR jako wiernego sformułowania technicznego bez dodatkowej kontroli. Dla integracji pojęciowej preferuj parafrazę.

### Waga epistemiczna

10. ważne twierdzenie empiryczne z wykładu lub podcastu pozostaje **SOURCE CLAIM**, dopóki nie zostanie wsparte źródłem pierwotnym albo wiarygodną literaturą;
11. materiały eksperckie mogą być bardzo wartościowe jako mapa problemu, argument, interpretacja i wskazanie literatury, ale nie ukrywaj ich formatu w notatce kanonicznej;
12. nieortodoksyjna hipoteza, prognoza technologiczna lub stanowisko filozoficzne powinny trafić do `Debates/` jako stanowisko / **OPEN QUESTION**, a nie zostać wygładzone do faktu;
13. wtórne komentarze, materiały inwestycyjne lub silnie uproszczone popularyzacje można zachować jako źródła niskiego priorytetu bez propagowania ich wszystkich twierdzeń do kanonu;
14. gdy film przywołuje głośne badanie, sprawdź, czy późniejsza literatura nie zmieniła jego interpretacji. Jeżeli istnieje realny spór, zapisz kontrkotwicę.

### Kotwice i deduplikacja

15. w źródłach YouTube używaj **timestampów** zamiast stron;
16. nie przechowuj pełnych transkrypcji w vaulcie, jeśli nie ma ku temu osobnego powodu — wystarczy mapa argumentu, kotwice czasowe, ograniczenia i link do źródła;
17. jeśli dwie transkrypcje lub dwa uploady odnoszą się do tego samego wykładu, utwórz jedną kanoniczną notatkę i zachowaj alternatywne `video_id` / URL / zakres dostępu;
18. różne rozmowy tego samego eksperta nie są automatycznie duplikatami, ale przy dużej redundancji materiał pomocniczy powinien linkować do lepszego źródła zamiast mnożyć identyczne Concepts.

### Minimalny frontmatter

Dla nowej notatki YouTube zapisuj co najmniej:

- `type: youtube-source`;
- `video_id` i `source_url`;
- `channel` i — gdy istotne — `speakers`;
- `caption_type`;
- `source_access` (`transcript-full`, `transcript-partial`, `video-only`);
- `evidence_role`;
- `integration_weight`;
- `status`.

Szablon: [[Source YouTube Template]].

## Szablony

- [[Concept Template]]
- [[Debate Template]]
- [[Synthesis Template]]
- [[Source Book Template]]
- [[Source YouTube Template]]
- [[Thinker Template]]

Up: [[Home]]
