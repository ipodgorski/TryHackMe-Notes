# Notatki: Linux Fundamentals

Zrozumienie systemu Linux jest kluczowe, ponieważ większość serwerów i narzędzi bezpieczeństwa opiera się na tym systemie.

### Kluczowe koncepcje:
* **System uprawnień:** Każdy plik ma właściciela, grupę i uprawnienia (Read, Write, Execute).
* **Struktura katalogów:** Zrozumiałem rolę katalogów `/etc` (konfiguracja), `/var/log` (logi systemowe) oraz `/home`.

### Przydatne polecenia (CLI):
* `ls -la` – pokazuje ukryte pliki i szczegółowe uprawnienia (kluczowe przy szukaniu luk w konfiguracji).
* `cat /etc/passwd` – przeglądanie użytkowników systemu.
* `find / -perm -u=s -type f 2>/dev/null` – szukanie plików z bitem SUID (częsty wektor eskalacji uprawnień).

### Wniosek:
W bezpieczeństwie Linux to nie tylko system operacyjny, to środowisko pracy. Najważniejsza lekcja: nigdy nie pracuj jako `root`, jeśli nie jest to absolutnie konieczne.
