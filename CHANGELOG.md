# Historia zmian (Changelog)

Wszystkie istotne zmiany w projekcie FilePilot będą dokumentowane w tym pliku.

---

## [0.9.1-beta] - 2026-07-29

### 🚀 Nowości
* **Praca w tle:** Dodano pełną obsługę zasobnika systemowego (System Tray) z menu kontekstowym (szybkie wyjście, status).
* **Pełne cofanie zmian (Undo):** Dedykowany mechanizm pozwalający jednym kliknięciem przywrócić posortowane pliki do ich oryginalnych lokalizacji.
* **Interfejs Glassmorphism:** Nowy, ciemny motyw z rozmytym tłem i neonowymi akcentami dopasowany do stylistyki Windows 11.
* **Animowany wskaźnik postępu:** Dodano 6-sekundowy pasek postępu (Framer Motion) w oknie `ProgressModal` z efektami wizualnymi Canvas Confetti po ukończeniu operacji.

### 🛠️ Poprawki i ulepszenia
* **Ochrona niedokończonych pobrań:** Silnik wykrywa pliki tymczasowe (`.crdownload`, `.part`, `.tmp`) i czeka na zakończenie pobierania przed ich przeniesieniem.
* **Ochrona struktury katalogów:** Kategoryzowane są wyłącznie pojedyncze pliki — własne podfoldery użytkownika pozostają nietknięte.
* **Optymalizacja wydajności:** Wykorzystanie Chokidar i Node.js do niezauważalnego dla procesora i RAM-u monitorowania plików w tle.

---

## [0.9.0-beta] - 2026-07-28

### 🚀 Pierwsze wydanie testowe (Initial Release)
* **Automatyczne sortowanie:** Podstawowy silnik kategoryzujący pliki trafiające do folderów *Pobrane* oraz *Pulpit*.
* **Architektura Electron + React + Vite:** Bazowa struktura aplikacji desktopowej stworzona pod system Windows (64-bit).
* **Instalator NSIS:** Przygotowanie skryptów Electron Builder do pakowania aplikacji w jednoplikowy instalator `.exe`.
