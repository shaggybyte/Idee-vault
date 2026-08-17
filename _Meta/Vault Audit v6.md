---
title: "Vault Audit v6"
type: audit
status: pass-full-local
tags: [meta, audit, v6, full, scope]
reviewed: "2026-08-17"
---

# Vault Audit v6

## Wynik

**PASS — pełny audyt lokalny + pełny audyt zakresu.**

To nie jest kontynuacja audytu różnicowego v5. Aktualny stan `main` (`49ad42e83693a6d5a27ab6374bafd3afa9f6cb8d`) został wyeksportowany do lokalnego środowiska jako pełny working tree. Przed jakąkolwiek korektą porównano lokalnie Git blob SHA **wszystkich 225 plików** z rekurencyjnym drzewem GitHuba: **0 braków, 0 plików dodatkowych, 0 różnic hashy**. Następnie repozytorium dostarczone przez użytkownika jako ZIP z pełnym `.git` niezależnie potwierdziło ten sam HEAD; czysty checkout utworzony wyłącznie z lokalnej bazy obiektów Gita był bez zmian (`git status` czysty) przed zastosowaniem poprawek v6.

## Stan wejściowy v5

Pełny lokalny licznik wykazał **223 pliki Markdown**, nie 222. Różnica pochodziła z pustego `_Inbox/Notes to integrate.md`, którego wcześniejszy bilans treści nie uwzględnił jako pełnoprawnej notatki. Historycznych raportów v4/v5 nie przepisujemy; korektę zapisuje niniejszy audyt.

Stan przed poprawkami:
- 223 `.md`;
- 61 `Sources/YouTube/`;
- 15 `Sources/Books/`;
- 13 `Sources/External/`;
- 4 `Sources/Project/`;
- 46 `Concepts/`;
- 24 `Debates/`;
- 16 `Syntheses/`;
- 12 `MOCs/`;
- 10 `Thinkers/`.

## Audyt techniczny — stan wejściowy

