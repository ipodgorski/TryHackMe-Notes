# Moduł: Networking Essentials

Zrozumienie sposobu przesyłania danych w sieci jest kluczowe dla każdego analityka bezpieczeństwa. Ten moduł skupia się na fundamentach komunikacji.

### 1. Model OSI (Open Systems Interconnection)
Zrozumienie 7 warstw modelu OSI pozwala na precyzyjne określenie, gdzie występuje problem lub atak:
1. **Physical** (Kable, sygnały)
2. **Data Link** (Adresy MAC, Ethernet)
3. **Network** (Adresy IP, Routing)
4. **Transport** (TCP/UDP, Porty)
5. **Session** (Zarządzanie sesją)
6. **Presentation** (Formatowanie danych, szyfrowanie)
7. **Application** (HTTP, FTP, DNS)



### 2. Kluczowe Protokoły
* **DNS (Domain Name System):** Zamiana nazw domenowych na adresy IP. Analiza zapytań DNS pozwala wykryć próby łączenia się złośliwego oprogramowania z serwerami C2 (Command & Control).
* **DHCP (Dynamic Host Configuration Protocol):** Automatyczne przyznawanie adresów IP. Proces **DORA**: **D**iscover, **O**ffer, **R**equest, **A**cknowledge.
* **ICMP:** Używany przez narzędzia takie jak `ping` i `traceroute` do diagnostyki sieci.



### 3. Encapsulation (Enkapsulacja)
Proces pakowania danych w nagłówki poszczególnych warstw (np. dodawanie nagłówka IP w warstwie 3 i nagłówka TCP w warstwie 4). Zrozumienie tego procesu jest niezbędne przy analizie pakietów w Wiresharku.

### Podsumowanie:
Sieci to język internetu. Każdy incydent bezpieczeństwa zostawia ślad w sieci, dlatego biegłość w protokołach jest moim priorytetem w drodze do pracy w SOC.

---
[⬅️ Poprzednia: Command Line](./04-Command-Line.md) | [🏠 Spis treści ścieżki](./README.md) | [Następna lekcja: Wireshark ➡️](./06-Wireshark-Basics.md)
