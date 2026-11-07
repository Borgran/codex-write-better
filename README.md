# codex-write-better

`write-better` to skill dla Codex, który pomaga pisać i redagować teksty dla konkretnego odbiorcy. Możesz zacząć od kilku punktów lub wkleić gotowy szkic. Skill pomaga ustalić główną myśl, uporządkować informacje i dobrać ton do miejsca publikacji.

## Co robi

- Pisze w języku zadania i dopasowuje styl do formatu, np. maila, artykułu, ogłoszenia, opisu produktu albo instrukcji.
- Zastępuje ogólniki konkretami i usuwa powtórzenia, zachowując fakty, zastrzeżenia i głos autora. Może też dopasować brzmienie do wskazanej próbki.
- Dopytuje, jeśli brakująca informacja może zmienić treść. Ustalenia z rozmowy zostają poza tekstem, który trafia do czytelnika.

## Przykład redakcji

**Przed**

> Pragniemy poinformować mieszkańców o planowanych utrudnieniach w dostępie do wody. W związku z realizacją prac przy sieci wodociągowej w czwartek od 8.00 do 12.00 nastąpi przerwa w dostawie wody przy ul. Lipowej 4–10. W tym czasie mieszkańcy będą mogli skorzystać z beczkowozu przy Lipowej 6.

**Po**

> W czwartek od 8.00 do 12.00 przy ul. Lipowej 4–10 nie będzie wody z powodu prac przy sieci wodociągowej. W tym czasie wodę można pobrać z beczkowozu przy Lipowej 6.

W tym fikcyjnym ogłoszeniu termin i adres trafiają do pierwszego zdania. Czytelnik od razu wie, czy przerwa go dotyczy i gdzie znajdzie wodę.

## Instalacja w Codex

Pobierz repozytorium i skopiuj `SKILL.md`, `agents/` oraz `references/` do jednego katalogu `write-better`. Zachowaj układ podkatalogów.

- Dla jednego projektu umieść katalog skilla w `.agents/skills/write-better/` wewnątrz projektu.
- Dla wszystkich swoich projektów użyj `~/.agents/skills/write-better/` w katalogu domowym.

Codex wykrywa nowe skille automatycznie. Jeśli skill się nie pojawi, uruchom Codex ponownie. [Dokumentacja OpenAI dotycząca skilli](https://learn.chatgpt.com/docs/build-skills#where-codex-loads-local-skills)

## Użycie

Wpisz `$write-better` w rozmowie z Codex i opisz zadanie. Jeśli chcesz przeredagować szkic, wklej go pod poleceniem.

```text
Użyj $write-better. Przeredaguj poniższe ogłoszenie dla mieszkańców.
Zachowaj termin, adresy i informację o beczkowozie.
```

## Pliki

- [SKILL.md](SKILL.md) — instrukcje pisania i redakcji.
- [references/warsztat.md](references/warsztat.md) — techniki redakcji dłuższych tekstów i dopasowania stylu.
- [agents/openai.yaml](agents/openai.yaml) — nazwa, krótki opis i przykładowe polecenie wyświetlane w Codex.

Pomysłodawca i autor wersji 1.0 — **Piotr Boryszek (www.averta.pl)**.
