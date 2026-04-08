# HUMBLE ONE – Discord Fleet Controller (DEMO)

Humble One to zaawansowane centrum zarządzania flotą kont Discord (self-botów), zaprojektowane z myślą o wysokiej wydajności, stabilności oraz przejrzystym interfejsie użytkownika (hUmble UI).  
Wersja DEMO prezentuje kluczowe mechanizmy zarządzania połączeniami i kontrolą floty.

---

## Kluczowe funkcje wersji DEMO

### 1. Sequential Strike Force (System dołączania)
Humble One wykorzystuje sekwencyjny algorytm dołączania zamiast standardowych metod równoległych. Konta dołączają jedno po drugim z precyzyjnym opóźnieniem (Stagger Join), co zwiększa stabilność połączeń bez potrzeby użycia proxy.

- **Obsługa zaproszeń:** aplikacja automatycznie rozpoznaje link lub ID kanału  
- **Auto-Guild Join:** automatyczne dołączanie do serwera przed wejściem na kanał głosowy  

### 2. Unkickable Protocol (Auto-Rejoin)
System monitoruje stan sesji w czasie rzeczywistym. W przypadku wyrzucenia konta z kanału, następuje natychmiastowe ponowne połączenie.  
Rozłączenie następuje wyłącznie po wydaniu polecenia przez użytkownika.

### 3. Fleet Manager i zarządzanie flotą
Zintegrowany panel umożliwia kontrolę wszystkich kont jednocześnie:

- **Mute/Deafen All** – synchronizacja mikrofonów i słuchawek  
- **Instant Disconnect** – natychmiastowe rozłączenie wszystkich sesji  
- **Real-time Status** – podgląd aktywności kont w czasie rzeczywistym  

### 4. Telemetria w czasie rzeczywistym
Panel statystyk odświeżany co sekundę prezentuje:

- zużycie zasobów  
- opóźnienia API (latency)  
- uptime aplikacji  

---

## Bezpieczeństwo i technologia

- **Code Obfuscation:** zabezpieczenie kodu (CFF, RC4, SE)  
- **Portable EXE:** aplikacja działa bez instalacji, zawiera wszystkie wymagane biblioteki  
- **Local Storage Persistence:** możliwość zapamiętania tokenów i danych logowania  

---

## Uruchomienie wersji DEMO

1. Pobierz plik `Humble One 0.0.2.exe` z release  
2. Uruchom aplikację  
3. Zaloguj się używając klucza demo który znajdziesz na discord: (https://discord.gg/WsCPzHZ79P)
4. W zakładce Settings wprowadź tokeny (limit: 5 w wersji demo)  
5. W zakładce Fleet podaj link zaproszenia lub ID kanału i kliknij „Deploy” (przy pierwszym uruchomieniu aplikacji i wprowadzeniu tokenów może być wymagane włączenie inicjalizacji tokenów) 
<img width="1919" height="1028" alt="image" src="https://github.com/user-attachments/assets/e619c4ab-11ac-4eba-bf68-271c89eb11dd" />

---

## Pełna wersja (w przygotowaniu)

Wersja DEMO stanowi ograniczoną wersję możliwości systemu. Pełna wersja będzie zawierać:

- rozszerzone mechanizmy operacyjne (m.in każde konto na innym proxy) 
- zaawansowane zarządzanie audio  
- brak limitu kont  
- synchronizację konfiguracji w chmurze  
- dodatkowe mechanizmy optymalizacji i zarządzania flotą w tym (flood/massdm) 

---

## Wymagania systemowe i zależności – Humble One

### System operacyjny
- Windows 10 lub nowszy (64-bit)  
- Alternatywnie macOS / Linux dla wersji developerskiej (Node.js)

### Sprzęt
- Procesor: minimum 4 rdzenie  
- RAM: 8 GB lub więcej (zalecane 16 GB dla większej floty)  
- Dysk: minimum 500 MB wolnego miejsca  
- Stałe połączenie z Internetem

### Oprogramowanie i zależności
- **Node.js**: wersja 18 lub wyższa  
- **npm**: do zarządzania pakietami Node.js (zazwyczaj dołączony do Node.js)  
- **FFmpeg**: do obsługi audio (wbudowane w EXE w wersji portable)  
- **Sodium** (libsodium): do szyfrowania audio i tokenów (wbudowane w EXE)  

### Uprawnienia
- Możliwość uruchamiania plików `.exe`  
- Uprawnienia do połączenia z Internetem (porty TCP/UDP dla Discord API)  
- Dostęp do lokalnego systemu plików do przechowywania tokenów (jeśli włączone "Remember Credentials")  

### Opcjonalnie (dla środowiska developerskiego)
- Git – do pobrania repozytorium z GitHub  
- Edytor kodu, np. Visual Studio Code  
- Terminal / PowerShell / CMD do uruchamiania skryptów Node.js  

### Uwagi
- Wersja DEMO działa z limitem 5 tokenów.  
- Pełna wersja wymaga konfiguracji w zakładce Settings i może obsługiwać setki tokenów jednocześnie.  
- Twórca nie ponosi odpowiedzialności za użycie programu w celach innych niż edukacyjne i testowe.

### VirusTotal

<img width="1906" height="916" alt="image" src="https://github.com/user-attachments/assets/e1ba1155-5b82-44a5-a00a-5667f1b6a2cb" />

- https://www.virustotal.com/gui/file/c6703929fac78649890d1ea465e8e4cecf6b15afce3c7f7ff8e954dfcb3907d8?nocache=1
-------------------------------------------------------
© 2026 Humble One. Wszelkie prawa zastrzeżone.

Humble One jest udostępniony na warunkach licencji MIT. Użycie programu jest dozwolone wyłącznie w celach edukacyjnych, testowych oraz zgodnych z prawem. Twórca nie ponosi odpowiedzialności za jakiekolwiek szkody wynikłe z użycia programu w innych celach.

---
