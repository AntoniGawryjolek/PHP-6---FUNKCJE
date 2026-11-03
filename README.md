# PHP #6 – Funkcje

Rozwiązania zadań z lekcji **„PHP: Funkcje – zadania”** (kurs PHP, technikprogramista.pl).

W tym dziale ćwiczyłem tworzenie własnych funkcji w PHP: deklarowanie funkcji, parametry wejściowe, wartości domyślne parametrów, zwracanie wartości przez `return` oraz funkcje rekurencyjne. Każde zadanie rozwiązałem jako osobną funkcję, a dane od użytkownika pobieram z formularza HTML.

## Struktura projektu

| Plik | Opis |
|------|------|
| `funkcje.php` | Wszystkie funkcje użyte w zadaniach (jedna funkcja na zadanie, każda opisana komentarzem) |
| `zadania.php` | Strona z formularzami do wszystkich 11 zadań. Dołącza funkcje przez `require_once 'funkcje.php';` |
| `README.md` | Ten opis |

Dzięki rozdzieleniu funkcji od wywołań ten sam plik z funkcjami można dołączać na wielu stronach, tak jak opisuje lekcja.

## Opis zadań

1. **SUMA** – `suma($a, $b)` oblicza i wyświetla sumę dwóch liczb całkowitych podanych przez użytkownika.
2. **PODSTAWY** – `podstawy($a, $b)` wyświetla różnicę, iloczyn i iloraz dwóch liczb (z zabezpieczeniem przed dzieleniem przez 0).
3. **KALKULATOR** – `kalkulator($a, $b, $dzialanie)` wykonuje wybrane działanie (suma, różnica, iloczyn, iloraz); wynik trafia do kontenera `<div id="wynik">`.
4. **MAKS** – `maks($a, $b, $c)` wypisuje największą z trzech liczb.
5. **WZROST** – `wzrost($w)` klasyfikuje wzrost: poniżej 150 cm niski, powyżej 180 cm wysoki, w pozostałych przypadkach średni.
6. **BMI** – `bmi($wzrost, $waga)` liczy BMI (kg/m²) i dodaje komentarz: poniżej 18,5 „za mało!”, powyżej 25 „za dużo!”, pomiędzy „OK!”; wynik w `<div id="wynik">`.
7. **STARSZY** – `starszy($data1, $data2)` porównuje dwie daty urodzenia i wypisuje, która osoba jest starsza.
8. **PRZESTĘPNY** – `przestepny($rok)` sprawdza, czy rok jest przestępny (podzielny przez 4 i niepodzielny przez 100, albo podzielny przez 400).
9. **SIŁA** – `sila($haslo)` ocenia hasło według długości (do 4 znaków słabe, do 8 średnie, od 8 mocne) oraz obecności cyfry, dużej litery, małej litery i znaku specjalnego (brak któregoś z nich oznacza hasło słabe).
10. **TRÓJKĄT** – `trojkat($a, $b, $c)` sprawdza warunek trójkąta: suma dowolnych dwóch boków musi być większa od trzeciego.
11. **SZYFR** – `szyfruj($tekst)` szyfruje tekst szyfrem Cezara z przesunięciem o 2 (a→c, k→m, z→b). Wynik pojawia się obok pola tekstowego przy każdym naciśnięciu klawisza (JavaScript `fetch` wysyła tekst do PHP).

## Uruchomienie

1. Skopiuj `funkcje.php` i `zadania.php` do tego samego katalogu serwera (np. `htdocs` w XAMPP).
2. Uruchom Apache.
3. Otwórz w przeglądarce: `http://localhost/zadania.php`.

Wymagany jest PHP w wersji 7.0 lub nowszej.
