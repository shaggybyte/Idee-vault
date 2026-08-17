---
title: "Vault Audit v4"
type: audit
tags: [meta, audit]
reviewed: "2026-08-17"
---

# Vault Audit v4

## Zakres

Audyt różnicowy `v3 → v4`, oparty na stanie `main` po integracji korpusu YouTube. `v3` miał pełny audyt bez brakujących wikilinków i duplikatów; tutaj sprawdzono nowo dodane i zmodyfikowane węzły oraz ich propagację do nawigacji.

## Bilans plików Markdown

- stan v3: **107** plików `.md`;
- nowe w v4: **74** pliki `.md`;
- oczekiwany stan końcowy v4: **181** plików `.md`.

Nowe pliki:

- 32 `Sources/YouTube/` z 33 wejściowych transkrypcji — jeden duplikat Ekerta scalony;
- 10 `Sources/External/`;
- 14 `Concepts/`;
- 11 `Debates/`;
- 2 `Syntheses/`;
- 2 `MOCs/`;
- 1 szablon YouTube;
- 1 log importu;
- 1 raport audytu.

## Wikilinki

**PASS — audyt różnicowy.**

- wszystkie nowe źródła YouTube prowadzą do [[YouTube źródła MOC]];
- `Home` prowadzi do [[YouTube źródła MOC]] i [[Fizyka, informacja i rzeczywistość MOC]];
- wszystkie nowe Concepts i Debates są osiągalne przez co najmniej jeden MOC lub nową syntezę;
- publikacje `Sources/External/` są podłączone z odpowiednich Concepts/Debates;
- linki dodane w zmodyfikowanych plikach mają odpowiadające basename’y w drzewie repozytorium;
- nie pozostawiono celowo notatek YouTube jako niepodłączonych bibliograficznych wysp.

## Duplikaty nazw

**PASS.** Nowe basename’y są unikalne. Dwie transkrypcje tego samego wykładu Artura Ekerta nie utworzyły dwóch kanonicznych źródeł; alternatywny `video_id` zapisano w jednej notatce.

## Frontmatter

**PASS dla nowych plików.** Każda nowa notatka Markdown ma domknięty YAML frontmatter. Źródła YouTube używają `type: youtube-source` i jawnych pól dostępu / jakości.

## Osiągalność od Home

**PASS.** Nowa gałąź fizyczno-epistemologiczna jest osiągalna przez [[Fizyka, informacja i rzeczywistość MOC]], a korpus źródłowy przez [[YouTube źródła MOC]]. Dziedzinowe MOC-y otrzymały linki wsteczne do nowych Concepts i Debates.

## Kod i składnia

- nowe pliki nie zawierają bloków kodu wymagających testu składni;
- nie wykryto celowo tworzonych plików konfiguracyjnych ani artefaktów wykonawczych;
- brak nowych przypadków niedomkniętych fence’ów w dodanej treści.

## Root i logi

**PASS.** Nie dodano przypadkowych plików do rootu. Import log znajduje się w `_Meta/Import Logs/`, audyt w `_Meta/`, szablon w `_Templates/`.

## Kontrola jakości źródeł

**PASS z oznaczonymi ograniczeniami.** Szczególnie sprawdzono cztery ryzykowne przypadki:

1. **„głodni sędziowie”** — zachowano oryginalny wynik, krytykę kolejności spraw i odpowiedź autorów; nie propagowano skrótu o glukozie jako faktu;
2. **Dragan / superluminalni obserwatorzy** — program zapisano jako spór, z kontrpracą Lake’a;
3. **CCC** — zapisano jako alternatywny program z publikacją zwolenników i negatywnymi reanalizami CMB;
4. **pomiar jako strzałka czasu** — zachowano jako stanowisko Meissnera, nie konsensus.

Dodatkowo uproszczony model „pień–układ limbiczny–racjonalna kora” z materiału o psychologii tłumu **nie został przeniesiony do kanonu**.

## Wynik

**v4 jest spójne na poziomie audytu różnicowego i gotowe do oznaczenia jako bieżąca wersja.**

Up: [[Vault Changelog]]
