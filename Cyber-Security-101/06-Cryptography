## 📖 1. Podstawowe Pojęcia
* **Plaintext (Tekst jawny):** Oryginalna informacja, którą każdy może odczytać (np. treść e-maila).
* **Ciphertext (Szyfrogram):** Zaszyfrowana, nieczytelna forma danych.
* **Encryption (Szyfrowanie):** Proces zamiany tekstu jawnego w szyfrogram.
* **Decryption (Deszyfrowanie):** Odwrócenie procesu szyfrowania przy użyciu klucza.

---

## 🏛️ 2. Szyfry Klasyczne (np. Szyfr Cezara)
Najprostsza metoda polegająca na przesuwaniu liter alfabetu o stałą liczbę pozycji ($k$).

* **Wzór szyfrowania:** $c = (p + k) \pmod{26}$
* **Przykład:** Słowo `KOT` przesunięte o 3 staje się `NRW`.
* **Wniosek:** Bardzo łatwy do złamania metodą *Brute Force* (siłową).

---

## 🔑 3. Szyfrowanie Symetryczne
Używa **tego samego klucza** do szyfrowania i deszyfrowania.

| Algorytm | Status | Uwagi |
| :--- | :--- | :--- |
| **DES** | Złamany | Stary standard (56-bit), złamany w <24h. |
| **3DES** | Wycofany | Potrójny DES, wolny i przestarzały. |
| **AES** | **Standard** | Obecnie najbezpieczniejszy (128, 192, 256 bitów). |

**Główny problem:** "Key Exchange Problem" – jak bezpiecznie przekazać hasło drugiej osobie, nie dając go przechwycić?

---

## 🔓 4. Szyfrowanie Asymetryczne (Public Key Cryptography)
Używa **pary kluczy**:
1.  **Klucz Publiczny:** Udostępniasz go każdemu. Służy do **szyfrowania**.
2.  **Klucz Prywatny:** Trzymasz go w tajemnicy. Służy do **deszyfrowania**.

### Popularne algorytmy:
* **RSA:** Opiera się na trudności faktoryzacji dużych liczb (zalecane min. 2048 bitów).
* **ECC (Elliptic Curve):** Nowocześniejszy, oferuje wysokie bezpieczeństwo przy znacznie krótszych kluczach (np. 256 bitów ECC $\approx$ 3072 bity RSA).

