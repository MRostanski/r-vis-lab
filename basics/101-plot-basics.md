# Podstawy funkcji plot - część 1

## Przygotowanie

1. Zaimportuj wybraną bibliotekę graficzną.

``` 
require(graphics)
```

2. Zaimportuj wymagane biblioteki.

```
require(stats)
```

3. W serii 'discoveries' umieszczono ilości "wspaniałych" wynalazków i odkryć naukowych pomiędzy 1860 i 1959.
Użyj funkcji str() i summary() celem podstawowej analizy zbioru. Możesz też stworzyć własną zmienną i przypisać jej 'discoveries'.

## Używanie funkcji plot

4. Narysuj podstawowy wykres ilości w czasie

```
plot(discoveries)
```

5. Dokonaj modyfikacji wykresu

    a) Dodaj tytuł

```
title(main = "discoveries data set")
```

    b) Zmień podpisy używając dodatkowych parametrów funkcji plot

* main
* xlab
* ylab
* sub

na przykład: plot(discoveries, ylab = "Ważne odkrycia w latach 1860-1959")

    c) Zmień typ rysowania punktów, używając wartości parametru 'type':

* p
* b
* s
* l
* n

na przykład: 

```
plot(discoveries, type = "p")
```

    d) użyj parametrów cex, cex.main, cex.axis, cex.sub i cex.lab z wartościami mniejszymi od jeden, np.: .5 

    e) użyj parametrów col oraz analogicznie col.main, itd. z wartościami "#XXXXXX", gdzie X to liczby szesnastkowe. 

    f) użyj parametru "family" z wartościami "serif", "sans" i "mono". Sprawdź, czy da się wpisać bezpośrednio nazwę czcionki.

Ciekawostka - użyj komendy demo(Hershey) aby zobaczyć demonstrację używania m.in. symboli specjalnych.

6. Sprawdź, jak działają parametry 'pch', 'las', 'lty', czy 'lend' (wartości naturalne).

7. Zwróć uwagę, że na wykresie można nałożyć dodatkowe wykresy, m. in. funkcjami 'line' i 'points'.

    a) nałóż na wykres odkryć średnią przy pomocy funkcji abline():

```
abline(h=mean(discoveries))
```

    b) narysuj wykres używając typu "n", a następnie nałóż punkty funkcją "points" lub "lines", (używając parametrów jak w funkcji plot).




