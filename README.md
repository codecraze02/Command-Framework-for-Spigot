# Command Framework for Spigot

Nowoczesny, oparty na adnotacjach framework komend dla pluginów Spigot, zaprojektowany z myślą o mocy, elastyczności i łatwości użycia. Wykorzystuje płynne API (fluent builder) do konfiguracji oraz rozszerzalny system dostawców (provider system) dla niestandardowych typów argumentów, pozwalając deweloperom pisać czystą logikę komend bez zbędnego kodu.

---
## Funkcjonalności ✨

- ✅ **Oparty na Adnotacjach:** Definiuj komendy, sub-komendy, uprawnienia i inne bezpośrednio w metodach.
- ✅ **Płynne API (Fluent Builder):** Czysty, łańcuchowy interfejs do inicjalizacji i konfiguracji frameworka.
- ✅ **Rozszerzalne Dostawcy Argumentów:** Łatwo konwertuj argumenty komend na dowolny niestandardowy typ obiektu (np. `User`, `Gildia`, `Arena`).
- ✅ **Automatyczna Rejestracja:** Rejestruj komendy pojedynczo lub automatycznie skanuj całe pakiety.
- ✅ **Komendy z Konfiguracji:** Pozwól administratorom serwera tworzyć proste komendy bezpośrednio w pliku `config.yml`.
- ✅ **Inteligentne Uzupełnianie Tabulatorem:** Kontekstowe podpowiedzi dla sub-komend, nazw graczy i niestandardowych typów.
- ✅ **Automatyczne Generowanie Pomocy:** Generuje przejrzystą wiadomość pomocy, wymieniając wszystkie komendy i ich opisy.
- ✅ **Wbudowana Walidacja:** Używaj adnotacji takich jak `@Range` i `@Length`, aby automatycznie walidować argumenty.
- ✅ **Logowanie Wydajności:** Automatycznie loguje czas wykonania każdej komendy do konsoli w celu łatwej optymalizacji.

---
## Instalacja 🚀

Ponieważ jest to samodzielny framework, a nie biblioteka hostowana w repozytorium jak Maven Central, najprostszym sposobem na dodanie go do projektu jest skopiowanie plików źródłowych.

1.  **Skopiuj kod frameworka** do swojego projektu, umieszczając go w dedykowanym pakiecie, na przykład: `com.twojplugin.framework.command`.
2.  Wymagane klasy to:
    * `CommandFramework.java`
    * `CommandManager.java`
    * `MasterCommandExecutor.java`
    * `ClassScanner.java`
    * `Configuration.java`
    * `Binder.java`
    * Wszystkie adnotacje (`Command`, `Sender`, `Param`, itp.)
    * System argumentów (`ArgumentProvider`, `CommandArgumentException`)
    * System komend z pliku konfiguracyjnego (`ConfigCommand`)

---
