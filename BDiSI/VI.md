### wstep
- vi to prastary edytor tekstowy ktory jest juz bardzo rzadko spotykany. 
- vi zostal zaprojektowany zeby byc szybkim edytorem. Stad poczatkowo jest bardzo trudny w obsludze, ale z czasem wynagradza to efektywnoscia pracy
- Zostal prawie calkowicie wyparty przez Vim czyli wersje udoskonalona
- Zarowno Vim , NeoVim jak i Vi maja to samo sterowanie wiec umiejetnosci nabyte w jednym edytorze przenosza sie na inne. 
- Kazda nowoczesna dystrybucja linuxa ma w sobie wbudowany Vim , stad warto sie go nauczyc (niektore korzystaja z Vi ale to raczej dinozaury)

## podstawy
piszac w vi przeskakujemy pomiedzy 2 trybami
1.tryb komend - klikajac [Esc] wchodzimy w tryb komend. Ten tryb pozwala nam na usuwanie tekstu, zapis pliku, wpisywanie komend, etc . 
2.tryb wpisywania - klikajac [o],[O],[i],[I],[a] lub [A] wchodzimy w tryb wpisywania ktory pozwala na wpisywanie tekstu. 

### Tryb komend - podstawowe operacje
- h - lewo
- j - dol 
- k - gora
- l - prawo

### podstawowe operacje na pliku
- :w! -zapisz plik
- :q! -wyjdz z pliku
- :wq! -zapisz plik i wyjdz z niego
- u - cofnij zmiane

### podstawowe usuwanie tekstu
- x - usun znak pod kursorem
- dw - usun slowo (parzac od kursora)
- dd - usun linie 
- D - usun reszte linii (patrzac od kursora)

### podstawowe kopiowanie i wklejanie
- p - wklej ostatnio skopiowany tekst za kursorem 
- P - wklej ostatnio skopiowany tekst przed kursorem 
- yy - skopiuj cala linie

### Rozne opcje przejscia w tryb wpisywania
- i - wejdz w tryb wpisywania w miejscu w ktorym masz kursor
- I - wejdz w tryb wpisywania na poczatku linii 
- o - wejdz w tryb wpisywania tworzac nowa linie ponizej
- O - wejdz w tryb wpisywania tworzac nowa linie powyzej
- a - wejdz w tryb wpisywania za miejscem w ktorym masz kursor
- A - wejdz w tryb wpisywania na koncu linii

## Zaawansowane poruszanie sie w trybie komend
- w - przeskocz na poczatek nastepnego slowa
- b - przeskocz na poczatek poprzedniego slowa 
- e - przeskocz na koniec nastepnego slowa 
- [Control]u - skocz strone do gory
- [Control]d - skocz strone w dol 

### Co dalej?
Po bardziej rozbudowaną wersję odsyłam do man'a: https://man.archlinux.org/man/vi.1
