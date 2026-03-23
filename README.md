# Cisco Device (basics1.pkt)
Dokumentacja techniczna z analizy operacyjnej przełączników (L2) i routerów (L3) w środowisku Cisco IOS.
## 1. Analiza Tablicy Adresów MAC (Layer 2)
Skupienie na procesie budowania tablicy CAM (Content Addressable Memory) przez przełącznik:
* [cite_start]**Weryfikacja mapowania:** Analiza powiązań adresów fizycznych z portami przy użyciu `show mac address-table`[cite: 11].
* [cite_start]**Proces uczenia (Learning):** Obserwacja dynamicznego uzupełniania tablicy po zainicjowaniu ruchu ICMP między hostami[cite: 11].
* [cite_start]**Zarządzanie wpisami:** Rozróżnienie między wpisami dynamicznymi a statycznymi w pamięci przełącznika[cite: 11].

## 2. Funkcje Routera i Tablica Routingu (Layer 3)
Badanie procesu podejmowania decyzji o przekazywaniu pakietów na poziomie sieciowym:
* [cite_start]**Status interfejsów:** Monitorowanie stanu fizycznego i logicznego portów poleceniem `show ip interface brief`[cite: 11].
* [cite_start]**Interpretacja tras:** Analiza tablicy routingu (`show ip route`) pod kątem sieci bezpośrednio podłączonych (C) oraz lokalnych (L)[cite: 11].
* [cite_start]**Forwarding:** Zrozumienie mechanizmu wyboru trasy na podstawie docelowego adresu IP w nagłówku pakietu[cite: 11].

## 3. Diagnostyka i Weryfikacja Łączności
Praktyczne sprawdzenie przepływu danych w topologii:
* [cite_start]**Testy ICMP:** Wykorzystanie narzędzia `ping` do weryfikacji pełnej ścieżki komunikacji (end-to-end)[cite: 11].
* [cite_start]**Brama Domyślna:** Potwierdzenie roli interfejsów routera jako punktów wyjścia dla hostów z różnych podsieci[cite: 11].
