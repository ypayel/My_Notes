# My_Notes
Rest api and mixroservices

Roznica miedzy rest api to sposob na kommunikacje pomiedzy klientem a servezem przez http requests, a mickroservice to sposob na organizacje architektury na serverze, gdzie mikroservice nie powinny wymieniac sie przez rest api

Target and current.target

current target - to element ktory załączono procedurę obsługi zdarzeń

target - gdzie wydazylo sie to zdarzenie

Jak dziala przygladarka  ?

    1.Wpisujemy URL (Uniform Resource Locator) w szukiwarku przegladarki. URL wyswietla ns strone, ktora uzytkownik chce odzwiedziec.
    2.Przegladarka wysyla DNS(Domain Name System) na DNS-server, zeby otzymac IP-adress servera, na ktorym sie znajduje strona. DNS-server przetwarza nazwe domeny (naprzyklad, [www.example.com](http://www.example.com/)) na odpowiedni IP-adress
    3.Przegladarka nawiazuje polaczenie TCP z serverem, wykorzystując otrzymany adres IP. Dzięki temu przeglądarka może wysyłać i odbierać dane z serwera
    4.Przeglądarka wysyła do serwera żądanie HTTP (Hypertext Transfer Protocol) z żądaniem wyświetlenia strony internetowej. Żądanie może zawierać różne parametry, takie jak metoda żądania (GET, POST itp.), nagłówki i treść żądania
    5.Serwer przetwarza żądanie i odsyła odpowiedź HTTP zawierającą żądaną stronę internetową. Odpowiedź może również zawierać różne nagłówki, status odpowiedzi i treść odpowiedzi

    HTTP to protokół aplikacji służący do przesyłania dokumentów hipertekstowych, takich jak HTML. Przeznaczony jest do komunikacji pomiędzy przeglądarkami internetowymi i serwerami WWW
    Request Method(**GET HEAD POST PUT DELETE CONNECT OPTIONS TRACE**
 **PATCH)

 (Headers) – to metadane, które są przesyłane wraz z żądaniem i zawierają dodatkowe informacje o żądaniu, takie jak typ zawartości, uwierzytelnianie, buforowanie i inne parametry

 Body – jest używane tylko w niektórych metodach żądania, takich jak POST lub PUT. Zawiera dane, które klient wysyła do serwera, na przykład formularz do wysłania lub obiekt JSON

 CSSOM to zestaw API, które pozwalają na modyfikowanie CSS za pomocą JavaScriptu bez konieczności przeładowywania strony

 Critical Rendering Path (CRP) – to proces, który przeglądarka wykonuje, aby przekształcić HTML, CSS i JavaScript w wizualny interfejs na ekranie użytkownika
 1.Przeglądarka otrzymuje kod HTML dokumentu z serwera
 2.Przeglądarka analizuje kod HTML i tworzy strukturę drzewa dokumentu, zwaną DOM (Document Object Model)
 3.Przeglądarka ładuje zewnętrzne pliki CSS, a także osadzone i wbudowane style niezbędne do wyglądu strony. Po załadowaniu plików CSS przeglądarka tworzy CSSOM (CSS Object Model)
 4.Przeglądarka łączy DOM i CSSOM, aby utworzyć Render Tree, który zawiera tylko te węzły DOM, które zostaną wyświetlone na ekranie, oraz odpowiadające im style
 5.Przeglądarka określa rozmieszczenie każdego elementu w Render Tree, uwzględniając jego rozmiary i pozycję.
 6.Na podstawie Render Tree i układu (layout) przeglądarka rozpoczyna renderowanie zawartości na ekranie użytkownika. Proces ten obejmuje rysowanie pikseli dla każdego wyświetlanego elementu.
 7.Przeglądarka łączy wyrenderowane warstwy (layers) i tworzy ostateczny obraz, który użytkownik widzi na ekranie

 Optymalizacja CRP odgrywa ważną rolę w tworzeniu szybko ładujących się i responsywnych stron internetowych. Obejmuje to minimalizowanie użycia zasobów, optymalizację CSS i JavaScript, a także stosowanie metod, takich jak leniwe ładowanie zasobów i asynchroniczne ładowanie skryptów, aby przyspieszyć proces renderowania strony


CORS (Cross-Origin Resource Sharing).
 Mekanizm, który wykorzystuje dodatkowe nagłówki HTTP, aby umożliwić agentowi użytkownika uzyskiwanie zezwoleń na dostęp do wybranych zasobów z serwera na źródle (domenie), innym niż ta, którą obecnie używa strona, nazywa się 



MVC (Model-View-Controller)
Wzor projektowy, który umożliwia efektywne oddzielenie modelu danych (gdzie wszystko obsługuje serwer), wyświetlania i obsługi akcji (kontroler wykonuje odpowiednie operacje i przekazuje je do widoku)

Wzorcami projektowymi (Design Patterns)
To gotowe do użycia rozwiązania często występujących problemów w programowaniu

"use strict" to dyrektywa w JavaScript, która wprowadza tryb restrykcyjny, zmieniając sposób działania języka w celu uniknięcia pewnych powszechnych błędów i poprawy bezpieczeństwa
wprowadza szereg ograniczeń, takich jak:
Zakaz używania niezadeklarowanych zmiennych.
Uniemożliwienie przypisania wartości do tylko do odczytu (np. do stałych).
Zmiana sposobu działania funkcji, w tym rozróżnianie nazw argumentów w przypadku funkcji o tej samej nazwie.

let
Służy do deklarowania zmiennych, które mogą być zmieniane (modyfikowane) w późniejszym czasie.
Ma blokowy zakres (block scope), co oznacza, że jest dostępny tylko w obrębie bloku kodu, w którym został zadeklarowany (np. wewnątrz pętli, funkcji, warunku).
Nie jest hoistowane jak var, czyli nie można odwołać się do zmiennej przed jej zadeklarowaniem.

const
Służy do deklarowania zmiennych, które nie mogą być modyfikowane po ich inicjalizacji (są stałymi).
Również ma blokowy zakres (block scope).
Musi być zainicjalizowana w momencie deklaracji

let jest używane do zmiennych, których wartość może się zmieniać.
const jest używane do zmiennych, których wartość nie powinna być zmieniana po przypisaniu.