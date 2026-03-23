## 🔑 RSA (Asymmetric Encryption)
* **Fundament:** Trudność faktoryzacji dużych liczb pierwszych.
* **Wzory:**
    * $n = p \times q$ (Moduł)
    * $\phi(n) = (p-1) \times (q-1)$ (Funkcja Eulera)
* **Klucze:** Publiczny $(n, e)$, Prywatny $(n, d)$.

## 🤝 Diffie-Hellman (Key Exchange)
* **Cel:** Bezpieczne ustalenie wspólnego klucza (Shared Secret) przez podsłuchiwany kanał.
* **Mechanizm:** Obie strony generują ten sam wynik $g^{ab} \pmod{p}$ bez przesyłania swoich kluczy prywatnych.

## 🐚 SSH (Secure Shell)
* **Klucze:** Para `id_algorithm` (prywatny) i `id_algorithm.pub` (publiczny).
* **Uprawnienia:** Klucz prywatny musi mieć `chmod 600`.
* **Pliki:** * `~/.ssh/authorized_keys` – lista kluczy publicznych z dostępem do serwera.
    * `~/.ssh/known_hosts` – odciski palców (fingerprints) znanych serwerów.
* **Komenda:** `ssh -i <klucz> <user>@<host>`

## 🖋️ Signatures & Certificates
* **Podpis Cyfrowy:** Hash wiadomości zaszyfrowany kluczem prywatnym nadawcy. Gwarantuje **integralność** i **autentyczność**.
* **Certyfikat TLS:** Klucz publiczny potwierdzony przez zaufaną trzecią stronę (CA - Certificate Authority).
* **Chain of Trust:** Przeglądarka ufa certyfikatowi, bo ufa urzędowi (Root CA), który go podpisał.

## 🔐 GPG (GnuPG)
* **Importowanie klucza:** `gpg --import <plik>`
* **Deszyfracja:** `gpg --decrypt <plik.gpg>`
* **Łamanie hasła klucza:** `gpg2john <klucz> > hash` -> `john hash`


[⬅️ Poprzednia: Cryptography](./09-Cryptography.md) | [🏠 Spis treści ścieżki](./README.md) | [Następna lekcja: Soon ➡️]()
