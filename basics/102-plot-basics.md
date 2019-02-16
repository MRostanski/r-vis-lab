# Podstawy funkcji plot - część 2

## Przygotowania

1. Użyj zestawu danych 'airquality'. 

Są to dzienne pomiary jakości powietrza w Nowym Jorku wykonane od maja do września 1973r.

Jest to 'dataframe' z 154 obserwacjami i 6 zmiennymi:


* [,1] Ozone (ppb)
* [,2] Solar R (lang)
* [,3] Wind (mph)
* [,4] Temperature (degrees F)
* [,5] Month (1--12)
* [,6] Day of month (1--31)

2. Zbadaj podstawowe statystyki zestawu.

## Ćwiczenia z funkcją plot

3. Korzystając z dotychczasowych wiadomości, wykonaj wykres pokazujący pomiary prędkości wiatru i temperatury w Nowym Jorku.

4. Korzystając z dotychczasowych wiadomości, nanieś na jeden wykres wartości dotyczące stosunku promieniowania słonecznego do ozonu w odniesieniu do temperatury. 

5. Spróbuj pokazać temperatury w danym miesiącu. Wykorzystaj następującą konstrukcję:

```
op <- par(mfrow = c(2, 2), # 2 x 2 wykresy na jednym obszarze
          pty = "s")       # kwadratowy obszar wykresu
plot(...)
plot(...)
plot(...)
plot(...)
par(op)                    # zresetuj parametry do poprzednich ustawień.
```

6. Funkcja par() służy do ustawiania parametrów przed rysowaniem wykresu. Wypróbuj par(), aby uzyskać satysfakcjonujący zestaw do używania w swoim zestawie wizualizacyjnym.

7. Wypróbuj również funkcję pairs():

```
pairs(airquality, panel = points)
```

Jako funkcji rysującej 'panel' użyj 'panel.smooth'