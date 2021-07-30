# Aspekty CI & CD

## Specyfikacja procesu integracyjno-wydawniczo-wdrożeniowego (IWW)

Specyfikacja procesu CICD (polski skrót mojego autorstwa: IWW) określa kroki jakie będą wykonywane automatycznie jeden po drugim.

Specyfikacja może przyjmować parametry wejściowe. Niektóre parametry mogą być obliczane automatycznie na podstawie zdefiniowanych reguł.  

Specyfikacja procesu powinna być wersjonowana .


### Proces integracyjny
Proces, którego rezultatem jest przetestowany kod źródłowy komponentu przeznaczonego do wydania.

Proces integracyjny jest częścią (podprocesem) procesu wydawniczego.

### Proces wydawniczy
Proces, który tworzy a następnie publikuje/wydaje komponent. Komponenty będącę serwisami będą nastepnie wdrożone.

### Proces wdrożeniowy
Proces, którego rezultatem jest aktualizacja działającego systemu na określonym środowisku.

W architekturze mikroserwisów, kontekst procesu zwykle ograniczony jest do pojedynczego serwisu.

Proces wdrożeniowy może korzystać z rezultatów procesu wdrożeniowego dla środowiska niższej rangi.

Proces wdrożeniowy dla środowiska produkcyjnego (środowiska najwyższej rangi) jest procesem końcowym.  

## Środowisko

Możliwość wydawania systemu na różnych środowiskach.

Możliwość tworzenia definicji procesu IWW dla konkretnych środowisk.

## Automatyzacja uruchamiania procesu
Automatyczne uruchamianie procesu IWW na konkretnym środowisku w wyniku określonego zdarzenia.

Przykłady zdarzeń inicjalizujących proces IWW:

- (commit) zmiany w plikach źródłowych (pliki źródłowe serwisów, bibliotek, konfiguracji środowisk). Możliwość parametryzacji procesu na podstawie brancha, z którego pochodzi commit. 
- wydanie nowej wersji serwisu / biblioteki

## Notyfikacje oraz aktualna informacja o stanie środowiska
Proces wydawniczy powinien publikować informacje o rezultatach swojego działania, tj:  nowo wydanych wersjach bibliotek bądź serwisów, nowo zdeployowanych wersjach serwisów itp.

Informacja o aktualnym stanie środowiska tj. informacja o wersjach wszystkich serwisów działających na danym środowisku powinna być łatwo dostępna.
