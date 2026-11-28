# Dart 501 (PWA) v2
Wgraj cały folder na hosting HTTPS (Vercel, Netlify, GitHub Pages).
Telefon: Gracze -> "Utwórz pokój" (pokazuje 4-znakowy kod, wpisuje rzuty).
Laptop: Gracze -> wpisz kod -> "Wyszukaj pokój" (przełącza się w tryb ekranu).
Połączenie przez publiczny broker MQTT (broker.emqx.io), działa między dowolnymi sieciami.

## Zmiany (v10)
- Mecz zapisuje się automatycznie po wygranej (Cofnij rzut po wygranej wycofuje zapis).
- Statystyki: zakres (wszystkie / ostatnie 10 / 30 dni), wygrane %, pudła %, najlepszy leg, wykres formy, porównanie dwóch graczy.
- Kto zaczyna: wg kolejności wyboru lub losowo (Gracze -> Tryb gry).
- Poprawa rzutu w trakcie tury: dotknij chipa „Rzut 1/2/3” i wybierz poprawny rzut.
- Gracze i mecze mają drugą kopię w IndexedDB (odtwarzanie, gdy przeglądarka wyczyści localStorage).

## Zmiany (v11) – ekran TV
- Osobny układ pod telewizor: gracze po lewej, tarcza i bieżąca tura po prawej, wszystko skalowane do wysokości ekranu.
- Pełny ekran (przycisk, Enter lub F), wskaźnik połączenia, duży kod pokoju na ekranie oczekiwania.
- Tarcza zawsze widoczna: trasa zamknięcia, rzuty z bieżącej tury albo cel w Around the Clock.
- Pasek meczu: leg, sety, legi, kto zaczyna i kto rzuca. Ostatnia tura pod tarczą.
- Duże ogłoszenia: 180, High Finish, LEG, BUST. Powtórka tury na tarczy z numerami rzutów.
- Statystyki na żywo przy graczach: średnia meczu i lega, najwyższa tura, liczba 180.
- Podsumowanie meczu na pełnym ekranie. Na telefonie przycisk „Rewanż” (zaczyna drugi gracz).
