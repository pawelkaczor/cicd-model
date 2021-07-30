# Aspekty CI & CD

## Specyfikacja procesu wydawniczego
Specyfikacja procesu wydawniczego określa kroki jakie będą wykonywane automatycznie jeden po drugim.

Specyfikacja może przyjmować parametry wejściowe. Niektóre parametry mogą być obliczane automatycznie na podstawie zdefiniowanych reguł.  

Specyfikacja procesu powinna być wersjonowana.

**Proces wydawniczy** - proces, którego rezultatem jest aktualizacja działającego systemu na określonym środowisku.

W architekturze mikroserwisów, kontekst procesu zwykle ograniczony jest do pojedynczego serwisu.

Proces wydawniczy może korzystać z rezultatów procesu wydawniczego dla środowiska niższej rangi.

Proces wydawniczy dla środowiska produkcyjnego (środowiska najwyższej rangi) jest procesem końcowym.  


## Środowisko

Możliwość wydawania systemu na różnych środowiskach.

Możliwość tworzenia definicji procesu wydawniczego dla konkretnych środowisk.

## Automatyzacja uruchamiania procesu

Automatyczne uruchamianie procesu wydawniczego na konkretnym środowisku w wyniku określonego zdarzenia.

Przykłady zdarzeń inicjalizujących proces wydawniczych:

- (commit) zmiany w plikach źródłowych (pliki źródłowe serwisów, bibliotek, konfiguracji środowisk). Możliwość parametryzacji procesu na podstawie brancha, z którego pochodzi commit. 
- wydanie nowej wersji serwisu / biblioteki

Możliwe powinno być ręczne uruchomienie procesu wydawniczego (?)

## Notyfikacje oraz aktualna informacja o stanie środowiska
Proces wydawniczy powinien publikować informacje o rezultatach swojego działania, tj:  nowo wydanych wersjach bibliotek bądź serwisów, nowo zdeployowanych wersjach serwisów itp.

Informacja o aktualnym stanie środowiska tj. informacja o wersjach wszystkich serwisów działających na danym środowisku powinna być łatwo dostępna.
