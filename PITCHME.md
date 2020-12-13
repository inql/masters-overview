---
marp: true
theme: simple
class:
  - lead
paginate: true
header: 'Programowanie generyczne algorytmów z wykorzystaniem języka C++'
footer: 'Dawid Bińkuś'
---
<!-- _class: invert -->
# Programowanie generyczne algorytmów
##### z wykorzystaniem języka C++
###### Dawid Bińkuś - Uniwersytet Gdański

---
# Zagadnienia
- Cel pracy magisterskiej
- Funkcjonalności języka C++ w kontekście generyczności
- Wybór algorytmów
- Środowisko testowe
- Egzekucja badań

---
## Cel pracy magisterskiej
- Zgłębienie tematu programowania generycznego na przykładzie języka C++
- Przegląd funkcjonalności umożliwiających programowanie generyczne
- Analiza wpływu zastosowania generyczności (wydajność, poprawność)
---
## Funkcjonalności języka C++ w kontekście generyczności
- Szablony
- Klasy cech i wytycznych
    - type_traits
- SFINAE
- Variadic templates
- Fold expressions (C++17)
- Krotki
- Sekwencje indeksów
---
## Wybór algorytmów
- Arytmetyka wielomianów
- Operacje na macierzach
- Algorytm Karacuby
- Drzewa binarne (+ podstawowe operacje)
---
### Arytmetyka wielomianów
- Podstawowe obliczenia na wielomianach
  - dodawanie
  - odejmowanie
  - mnożenie
- Dzielenie wielomianów
- GCD dla wielomianów
---
1. Implementacja bez użycia generyczności
1. Implementacja z uwzględnieniem generyczności wielomianów (templates)
---
### Operacje na macierzach
- Operacje elementarne:
  - Dodanie do jednego wiersza inny, pomnożony przez liczbę
  - Zamienianie wierszy miejscami
  - Mnożenie wiersza przez liczbę != 0
- Dodawanie macierzy
- Mnożenie macierzy przez liczbę
- Mnożenie macierzy
---
1. Implementacja macierzy bez użycia generyczności (założenie = liczby zmiennoprzecinkowe)
1. Zastosowanie generyczności (macierze mogą zawierać dowolny typ danych)
---
### Algorytm Karacuby
1. Implementacja rekurencyjna, iteracyjna.
1. Porównanie wydajności dla dużych i małych liczb.
1. Wpływ zastosowania generycznści.
---
### Drzewa binarne
- Wyszukiwanie klucza
- Wyszukiwanie min i max w drzewie
- Wyszukiwanie następnika i poprzednika
- Wstawianie oraz usuwanie klucza
- Wyważanie drzewa (drzewa czerwono-czarne)
---
### Środowisko testowe
- Wydajność
  - https://github.com/ivafanas/sltbench
  - std::chrono - własny framework do testowania
  - https://github.com/google/benchmark
- Zużycie pamięci
  - POSIX API
---
### Egzekucja badań
- Powrównianie wyników z różnych środowisk testowych
- Wykorzystanie const i constexpr w celu przyspieszenia egzekucji (o ile to możliwe)
---
# Dziękuję za uwagę