# Nmap: The Basics

Standardowe, potężne narzędzie do rekonesansu sieciowego i skanowania portów. 

## 🛠️ Podstawowe techniki skanowania
* **TCP Connect Scan (`-sT`):** Pełne nawiązanie połączenia (3-way handshake). Używane domyślnie bez `sudo`. Pozostawia ślady w logach.
* **SYN Scan (`-sS`):** Tzw. "Stealth Scan". Puka do portu i ucieka przed odpowiedzią, przez co jest trudniejszy do wykrycia. **Wymaga sudo.**
* **UDP Scan (`-sU`):** Skanowanie portów UDP (DNS, DHCP). Wolniejsze, ale kluczowe do pełnego obrazu sieci.
* **Fast Mode (`-F`):** Skanuje tylko 100 najpopularniejszych portów (zamiast standardowego 1000).

## 🔍 Wyciąganie informacji 
* **Service Detection (`-sV`):** Sprawdza dokładną wersję usługi (np. Apache 2.4.41). Kluczowe do szukania exploitów.
* **OS Detection (`-O`):** Próbuje zgadnąć system operacyjny (Linux/Windows) na podstawie zachowania stosu TCP/IP.
* **Aggressive Mode (`-A`):** "Kombo" – włącza wykrywanie wersji, systemu, skrypty NSE oraz traceroute. Bardzo głośne, ale skuteczne.

## 🛡️ Omijanie firewalli i optymalizacja
* **Skip Ping (`-Pn`):** Traktuje hosta jako aktywny, nawet jeśli nie odpowiada na pingi. Niezbędne przy skanowaniu maszyn za firewallem.
* **Timing Templates (`-T<0-5>`):** Kontrola prędkości.
    * `-T4` (Aggressive): Najlepszy balans na CTF-y/TryHackMe.
    * `-T0` (Paranoid): Ekstremalnie wolne, by uniknąć wykrycia przez IDS.
* **Port Selection (`-p`):**
    * `-p-`: Skanuje wszystkie 65 535 portów.
    * `-p80,443`: Skanuje tylko wybrane porty.

## 📊 Wyniki i Raportowanie
* **Verbosity (`-v` / `-vv`):** Wyświetla wyniki w czasie rzeczywistym. Nie musisz czekać do końca skanu, by zobaczyć pierwszy otwarty port.
* **Zapisywanie (`-oA <nazwa>`):** Zapisuje wyniki w 3 formatach naraz: Normalnym, XML (do narzędzi) i Grepable (do szybkiego filtrowania).

---
[⬅️ Poprzednia: Tcpdump](./07-Tcpdump-Basics.md) | [🏠 Spis treści ścieżki](./README.md) | [Następna lekcja: Cryptography ➡️](./09-Cryptography.md)
