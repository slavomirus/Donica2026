# 💕 Nasz Wyjątkowy Dzień — Interaktywna Gra Terenowa

Romantyczna interaktywna gra na specjalny dzień, z odliczaniem, wyzwaniami i galerią w stylu Netflixa.

## 🚀 Jak wdrożyć na GitHub Pages

### Krok 1 — Stwórz repozytorium
1. Zaloguj się na [github.com](https://github.com)
2. Kliknij **New repository**
3. Nazwa np. `nasza-przygoda` lub `special-day`
4. Ustaw jako **Public** (wymagane dla darmowych GitHub Pages)
5. **Nie** zaznaczaj "Add a README" — wgrasz te pliki samodzielnie
6. Kliknij **Create repository**

### Krok 2 — Wgraj pliki
**Opcja A — przez przeglądarkę (najłatwiej):**
1. Na stronie repozytorium kliknij **Add file → Upload files**
2. Wgraj wszystkie pliki z tego folderu (w tym folder `.github`)
3. Kliknij **Commit changes**

**Opcja B — przez Git (terminal):**
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/TWOJ_LOGIN/NAZWA_REPO.git
git push -u origin main
```

### Krok 3 — Włącz GitHub Pages
1. Wejdź w **Settings** repozytorium
2. Przejdź do sekcji **Pages** (lewy panel)
3. W **Source** wybierz **GitHub Actions**
4. Gotowe! Deployment uruchomi się automatycznie

### Krok 4 — Znajdź swój link
Po chwili (1-2 minuty) strona będzie dostępna pod adresem:
```
https://TWOJ_LOGIN.github.io/NAZWA_REPO/
```

---

## 🎮 Funkcje aplikacji

| Ekran | Opis |
|-------|------|
| **Odliczanie** | Romantyczny timer do 5 czerwca 2026 godz. 13:00 |
| **Instrukcja** | Zasady gry z podziałem na role |
| **Wyzwania** | 15 zadań z uploadem zdjęć/video, mapami Google |
| **Finał Netflix** | Galeria wszystkich wspomnień w stylu Netflixa |

## ⚙️ Szczegóły techniczne

- **Brak buildu** — czysty HTML/CSS/JS, działa od razu
- **LocalStorage** — zdjęcia i filmy zapisywane lokalnie w przeglądarce
- **Offline-ready** — po wczytaniu działa bez internetu (poza mapami)
- **Responsywny** — działa na telefonach i komputerach

## 🧪 Testowanie

Na ekranie odliczania w prawym dolnym rogu znajdziesz przycisk **Skip Countdown** — zeruje licznik i pokazuje przyciski wyboru roli, bez czekania do 5 czerwca.

## ⚠️ Uwaga o zdjęciach

Ze względu na limit LocalStorage (~5MB per origin), duże pliki wideo mogą nie zapisać się do pamięci. Aplikacja obsługuje ten błąd gracefully — w galerii pojawi się placeholder 📼 zamiast brakującego nagrania.

---

Made with ♡
