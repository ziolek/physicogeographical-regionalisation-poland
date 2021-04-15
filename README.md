Regionalizacja fizycznogeograficzna Polski, zgodna z założeniami regionalizacji światowej, została w zasadzie stworzona pod koniec lat 60. XX wieku, głównie przez prof. Jerzego Kondrackiego.

# Zawartość repozytorium
Znajdziesz tu pliki YAML z podziałami (regionalizacja):
* `regionalizacja_kondracki.yaml` - regionalizacja według Jerzego Kondrackiego z modyfikacjami (aktualne nazwy z Wikipedii)

# Struktura plików YAML
W pliku YAML została odwzorowany podział na:
* prowincje
  * podprowincje
    * makroregiony
      * mezoregiony

## Przykład
```
Wyżyny Ukraińskie:
  Wyżyna Wołyńsko-Podolska:
    Wyżyna Wołyńska:
      Grzęda Horodelska: []
      Kotlina Hrubieszowska: []
      Grzęda Sokalska: []
    Kotlina Pobuża:
      Równina Bełska: []
```

# Generowanie folderów
Na bazie pliku YAML można wygenerować drzewo katalogów za pomocą narzędzia `yamldirs`.

```
$ pip3 install yamldirs
$ yamldirs regionalizacja_kondracki.yaml
```