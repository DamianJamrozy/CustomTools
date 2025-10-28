# 🖼️ optimize_images.bat  
## 🇵🇱 Wersja polska

### 📘 Opis programu
**optimize_images.bat** to prosty i skuteczny skrypt wsadowy stworzony przez **Damiana Jamrożego**, służący do automatycznej **konwersji i optymalizacji obrazów** w formatach **JPG** i **PNG** do nowoczesnych, skompresowanych formatów **WEBP** oraz **AVIF**.

Program generuje zoptymalizowane wersje grafik w różnych rozdzielczościach, co jest szczególnie przydatne przy tworzeniu stron internetowych, aplikacji webowych lub materiałów promocyjnych.

---

### ⚙️ Funkcjonalności
- ✅ Automatyczna konwersja plików `.jpg` i `.png` z bieżącego katalogu  
- ✅ Tworzenie zoptymalizowanych kopii w formatach:
  - **WEBP** (jakość 82)
  - **AVIF** (jakość 48)
- ✅ Generowanie wielu rozdzielczości: `400`, `800`, `1200`, `1600` pikseli  
- ✅ Zapis wyników w folderze `optimized/`  
- ✅ Obsługa znaków UTF-8 (np. polskie znaki w nazwach plików)  
- ✅ Automatyczne sprawdzanie dostępności programu **ImageMagick**

---

### 🧩 Wymagania
- System operacyjny **Windows 10/11**
- Zainstalowany program **ImageMagick**

#### 🖥️ Instalacja ImageMagick przez CMD (winget)
Jeśli nie masz zainstalowanego programu **ImageMagick**, uruchom **Wiersz poleceń (CMD)** jako administrator i wpisz:

```cmd
winget install ImageMagick.ImageMagick
```

Po zakończeniu instalacji upewnij się, że polecenie `magick` działa:

```cmd
magick -version
```

Jeśli zobaczysz wersję programu — instalacja przebiegła pomyślnie ✅

---

### 🚀 Sposób użycia
1. Skopiuj plik `optimize_images.bat` do folderu zawierającego pliki `.jpg` lub `.png`
2. Uruchom skrypt dwukrotnym kliknięciem lub z poziomu CMD:
   ```cmd
   optimize_images.bat
   ```
3. Po zakończeniu działania skryptu utworzy się folder:
   ```
   optimized/
   ```
   Zawierający zoptymalizowane pliki w formatach `.webp` i `.avif` dla każdej rozdzielczości.

---

### 📂 Przykładowa struktura katalogu
```
/ (bieżący folder)
│
├── photo1.jpg
├── photo2.png
│
└── optimized/
    ├── photo1-400.webp
    ├── photo1-400.avif
    ├── photo1-800.webp
    ├── photo1-800.avif
    ├── photo2-1200.webp
    └── photo2-1200.avif
```

---

### 🧠 Dodatkowe wskazówki
- Możesz edytować pętlę:
  ```bat
  for %%S in (400 800 1200 1600)
  ```
  aby dodać własne rozdzielczości.
- Zmniejszenie parametru `-quality` spowoduje większą kompresję (mniejszy rozmiar pliku).
- Format **AVIF** oferuje najlepszy stosunek jakości do rozmiaru, lecz nie wszystkie przeglądarki go obsługują.

---

### 👨‍💻 Autor
**Damian Jamroży**  
Magister inżynier nauk informatycznych  
Uniwersytet Rzeszowski – Kolegium Nauk Przyrodniczych  
📅 Rok: 2025  

---

### 📜 Licencja
Ten skrypt jest udostępniany na zasadach **open-source**.  
Można go dowolnie modyfikować i używać w celach prywatnych oraz komercyjnych, z zachowaniem informacji o autorze.

---

## 🇬🇧 English Version

### 📘 Program Description
**optimize_images.bat** is a simple and efficient batch script created by **Damian Jamroży** for **automated image conversion and optimization** from **JPG** and **PNG** formats to modern compressed formats — **WEBP** and **AVIF**.

The script automatically generates optimized versions of images in multiple resolutions — ideal for web development, responsive design, or digital content optimization.

---

### ⚙️ Features
- ✅ Automatically converts `.jpg` and `.png` files from the current folder  
- ✅ Creates optimized copies in:
  - **WEBP** (`quality 82`)
  - **AVIF** (`quality 48`)
- ✅ Generates multiple sizes: `400`, `800`, `1200`, `1600` pixels  
- ✅ Saves results in the `optimized/` folder  
- ✅ UTF-8 support (Polish and special characters)  
- ✅ Checks if **ImageMagick** is installed before running

---

### 🧩 Requirements
- Operating system: **Windows 10/11**  
- Installed **ImageMagick**

#### 🖥️ Install ImageMagick via CMD (winget)
If you don’t have ImageMagick installed, open **Command Prompt (CMD)** as administrator and run:

```cmd
winget install ImageMagick.ImageMagick
```

After installation, verify it works by typing:

```cmd
magick -version
```

If you see version information — installation was successful ✅

---

### 🚀 Usage
1. Copy `optimize_images.bat` to a folder containing `.jpg` or `.png` images  
2. Run the script by double-clicking it or through CMD:
   ```cmd
   optimize_images.bat
   ```
3. The script will create a new folder:
   ```
   optimized/
   ```
   containing all optimized `.webp` and `.avif` files at various resolutions.

---

### 📂 Example Directory Structure
```
/ (current folder)
│
├── photo1.jpg
├── photo2.png
│
└── optimized/
    ├── photo1-400.webp
    ├── photo1-400.avif
    ├── photo1-800.webp
    ├── photo1-800.avif
    ├── photo2-1200.webp
    └── photo2-1200.avif
```

---

### 🧠 Tips
- You can modify the list of resolutions inside the loop:
  ```bat
  for %%S in (400 800 1200 1600)
  ```
  to suit your needs.  
- Lowering the `-quality` value increases compression (reduces file size).  
- The **AVIF** format provides the best compression ratio but may not be supported by all browsers.

---

### 👨‍💻 Author
**Damian Jamroży**  
M.Sc. Eng. in Computer Science  
University of Rzeszów – College of Natural Sciences  
📅 Year: 2025  

---

### 📜 License
This script is released under an **open-source license**.  
You are free to use and modify it for both personal and commercial purposes as long as proper credit is given to the author.

---

© 2025 Damian Jamroży
