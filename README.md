# Aspekty CI & CD

## Definiowanie procesu wydawniczego
Zdefiniowanie kroków procesu wydawniczego, które będą wykonywane automatycznie jeden po drugim.

Definicja może przyjmować parametry wejściowe. Niektóre parametry mogą być obliczane automatycznie na podstawie zdefiniowanych reguł.  

Wersjonowanie, edytowanie definicji procesu.

**Proces wydawniczy** - proces, którego rezultatem jest aktualizacja działającego systemu na konkretnym środowisku.  

## Środowisko

Możliwość wydawania systemu na różnych środowiskach.

Możliwość tworzenia definicji procesu wydawniczego dla konkretnych środowisk.

## Automatyzacja uruchamiania procesu

Automatyczne uruchamianie procesu wydawniczego na konkretnym środowisku w wyniku określonego zdarzenia.

Przykłady zdarzeń inicjalizujących proces wydawniczych:

- (commit) zmiany w plikach źródłowych (pliki źródłowe serwisów, bibliotek, konfiguracji środowisk). Możliwość parametryzacji procesu na podstawie brancha, z którego pochodzi commit. 
- wydanie nowej wersji serwisu / biblioteki

Możliwe powinno być ręczne uruchomienie procesu wydawniczego (?)

## Informacja o rezultatach procesu

Informacja zwrotna o rezultatach procesu.

Informacje o zmianach na środowisku (np. wersje komponentów / serwisów).
