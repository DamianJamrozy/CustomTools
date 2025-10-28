# 🖼️ optimize_images.bat

## 📘 Opis programu
**optimize_images.bat** to prosty i skuteczny skrypt wsadowy stworzony przez **Damiana Jamrożego**, służący do automatycznej konwersji i optymalizacji obrazów w formatach **JPG** i **PNG** do nowoczesnych, skompresowanych formatów **WEBP** oraz **AVIF**.

Skrypt generuje zoptymalizowane wersje obrazów w różnych rozdzielczościach, co jest szczególnie przydatne podczas przygotowywania grafik dla stron internetowych (np. responsywnych miniatur, zdjęć produktów lub banerów).

---

## ⚙️ Funkcjonalności
- ✅ Automatyczna konwersja plików `.jpg` i `.png` z bieżącego katalogu.  
- ✅ Tworzy zoptymalizowane kopie w formatach:
  - **WEBP** (`-quality 82`)
  - **AVIF** (`-quality 48`)
- ✅ Generuje wiele rozdzielczości: **400, 800, 1200, 1600 pikseli** (szerokość lub wysokość).
- ✅ Wszystkie wyniki są zapisywane w folderze `optimized/`.
- ✅ Obsługa znaków UTF-8 (np. polskie znaki w nazwach plików).
- ✅ Automatyczne sprawdzenie dostępności programu **ImageMagick**.

---

## 🧩 Wymagania
- System operacyjny **Windows**  
- Zainstalowany program **[ImageMagick](https://imagemagick.org/script/download.php)**  
  (należy dodać `magick` do zmiennej środowiskowej **PATH**)

---

## 🚀 Sposób użycia
1. Skopiuj plik `optimize_images.bat` do folderu ze zdjęciami (`.jpg` / `.png`).  
2. Uruchom skrypt dwukrotnym kliknięciem lub w wierszu poleceń:
   ```bash
   optimize_images.bat
