# Często zadawane pytania

## 1. Nie pojawia się okno dialogowe
Ten mod wymaga dodatkowego programu backendowego do działania. Pobierz zlokalizowany program backendowy tutaj: [https://github.com/szmania/Voices_of_the_Court/releases/latest](https://github.com/szmania/Voices_of_the_Court/releases/latest). Pobrany plik .exe zainstaluje się automatycznie po otwarciu.

## 2. Problemy z konfiguracją API
Zaleca się korzystanie z oficjalnego API DeepSeek. W menu rozwijanym połączenia modelu dialogowego wybierz stronę `custom(openai-compatible)`, aby skonfigurować:
- Adres URL serwera: `https://api.deepseek.com/beta`
- Klucz API: Wprowadź własny klucz API, o który można ubiegać się na stronie [https://platform.deepseek.com](https://platform.deepseek.com).

OpenAI i OpenRouter również powinny być kompatybilne.

## 3. Okno dialogowe nie pojawia się nawet wtedy, gdy program backendowy działa po instalacji
**Rozwiązanie**: Musisz użyć moda lokalizacyjnego.

Metody instalacji (wybierz jedną):
1. Po wypakowaniu pobranych plików moda lokalizacyjnego, nadpisz oryginalne pliki moda bezpośrednio w katalogu Steam Workshop.
2. Umieść wypakowany folder moda `voices_of_the_court_mod-1.2.1-beta` w folderze modów gry. Następnie użyj Notatnika, aby utworzyć nowy plik o nazwie `voices_of_the_court_mod-1.2.1-beta.mod` w folderze `Documents\Paradox Interactive\Crusader Kings III\mod` o następującej treści:
version="1.0"
tags={
"Gameplay"
}
name="Voices of the Court mcc"
supported_version="1.13.1"
path="C:/Users/ [Twoja nazwa użytkownika PC] / Documents/Paradox Interactive/Crusader Kings III/mod/voices_of_the_court_mod-1.2.1-beta"

Jeśli okno dialogowe nadal nie pojawia się po zainstalowaniu i włączeniu moda lokalizacyjnego, ścieżka folderu użytkownika CK3 może być ustawiona nieprawidłowo lub gra może być w trybie Ironman. Ten mod nie działa w trybie Ironman.

## 4. Błąd "TypeError: Cannot read properties of undefined (reading 'playerID')" z czerwonym tekstem podczas otwierania okna czatu
**Rozwiązanie**: Utwórz folder o nazwie `run` w `Documents\Paradox Interactive\Crusader Kings III`. Wejdź do tego folderu i utwórz plik tekstowy o nazwie `votc.txt`.

## 5. Ostatnie wspomnienia nie są odczytywane podczas rozmowy z postaciami
**Rozwiązanie**:
1. Jest to mały błąd w programie backendowym oryginalnego autora; pobranie zlokalizowanego backendu rozwiązuje ten problem.
2. Może to być również spowodowane limitami tokenów pamięci. Dostosuj rozmiar `max memory tokens` na stronie ustawień programu backendowego. Po dostosowaniu tokenów pamięci należy również zwiększyć `max new tokens`; najlepiej, jeśli `max new tokens` jest większe niż `max memory tokens`.

## 6. Skrypt generowania promptów powraca do stanu pierwotnego po zrestartowaniu programu backendowego
**Rozwiązanie**:
Zapisz go jako oddzielny plik w folderze `custom`.
