# My_Notes
***Rest api and mixroservices

Roznica miedzy rest api to sposob na kommunikacje pomiedzy klientem a servezem przez http requests, a mickroservice to sposob na organizacje architektury na serverze, gdzie mikroservice nie powinny wymieniac sie przez rest api

***Target and current.target

***current target - to element ktory załączono procedurę obsługi zdarzeń

***target - gdzie wydazylo sie to zdarzenie

***Jak dziala przygladarka  ?

    1.Wpisujemy URL (Uniform Resource Locator) w szukiwarku przegladarki. URL wyswietla ns strone, ktora uzytkownik chce odzwiedziec.
    2.Przegladarka wysyla DNS(Domain Name System) na DNS-server, zeby otzymac IP-adress servera, na ktorym sie znajduje strona. DNS-server przetwarza nazwe domeny (naprzyklad, [www.example.com](http://www.example.com/)) na odpowiedni IP-adress
    3.Przegladarka nawiazuje polaczenie TCP z serverem, wykorzystując otrzymany adres IP. Dzięki temu przeglądarka może wysyłać i odbierać dane z serwera
    4.Przeglądarka wysyła do serwera żądanie HTTP (Hypertext Transfer Protocol) z żądaniem wyświetlenia strony internetowej. Żądanie może zawierać różne parametry, takie jak metoda żądania (GET, POST itp.), nagłówki i treść żądania
    5.Serwer przetwarza żądanie i odsyła odpowiedź HTTP zawierającą żądaną stronę internetową. Odpowiedź może również zawierać różne nagłówki, status odpowiedzi i treść odpowiedzi

    HTTP to protokół aplikacji służący do przesyłania dokumentów hipertekstowych, takich jak HTML. Przeznaczony jest do komunikacji pomiędzy przeglądarkami internetowymi i serwerami WWW
    Request Method(**GET HEAD POST PUT DELETE CONNECT OPTIONS TRACE**
 **PATCH)

 ***(Headers) – to metadane, które są przesyłane wraz z żądaniem i zawierają dodatkowe informacje o żądaniu, takie jak typ zawartości, uwierzytelnianie, buforowanie i inne parametry

 ***Body – jest używane tylko w niektórych metodach żądania, takich jak POST lub PUT. Zawiera dane, które klient wysyła do serwera, na przykład formularz do wysłania lub obiekt JSON

 ***CSSOM to zestaw API, które pozwalają na modyfikowanie CSS za pomocą JavaScriptu bez konieczności przeładowywania strony

 Critical Rendering Path (CRP) – to proces, który przeglądarka wykonuje, aby przekształcić HTML, CSS i JavaScript w wizualny interfejs na ekranie użytkownika
 1.Przeglądarka otrzymuje kod HTML dokumentu z serwera
 2.Przeglądarka analizuje kod HTML i tworzy strukturę drzewa dokumentu, zwaną DOM (Document Object Model)
 3.Przeglądarka ładuje zewnętrzne pliki CSS, a także osadzone i wbudowane style niezbędne do wyglądu strony. Po załadowaniu plików CSS przeglądarka tworzy CSSOM (CSS Object Model)
 4.Przeglądarka łączy DOM i CSSOM, aby utworzyć Render Tree, który zawiera tylko te węzły DOM, które zostaną wyświetlone na ekranie, oraz odpowiadające im style
 5.Przeglądarka określa rozmieszczenie każdego elementu w Render Tree, uwzględniając jego rozmiary i pozycję.
 6.Na podstawie Render Tree i układu (layout) przeglądarka rozpoczyna renderowanie zawartości na ekranie użytkownika. Proces ten obejmuje rysowanie pikseli dla każdego wyświetlanego elementu.
 7.Przeglądarka łączy wyrenderowane warstwy (layers) i tworzy ostateczny obraz, który użytkownik widzi na ekranie

 Optymalizacja CRP odgrywa ważną rolę w tworzeniu szybko ładujących się i responsywnych stron internetowych. Obejmuje to minimalizowanie użycia zasobów, optymalizację CSS i JavaScript, a także stosowanie metod, takich jak leniwe ładowanie zasobów i asynchroniczne ładowanie skryptów, aby przyspieszyć proces renderowania strony


***CORS (Cross-Origin Resource Sharing).
 Mekanizm, który wykorzystuje dodatkowe nagłówki HTTP, aby umożliwić agentowi użytkownika uzyskiwanie zezwoleń na dostęp do wybranych zasobów z serwera na źródle (domenie), innym niż ta, którą obecnie używa strona, nazywa się 



****MVC (Model-View-Controller)
Wzor projektowy, który umożliwia efektywne oddzielenie modelu danych (gdzie wszystko obsługuje serwer), wyświetlania i obsługi akcji (kontroler wykonuje odpowiednie operacje i przekazuje je do widoku)

***Wzorcami projektowymi (Design Patterns)
To gotowe do użycia rozwiązania często występujących problemów w programowaniu

***"use strict" to dyrektywa w JavaScript, która wprowadza tryb restrykcyjny, zmieniając sposób działania języka w celu uniknięcia pewnych powszechnych błędów i poprawy bezpieczeństwa
wprowadza szereg ograniczeń, takich jak:
Zakaz używania niezadeklarowanych zmiennych.
Uniemożliwienie przypisania wartości do tylko do odczytu (np. do stałych).
Zmiana sposobu działania funkcji, w tym rozróżnianie nazw argumentów w przypadku funkcji o tej samej nazwie.

***let
Służy do deklarowania zmiennych, które mogą być zmieniane (modyfikowane) w późniejszym czasie.
Ma blokowy zakres (block scope), co oznacza, że jest dostępny tylko w obrębie bloku kodu, w którym został zadeklarowany (np. wewnątrz pętli, funkcji, warunku).
Nie jest hoistowane jak var, czyli nie można odwołać się do zmiennej przed jej zadeklarowaniem.

***const
Służy do deklarowania zmiennych, które nie mogą być modyfikowane po ich inicjalizacji (są stałymi).
Również ma blokowy zakres (block scope).
Musi być zainicjalizowana w momencie deklaracji

let jest używane do zmiennych, których wartość może się zmieniać.
const jest używane do zmiennych, których wartość nie powinna być zmieniana po przypisaniu.

***Zmienne zadeklarowane za pomocą var mogą być aktualizowane i deklarowane ponownie

***Scope (zakres zmiennych)
Zakres zmiennych to część programu, w której możemy odwołać się do zmiennej, funkcji lub obiektu.
Zakresy pomagają ukrywać zmienne przed niepożądanym dostępem i dzielić kod na logiczne bloki

***Różnice między funkcją strzałkową a zwykłą funkcją
Nie można używać jako konstruktora
Lekkie deklarowanie
Składnia


***W czym jest roznica pomiedzy Сookie, Local Storage и Session Storage

Cookies:
Przechowują małe ilości danych (zwykle do 4 KB na domenę). Najczęściej używane do wymiany danych z serwerem

Local Storage:
Pozwala przechowywać większe ilości danych (zwykle od 5 do 10 MB na domenę). Nie znika po zamknięciu karty lub ponownym uruchomieniu przeglądarki.

Session Storage:
Również przeznaczony do przechowywania małych ilości danych, podobnie jak Cookies, ale dane sesji są usuwane po zamknięciu karty lub przeglądarki.


***KISS (Keep It Simple, Stupid) – „Rób to prosto, głupcze”
Zasada sugeruje, aby kod był jak najprostszy i łatwy do zrozumienia.

***DRY (Don't Repeat Yourself) – „Nie powtarzaj się”
Każdy fragment kodu powinien mieć jedno, unikalne miejsce.

***Promise & Async await
Promise Promise to obiekt w JavaScript, który reprezentuje wartość,
która będzie dostępna w przyszłości (np. po zakończeniu operacji asynchronicznej, takiej jak pobieranie danych z serwera).

***Async/Await
Async/Await to nowocześniejszy i czytelniejszy sposób obsługi Promisów, który pozwala pisać kod asynchroniczny w stylu synchronicznym.

***e.preventDefault() + e.stopPropagation()
Są używane do kontrolowania zachowania zdarzeń w przeglądarce.

e.preventDefault() – zatrzymuje domyślne działanie przeglądarki
Przykład: zapobiega przeładowaniu strony po wysłaniu formularza

e.stopPropagation() – zatrzymuje propagację zdarzenia w górę drzewa DOM
Przykład: kliknięcie w przycisk nie uruchomi zdarzenia w elemencie nadrzędnym

***Event Loop
Event Loop to mechanizm, który pozwala asynchronicznemu kodowi działać w JavaScript bez blokowania głównego wątku.
 Dzięki niemu JavaScript (który jest jednoprotokółowy) może wykonywać operacje asynchroniczne, nie zatrzymując głównego wątku aplikacji

Jednoprotokółowość - JavaScript wykonuje jeden kawałek kodu na raz (wątek główny).
Event Loop zarządza kolejką zadań, która zawiera makro i mikrotaski.

Mikrotaski (np. Promise) mają wyższy priorytet. Są wykonywane po każdym synchronizowanym zadaniu, ale przed makrotaskami.
Makrotaski to głównie zdarzenia, takie jak setTimeout(), setInterval() itp



```jsx
console.log('Start');

fetch('https://api.example.com/data')
  .then(response => response.json())  // callback #1
  .then(data => {
    console.log('Data processed inside callback:', data);
  })  // callback #2
  .catch(error => {
    console.error('Error:', error);
  });

console.log('End');


1.fetch inicjuje asynchroniczny żądanie do serwera.
2.Gdy żądanie jest zakończone, Callback #1 (funkcja przekazana do .then()) trafia do Callback Queue (kolejki zadań)
3.Event Loop obserwuje Call Stack. Kiedy stos wywołań (Call Stack) jest pusty (po wykonaniu np. console.log('End')),
 Event Loop pobiera Callback #1 z kolejki i umieszcza go w stosie wywołań do wykonania
4.Callback #1 jest wykonywany. Jeśli zwróci nowy Promise, to Callback #2 (funkcja w kolejnym .then()) trafi do Callback Queue
5.Gdy stos wywołań znowu jest pusty, Event Loop przenosi Callback #2 z Callback Queue do stosu wywołań, aby go wykonać
6.Wewnątrz Callback #2 dane z serwera są już dostępne (np. w zmiennej data) i mogą zostać przetworzone.

***Map & forEach
forEach to metoda tablicy w JavaScript, która wykonuje określoną funkcję dla każdego elementu w tablicy
forEach nie zwraca nowej tablicy, jesli chce utworzyc nowa tablica, w tedy lepej uzyc map

map to metoda tablicy w JavaScript, która wykonuje funkcję dla każdego elementu tablicy i zwraca nową tablicę z wynikami tych funkcji


***Script async defer
Atrybut async jest używany w tagu <script> w HTML, aby umożliwić asynchroniczne ładowanie skryptów JavaScript.
 Gdy skrypt jest załadowany z atrybutem async, przeglądarka nie czeka na jego załadowanie i wykonanie przed renderowaniem reszty strony
 defer zapewnia, że skrypty będą ładowane asynchronicznie, ale ich wykonywanie będzie opóźnione do momentu, aż cała strona zostanie w pełni załadowana

 ***Semantyczne tagi
  (Semantic Tags)to tagi, które mają logiczne znaczenie i pomagają w zrozumieniu struktury strony naprzyklad header, footer, ahead, nav

  ***Iterator
  to obiekt, który pozwala na iterowanie po tablice, obiekty, mapy, zbiory itd.
   Iterator jest odpowiedzialny za dostarczanie kolejnych elementów z kolekcji jeden po drugim, aż do momentu, gdy wszystkie elementy zostaną przeiterowane

   ***Generator
   Specjalny typ funkcji do wstrzymywania i wznawiania wykonania funkcji. Zwykle używany do sekwencyjnego generowania wartości

   ***new
   Kiedy tworzysz instancję obiektu za pomocą operatora new, właściwości i metody zdefiniowane w funkcji konstruktora są dodawane do protokołu (prototype) utworzonego obiektu.
   Oznacza to, że te właściwości i metody są dostępne dla wszystkich instancji,
   które zostały utworzone przy użyciu tego konstruktora, dzięki mechanizmowi dziedziczenia prototypów w JavaScript.

   1.Tworzenie nowego obiektu: Operator new tworzy nowy pusty obiekt.
    2.Przypisanie prototypu: Prototyp nowego obiektu zostaje ustawiony na prototype funkcji konstruktora.
    3.Wykonanie funkcji konstruktora: Funkcja konstruktora jest wywoływana z przypisaniem this do nowego obiektu.
    4.Zwracanie obiektu: Jeśli funkcja konstruktora nie zwróci jawnie obiektu, new zwróci nowo utworzony obiekt.

    function Person(name, age) {
  this.name = name;
  this.age = age;
}

const person1 = new Person('Alice', 25);
const person2 = new Person('Bob', 30);

console.log(person1.name);  // "Alice"
console.log(person2.age);   // 30

***this

this — to odniesienie do obiektu, w kontekście którego jest wywoływane. Wartość this zależy od miejsca, w którym funkcja jest wywoływana
Wartość this wewnątrz funkcji może się zmieniać w zależności od tego, jak funkcja została wywołana. this jest dynamiczne, a jego wartość zależy od kontekstu wywołania funkcji.

1.W metodzie obiektu: Jeśli funkcja jest wywoływana jako metoda obiektu, this odnosi się do tego obiektu.
const person = {
  name: 'Alice',
  greet: function() {
    console.log(this.name); // this odnosi się do obiektu person
  }
};

person.greet(); // "Alice"

2.W funkcji konstruktora: Kiedy funkcja jest używana jako konstruktor (z operatoriem new), this odnosi się do nowo utworzonego obiektu.
function Person(name) {
  this.name = name;
}

const person = new Person('Alice');
console.log(person.name); // "Alice", ponieważ this odnosi się do nowego obiektu

3.W funkcji strzałkowej: Funkcje strzałkowe nie mają własnego this. Zamiast tego this w funkcji strzałkowej jest dziedziczone z kontekstu, w którym została utworzona.
const person = {
  name: 'Alice',
  greet: function() {
    const arrowFunction = () => {
      console.log(this.name); // this odnosi się do obiektu person
    };
    arrowFunction();
  }
};

person.greet(); // "Alice"

Zmiana wartości this za pomocą call, apply i bind: Można jawnie ustawić wartość this za pomocą metod call, apply i bind.
function greet() {
  console.log(this.name);
}

const person = { name: 'Alice' };
greet.call(person); // "Alice", ponieważ `this` zostało ustawione na obiekt person

***map & set
Map to kolekcja par klucz/wartość, gdzie każdy klucz jest unikalny. Map zachowuje kolejność dodawania elementów, podczas gdy obiekt tego nie robi
Set to kolekcja, która przechowuje unikalne wartości, gwarantując, że w niej nie ma powtarzających się elementów


***Boxing & unboxing
Podczas wywoływania metod na wartościach prymitywnych, JavaScript automatycznie opakowuje wartość w obiekt i wywołuje metodę na tym obiekcie.
 Po wykonaniu metody, obiekt jest automatycznie "rozpakowywany" na wartość prymitywną.

 ***SPA & PWA
 SPA (Single Page Application) to aplikacja webowa, która dynamicznie aktualizuje HTML na stronie, bez konieczności przeładowywania całej strony
 Przykłady SPA: Gmail, Facebook, Twitter
 PWA (Progressive Web Application) to technologia, która umożliwia przekształcenie tradycyjnej strony internetowej w aplikację mobilną,
  którą można zainstalować na ekranie głównym urządzenia (smartfona, tabletu) i używać jej jak natywną aplikację
  Przyklady PWA: Pinterest, Spotify, AliExpress

***Null & undefined
  undefined to wartość, która oznacza, że zmienna została zadeklarowana, ale nie została jej przypisana żadna wartość.
null to specjalna wartość, którą przypisujemy zmiennej, aby wyraźnie wskazać, że nie ma ona żadnej wartości 


***Memoization(Memyzacja)
Memyzacja to przechowywanie poprzedniej wartości funkcji


***Private accessors(Prywatne akcesory)
Prywatne akcesory, definiowane za pomocą symbolu #, umożliwiają enkapsulację danych poprzez tworzenie prywatnych pól i metod w klasach,
 ograniczając zbędny dostęp z zewnątrz tej klasy


***Callback hell
Callback hell wiele wywołań zwrotnych (callbacków) zagnieżdżonych wewnątrz innych wywołań zwrotnych


***Hoisting
 to przenoszenie zadeklarowanej funkcji na górę jej zakresu widoczności. 
 Działa tylko dla function declaration, ale nie ma zastosowania do function expression, bez przeładowywania strony podczas interakcji z użytkownikiem.

 ***Closure(Zamknięcie)
 Zamknięcie to możliwość funkcji uzyskania dostępu do zmiennych z nadrzędnego zakresu.
  Jest to mechanizm realizowany poprzez istnienie ukrytej zmiennej, która zapewnia dostęp do leksykalnego środowiska.


***Lexical Environment (leksykalne środowisko)
  Leksykalne środowisko to ukryty obiekt zawierający listę zmiennych funkcji oraz odnośnik do nadrzędnego zakresu. Wszystkie funkcje w JavaScript są zamknięciami.

***Prototypy (dziedziczenie)
  Wszystko w JavaScript podlega dziedziczeniu. Na przykład, kiedy tworzymy obiekt, ma on metody obiektu, które są dziedziczone z Prototype Object.
  W starszych wersjach JavaScript do modyfikowania właściwości dziedziczenia używano proto, natomiast we współczesnym JavaScript lepiej jest stosować metodę [Object.getPrototypeOf(obj)]


***Niezmienne (Immutable) obiekty:
W JavaScript prymitywne typy danych (np. liczby, ciągi znaków, wartości logiczne) są niezmienne.
Podczas operacji na prymitywnych typach tworzone są nowe wartości, a stare pozostają bez zmian.

Przykład niezmiennego (immutable) obiektu w JavaScript:

jsx

let x = 5;
let y = x;  // Tworzona jest kopia wartości x
x = x + 1;  // Tworzony jest nowy obiekt, a nie zmieniany stary
console.log(x);  // Wyjście: 6
console.log(y);  // Wyjście: 5 (wartość y pozostaje niezmieniona)



***Zmienne (Mutable) obiekty:
Obiekty w JavaScript (w tym tablice i obiekty) są zmienne.
Zmiany w obiektach są bezpośrednio odzwierciedlane w samym obiekcie, bez tworzenia nowego obiektu.

Przykład zmiennego obiektu w JavaScript:

jsx

let arr = [1, 2, 3];
arr.push(4);  // Zmienia się sama tablica, a nie tworzy nowa
console.log(arr);  // Wyjście: [1, 2, 3, 4]


***Rekurencja
Rekurencja to kiedy funkcja wywołuje sama siebie


***Async code (asynchroniczny kod)
Async code (asynchroniczny kod) to sposób programowania, który pozwala wykonywać operacje nieblokujące głównego wątku programu.
 Dzięki temu aplikacja może kontynuować działanie, zamiast czekać na zakończenie czasochłonnych zadań takich jak:
pobieranie danych z API,
operacje na plikach,
interakcje z bazą danych,



***Callback function (funkcja zwrotna) 
Callback function (funkcja zwrotna) to funkcja przekazywana jako argument do innej funkcji, która zostanie wywołana później, zazwyczaj po zakończeniu jakiejś operacji.



***Cookies 
HTTP cookie (web cookie, cookie przeglądarki) – to mały fragment danych wysyłany przez serwer do przeglądarki użytkownika,
który przeglądarka może zapisać i odesłać z kolejnym żądaniem do tego samego serwera. Pozwala to między innymi sprawdzić,
czy oba żądania pochodzą z tej samej przeglądarki (na przykład w celu uwierzytelnienia użytkownika).
To sa danne ktore schowane na komputerze w pliku txt

Cookies są wykorzystywane głównie do:
Zarządzania sesją (logowanie, koszyki wirtualnych zakupów)
Personalizacji (preferencje użytkownika)
Monitorowania (śledzenia zachowania użytkownika)


***Shadow DOM 
Shadow DOM to technologia w przeglądarkach, która pozwala tworzyć enkapsulowane elementy DOM z własnymi stylami i logiką,
które nie wpływają na zewnętrzny dokument i są od niego niezależne.

***DOM 
To reprezentacja dokumentu HTML w postaci drzewa znaczników,
umożliwiająca interakcję za pomocą JavaScript (dodawanie/usuwanie elementów z drzewa, zmiana stylów elementów i wiele więcej).


***OPP 
OOP to sposób pisania kodu, który pozwala tworzyć obiekty na podstawie jednego obiektu.

Abstrakcja – tworzenie klasy bazowej z minimalnym zestawem wspólnych metod przeznaczonych do dziedziczenia.
Polimorfizm – zmiana funkcjonalności lub zachowania istniejącej metody lub właściwości.
Dziedziczenie – możliwość obiektu lub klasy do bazowania na innym obiekcie lub klasie. Jest to główny mechanizm ponownego użycia kodu.
Enkapsulacja – ukrywanie właściwości lub metod przed niepotrzebnym dostępem, np. za pomocą pól prywatnych.


***SOLID
S – Zasada pojedynczej odpowiedzialności (The Single Responsibility Principle) – każda klasa powinna wykonywać tylko jedno zadanie
O – Zasada otwartości/zamkniętości (The Open/Closed Principle) – nowa funkcjonalność powinna być dodawana poprzez rozszerzenie,
 a nie modyfikację istniejącego kodu (kod powinien być zamknięty na modyfikacje, ale otwarty na rozszerzenia).
L – Zasada podstawienia Liskov (The Liskov Substitution Principle) – klasa dziedzicząca powinna rozszerzać funkcjonalność klasy bazowej, a nie ją zmieniać.
I – Zasada segregacji interfejsów (The Interface Segregation Principle) – wiele dedykowanych interfejsów jest lepsze niż jeden ogólny interfejs.
D – Zasada odwrócenia zależności (The Dependency Inversion Principle) – moduły wyższego poziomu nie powinny zależeć od modułów niższego poziomu. Oba powinny zależeć od abstrakcji.

Poprawny kod 
// Klasa do wysyłania e-maili
class EmailService {
  sendEmail(to, subject, body) {
    // Wysyłanie e-maila
    console.log(`Send message ${to}: ${subject} - ${body}`);
  }
}
// Klasa do zarządzania użytkownikami
class UserService {
   // Konstruktor przyjmuje EmailService jako zależność
  constructor(emailService) {
    this.emailService = emailService;
  }
 // Rejestracja użytkownika i wysyłanie e-maila
  registerUser(username, email) {
    // Wysyłanie e-maila
    this.emailService.sendEmail(email, "Registration", `Welcome, ${username}!`);
  }
}
// Tworzymy instancję EmailService
const emailService = new EmailService();
// Przekazujemy ją do konstruktora UserService
const userService = new UserService(emailService);
userService.registerUser("John", "john@example.com");

Nie poprawny kod
// Klasa do wysyłania e-maili
class EmailService {
  sendEmail(to, subject, body) {
    // Wysyłanie e-maila
    console.log(`Send message ${to}: ${subject} - ${body}`);
  }
}
// Klasa do zarządzania użytkownikami
class UserService {
  // Konstruktor samodzielnie tworzy zależność od EmailService
  constructor() {
    this.emailService = new EmailService();  // ❌ Tworzenie zależności wewnątrz klasy
  }
// Rejestracja użytkownika i wysyłanie e-maila
  registerUser(username, email) {
     // Wysyłanie e-maila
    this.emailService.sendEmail(email, "Registration", `Welcome, ${username}!`);
  }
}
// Tworzymy instancję UserService
const userService = new UserService();
userService.registerUser("John", "john@example.com");




***WebSocket 
Zapewnia możliwość wymiany danych między przeglądarką a serwerem za pomocą stałego połączenia.
Dane są przesyłane w obu kierunkach w postaci "pakietów", bez przerywania połączenia i dodatkowych żądań HTTP.



*** Server Side Events (SSE)
Klient wysyła żądanie HTTP do serwera i pozostawia połączenie otwarte, dzięki czemu serwer może okresowo wysyłać aktualizacje do klienta przez to połączenie.
• SSE obsługuje komunikację jednokierunkową, co oznacza, że dane mogą być wysyłane tylko z serwera do klienta.
• Long Polling również wykorzystuje HTTP, ale w przeciwieństwie do SSE, klient wysyła żądanie do serwera, a serwer odpowiada dopiero wtedy,
 gdy ma dane do wysłania lub po upływie określonego czasu (timeout).


 ***Polling & Long Polling
 Polling – co pewien czas klient wysyła żądanie do serwera.
 Long polling – klient wysyła żądanie do serwera, które pozostaje otwarte i czeka na odpowiedź, aż zdarzy się jakieś wydarzenie lub zostanie otrzymana aktualizacja.



 ***Bing, Call, Apply
Wszystkie trzy służą do zmiany kontekstu this, jednak różnią się w sposobie użycia:
Call i Apply natychmiast wywołują funkcję i zwracają wynik jej wykonania.
Bind zwraca nową funkcję, którą można wywołać później.

Metoda bind() tworzy nową funkcję, która przy wywołaniu ustawia jako kontekst wykonania this na podaną wartość.

Metoda apply() wywołuje funkcję z określonym kontekstem this i parametrami przekazanymi w formie tablicy (lub obiektu przypominającego tablicę).


Przyklady 

apply()
func.apply(thisArg, [argsArray])
Metoda apply() wywołuje funkcję z określonym kontekstem this i argumentami przekazanymi w postaci tablicy (lub obiektu przypominającego tablicę).

call()
fun.call(thisArg, arg1, arg2, ...)
Metoda call() wywołuje funkcję z określonym kontekstem this i argumentami przekazanymi jako lista (oddzielne parametry).