Pełny parser wszystkich Markdown wykazał już przed poprawkami:
- **0** nierozwiązanych wikilinków;
- **0** niejednoznacznych wikilinków;
- **0** duplikatów basename;
- **0** błędów YAML/frontmatter w niepustych notatkach;
- **0** niedomkniętych bloków ``` / ~~~;
- **0** przypadkowych plików w root.

Wykrył jednak dwa problemy strukturalne:

1. **5 plików nieosiągalnych od `Home`:** `README.md`, pusty `_Inbox` oraz trzy źródła zewnętrzne dotyczące badania komisji zwolnień warunkowych. Trzy publikacje były połączone między sobą i linkowały do konceptu szumu, ale koncept nie prowadził z powrotem do klastra.
2. [[YouTube źródła MOC]] nie był kompletnym indeksem: **11 z 61** istniejących notatek YouTube nie występowało w MOC-u.

## Poprawki strukturalne

- [[Szum w osądach i higiena decyzyjna]] otrzymał jawne linki do [[Extraneous factors in judicial decisions — Danziger et al. 2011]], [[Overlooked factors in the analysis of parole decisions — Weinshall-Margel i Shapard 2011]] i [[Extraneous factors persist — Danziger et al. reply 2011]].
- [[Home]] prowadzi teraz również do [[README]] i [[Notes to integrate]].
- `_Inbox/Notes to integrate.md` otrzymał frontmatter i definicję funkcji jako **tymczasowej kolejki**, nie magazynu wiedzy.
- [[YouTube źródła MOC]] został odbudowany jako kompletny indeks zachowanej warstwy.

## Pełny audyt zakresu

Audyt zakresu objął **cały vault**, nie tylko import v5. Parser sprawdził wszystkie pliki, a warstwa źródłowa została dodatkowo przejrzana pod kątem tytułów, frontmatteru, statusu integracji, wagi, połączeń z grafem i treści notatek. Szczególną uwagę poświęcono wszystkim źródłom YouTube, bo tam ryzyko dryfu w stronę archiwum ciekawostek jest największe.

### IT / techniczne AI

**PASS.** W aktywnej warstwie `Concepts`, `Debates`, `Syntheses` i `Sources` nie znaleziono samodzielnych notatek, których główną wartością jest programowanie, API, cybersecurity, infrastruktura, implementacja modeli czy tutorial narzędziowy. Wystąpienia tych słów poza `_Meta` dotyczą jawnego opisu granicy zakresu.

Pozostawione notatki AI dotyczą trwałych pytań o inteligencję, świadomość, autonomię, predykcję, prywatność inferencyjną, władzę, proces odkrycia naukowego lub rolę agenta.

### Brama „nie-ciekawostka” i retencja

Usunięto pięć notatek źródłowych:

1. *Psychologia tłumu — Analizy Live* — `integration_weight: low`, źródło wtórne, brak unikalnego węzła; dodatkowo zawierało uproszczony model „trzech mózgów”, którego vault i tak nie propagował.
2. *Czytamy naturę 146* — `low-medium`, wielotematyczny roundup; jedyny trwały wkład (jawne omawianie ograniczeń badania) jest już lepiej reprezentowany przez inne źródła metodologiczne.
3. *Dragan i Stanowski* — `low-medium`, długa i silnie redundantna rozmowa; program nadświetlnych obserwatorów ma lepsze źródło popularne oraz publikację pierwotną i kontrźródło.
4. *Andrzej Dragan — bezczelny fizyk* — `low-medium`, ogólne uwagi o praktyce nauki są powtórzone w gęstszych materiałach, m.in. [[Co nam daje nauka — Andrzej Dragan]].
5. *Nerwowe labradory — stereotyp rasy i projekt badania* — pojedynczy ciekawy przykład metodologiczny, ale bez trwałego, unikalnego węzła; nie uzasadnia osobnej kanonicznej notatki źródłowej.

Historyczne logi zachowują informację, że materiały były przetworzone i dlaczego później zostały usunięte, ale nie pozostawiają martwych wikilinków.

Po cleanupie nie pozostały źródła YouTube z `integration_weight: low` ani `low-medium`; nie jest to przyszły wymóg automatyczny, tylko wynik tej konkretnej rewizji.

## Reguła retencji

Dodano [[Ideas Profile Extension#13. Retencja źródeł — kanon nie jest archiwum]]. Najważniejsze rozróżnienie: **import ≠ wieczysta retencja**. Niski stopień grafu jest sygnałem do przeglądu, nie automatycznym powodem usunięcia; źródło może pozostać jako unikalna kontrkotwica. Status `catalogued*` ma natomiast wymuszać późniejszą decyzję `integrate albo prune`.

## Stan końcowy v6

Po wszystkich poprawkach i dodaniu tego raportu:
- **219 plików Markdown**;
- 56 `Sources/YouTube/`;
- 15 `Sources/Books/`;
- 13 `Sources/External/`;
- 4 `Sources/Project/`;
- 46 `Concepts/`;
- 24 `Debates/`;
- 16 `Syntheses/`;
- 12 `MOCs/`;
- 10 `Thinkers/`;
- 13 plików `_Meta/`;
- 6 szablonów;
- 1 aktywny `_Inbox`.

Końcowy pełny parser:
- **0** nierozwiązanych wikilinków;
- **0** niejednoznacznych wikilinków;
- **0** duplikatów basename;
- **0** błędów YAML/frontmatter;
- **0** pustych notatek;
- **0** niedomkniętych fence'ów;
- **0** notatek nieosiągalnych od [[Home]];
- **0** notatek bez żadnego inbound linku;
- **56/56** zachowanych źródeł YouTube obecnych w [[YouTube źródła MOC]];
- **15/15** książek w [[Książki źródłowe MOC]];
- **10/10** myślicieli w [[Myśliciele MOC]];
- **4/4** materiałów projektu w [[Materiały projektu MOC]];
- root zgodny z kontraktem (`Home.md`, `Idee MOC.md`, `README.md`, `.gitignore`, `.gitattributes`).

## Status

**PASS — pełny lokalny audyt techniczny, grafowy i zakresowy zakończony.**

Up: [[Vault Changelog]]
