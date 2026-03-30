# 🌐 Cisco Device (1.pkt)

* **Analiza tablic operacyjnych (L2/L3):** Weryfikacja powiązań adresów MAC z portami przełącznika (`show mac address-table`) oraz badanie logiki wyboru tras w tablicy routingu (`show ip route`) dla sieci bezpośrednio podłączonych.
* **Monitorowanie i diagnostyka interfejsów:** Sprawdzanie stanu fizycznego oraz logicznego portów (`show ip interface brief`) i weryfikacja roli interfejsów routera jako bram domyślnych (Default Gateway) poprzez testy łączności `ping`.
  
# 🌐 Cisco Device (2.pkt)

* **Konfiguracja klientów DNS:** Implementacja obsługi nazw domenowych na routerach Cisco przy użyciu poleceń `ip domain-lookup` oraz `ip name-server`, umożliwiająca komunikację z wykorzystaniem nazw hostów zamiast adresów IP.
* **Analiza mechanizmu ARP:** Weryfikacja działania protokołu Address Resolution Protocol poprzez badanie zawartości tablicy `show arp` oraz zrozumienie procesu mapowania adresów warstwy 3 na adresy fizyczne MAC w sieci lokalnej.

# 🌐 Cisco Device (3.pkt)

* **Diagnostyka usług warstwy aplikacji:** Wykorzystanie narzędzia `telnet` do weryfikacji dostępności portów i stanu usług na serwerze DNS (10.10.10.10) oraz identyfikacja problemów z łącznością TCP.
* **Weryfikacja konfiguracji serwera:** Analiza i naprawa błędów po stronie hosta usługowego, w tym przywracanie działania wyłączonych usług systemowych (DNS Service) oraz weryfikacja rekordów zasobów (Resource Records).
* **Testowanie potoku rozwiązywania nazw:** Implementacja pełnego cyklu testowego — od sprawdzenia tablicy hostów na routerze, przez odpytanie serwera, aż po końcową weryfikację łączności `ping` przy użyciu nazw domenowych.

# 🌐 Cisco Device (4.pkt)

* **Diagnostyka ścieżki routingu i interfejsów:** Wykorzystanie narzędzi `ping` oraz `traceroute` do precyzyjnej lokalizacji miejsca utraty pakietów w sieci, a następnie weryfikacja i podnoszenie wyłączonych administracyjnie portów (za pomocą komend `show ip int brief` oraz `no shutdown`).
* **Korekta konfiguracji klienta DNS na routerze:** Identyfikacja błędnie przypisanego adresu serwera nazw na urządzeniu sieciowym (R3), usunięcie wadliwych wpisów i poprawne wskazanie docelowego serwera za pomocą komend `no ip name-server` oraz `ip name-server`.
* **Weryfikacja usług warstwy aplikacji:** Testowanie dostępności usługi na serwerze docelowym (10.10.10.10) z użyciem protokołu `telnet` oraz diagnoza i fizyczne uruchomienie wyłączonej usługi DNS bezpośrednio w panelu usług (Services GUI) na serwerze.
