# My_Notes

\*\*\*Rest api and mixroservices

Roznica miedzy rest api to sposob na kommunikacje pomiedzy klientem a servezem przez http requests, a mickroservice to sposob na organizacje architektury na serverze, gdzie mikroservice nie powinny wymieniac sie przez rest api

\*\*\*Target and current.target

\*\*\*current target - to element ktory załączono procedurę obsługi zdarzeń

\*\*\*target - gdzie wydazylo sie to zdarzenie

\*\*\*Jak dziala przygladarka ?

    1.Wpisujemy URL (Uniform Resource Locator) w szukiwarku przegladarki. URL wyswietla ns strone, ktora uzytkownik chce odzwiedziec.
    2.Przegladarka wysyla DNS(Domain Name System) na DNS-server, zeby otzymac IP-adress servera, na ktorym sie znajduje strona. DNS-server przetwarza nazwe domeny (naprzyklad, [www.example.com](http://www.example.com/)) na odpowiedni IP-adress
    3.Przegladarka nawiazuje polaczenie TCP z serverem, wykorzystując otrzymany adres IP. Dzięki temu przeglądarka może wysyłać i odbierać dane z serwera
    4.Przeglądarka wysyła do serwera żądanie HTTP (Hypertext Transfer Protocol) z żądaniem wyświetlenia strony internetowej. Żądanie może zawierać różne parametry, takie jak metoda żądania (GET, POST itp.), nagłówki i treść żądania
    5.Serwer przetwarza żądanie i odsyła odpowiedź HTTP zawierającą żądaną stronę internetową. Odpowiedź może również zawierać różne nagłówki, status odpowiedzi i treść odpowiedzi

    HTTP to protokół aplikacji służący do przesyłania dokumentów hipertekstowych, takich jak HTML. Przeznaczony jest do komunikacji pomiędzy przeglądarkami internetowymi i serwerami WWW
    Request Method(**GET HEAD POST PUT DELETE CONNECT OPTIONS TRACE**

\*\*PATCH)

\*\*\*(Headers) – to metadane, które są przesyłane wraz z żądaniem i zawierają dodatkowe informacje o żądaniu, takie jak typ zawartości, uwierzytelnianie, buforowanie i inne parametry

\*\*\*Body – jest używane tylko w niektórych metodach żądania, takich jak POST lub PUT. Zawiera dane, które klient wysyła do serwera, na przykład formularz do wysłania lub obiekt JSON

\*\*\*CSSOM to zestaw API, które pozwalają na modyfikowanie CSS za pomocą JavaScriptu bez konieczności przeładowywania strony

Critical Rendering Path (CRP) – to proces, który przeglądarka wykonuje, aby przekształcić HTML, CSS i JavaScript w wizualny interfejs na ekranie użytkownika
1.Przeglądarka otrzymuje kod HTML dokumentu z serwera
2.Przeglądarka analizuje kod HTML i tworzy strukturę drzewa dokumentu, zwaną DOM (Document Object Model)
3.Przeglądarka ładuje zewnętrzne pliki CSS, a także osadzone i wbudowane style niezbędne do wyglądu strony. Po załadowaniu plików CSS przeglądarka tworzy CSSOM (CSS Object Model)
4.Przeglądarka łączy DOM i CSSOM, aby utworzyć Render Tree, który zawiera tylko te węzły DOM, które zostaną wyświetlone na ekranie, oraz odpowiadające im style
5.Przeglądarka określa rozmieszczenie każdego elementu w Render Tree, uwzględniając jego rozmiary i pozycję.
6.Na podstawie Render Tree i układu (layout) przeglądarka rozpoczyna renderowanie zawartości na ekranie użytkownika. Proces ten obejmuje rysowanie pikseli dla każdego wyświetlanego elementu.
7.Przeglądarka łączy wyrenderowane warstwy (layers) i tworzy ostateczny obraz, który użytkownik widzi na ekranie

Optymalizacja CRP odgrywa ważną rolę w tworzeniu szybko ładujących się i responsywnych stron internetowych. Obejmuje to minimalizowanie użycia zasobów, optymalizację CSS i JavaScript, a także stosowanie metod, takich jak leniwe ładowanie zasobów i asynchroniczne ładowanie skryptów, aby przyspieszyć proces renderowania strony

\*\*\*CORS (Cross-Origin Resource Sharing).
Mekanizm, który wykorzystuje dodatkowe nagłówki HTTP, aby umożliwić agentowi użytkownika uzyskiwanie zezwoleń na dostęp do wybranych zasobów z serwera na źródle (domenie), innym niż ta, którą obecnie używa strona, nazywa się

\*\*\*\*MVC (Model-View-Controller)
Wzor projektowy, który umożliwia efektywne oddzielenie modelu danych (gdzie wszystko obsługuje serwer), wyświetlania i obsługi akcji (kontroler wykonuje odpowiednie operacje i przekazuje je do widoku)

\*\*\*Wzorcami projektowymi (Design Patterns)
To gotowe do użycia rozwiązania często występujących problemów w programowaniu

\*\*\*"use strict" to dyrektywa w JavaScript, która wprowadza tryb restrykcyjny, zmieniając sposób działania języka w celu uniknięcia pewnych powszechnych błędów i poprawy bezpieczeństwa
wprowadza szereg ograniczeń, takich jak:
Zakaz używania niezadeklarowanych zmiennych.
Uniemożliwienie przypisania wartości do tylko do odczytu (np. do stałych).
Zmiana sposobu działania funkcji, w tym rozróżnianie nazw argumentów w przypadku funkcji o tej samej nazwie.

\*\*\*let
Służy do deklarowania zmiennych, które mogą być zmieniane (modyfikowane) w późniejszym czasie.
Ma blokowy zakres (block scope), co oznacza, że jest dostępny tylko w obrębie bloku kodu, w którym został zadeklarowany (np. wewnątrz pętli, funkcji, warunku).
Nie jest hoistowane jak var, czyli nie można odwołać się do zmiennej przed jej zadeklarowaniem.

\*\*\*const
Służy do deklarowania zmiennych, które nie mogą być modyfikowane po ich inicjalizacji (są stałymi).
Również ma blokowy zakres (block scope).
Musi być zainicjalizowana w momencie deklaracji

let jest używane do zmiennych, których wartość może się zmieniać.
const jest używane do zmiennych, których wartość nie powinna być zmieniana po przypisaniu.

\*\*\*Zmienne zadeklarowane za pomocą var mogą być aktualizowane i deklarowane ponownie

\*\*\*Scope (zakres zmiennych)
Zakres zmiennych to część programu, w której możemy odwołać się do zmiennej, funkcji lub obiektu.
Zakresy pomagają ukrywać zmienne przed niepożądanym dostępem i dzielić kod na logiczne bloki

\*\*\*Różnice między funkcją strzałkową a zwykłą funkcją
Nie można używać jako konstruktora
Lekkie deklarowanie
Składnia

\*\*\*W czym jest roznica pomiedzy Сookie, Local Storage и Session Storage

Cookies:
Przechowują małe ilości danych (zwykle do 4 KB na domenę). Najczęściej używane do wymiany danych z serwerem

Local Storage:
Pozwala przechowywać większe ilości danych (zwykle od 5 do 10 MB na domenę). Nie znika po zamknięciu karty lub ponownym uruchomieniu przeglądarki.

Session Storage:
Również przeznaczony do przechowywania małych ilości danych, podobnie jak Cookies, ale dane sesji są usuwane po zamknięciu karty lub przeglądarki.

\*\*\*KISS (Keep It Simple, Stupid) – „Rób to prosto, głupcze”
Zasada sugeruje, aby kod był jak najprostszy i łatwy do zrozumienia.

\*\*\*DRY (Don't Repeat Yourself) – „Nie powtarzaj się”
Każdy fragment kodu powinien mieć jedno, unikalne miejsce.

\*\*\*Promise & Async await
Promise Promise to obiekt w JavaScript, który reprezentuje wartość,
która będzie dostępna w przyszłości (np. po zakończeniu operacji asynchronicznej, takiej jak pobieranie danych z serwera).

\*\*\*Async/Await
Async/Await to nowocześniejszy i czytelniejszy sposób obsługi Promisów, który pozwala pisać kod asynchroniczny w stylu synchronicznym.

\*\*\*e.preventDefault() + e.stopPropagation()
Są używane do kontrolowania zachowania zdarzeń w przeglądarce.

e.preventDefault() – zatrzymuje domyślne działanie przeglądarki
Przykład: zapobiega przeładowaniu strony po wysłaniu formularza

e.stopPropagation() – zatrzymuje propagację zdarzenia w górę drzewa DOM
Przykład: kliknięcie w przycisk nie uruchomi zdarzenia w elemencie nadrzędnym

\*\*\*Event Loop
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



React Install
1. Jeseli jest stara wersja npm install react-scripts@latest
2.Wybieramy framework
3. Wybrac variant 
4. npm create vite@latest countries-task
5. Wchodzimy do pliku cd nazwa-repo
6.npm install
7. Zeby uruchomic aplikacje npm run dev

o taki sposob mozna dolaczyc jakoms wartosc za pomoca `join` {topCurrencies.join(", ")}

 table-layout: fixed; - każda kolumna dostaje równą szerokość */

 word-break: break-word jest przydatna np. "West African CFA franc" zawinie się w dwóch linijkach, a nie wyjdzie poza ekran. (pozwala zawiac dlugie teksty)


Context

1. Tworzy sie typ w kompononecie "Global.tsx" (zawsze powinnie byc "export const") np export const GlobalTypes
2. I tworzymy nasz plik hook nazwa powinna zawierac "use" np. "useGlobalContext.tsx"
2. Robimy typ podobny na nasz "GlobalTypes" w tym przypadku bedzie to "GlobalContextType" i przypisujemy nazwy typuw z naszego "GlobalType" oraz jakiego typu oni sa np. "string", "number", i td.
3. Teraz robimy sam nasz komponent gdxie bedziemy przekazywac typy oraz stworzymy nasz provider -
export const GlobalContext = createContext<GlobalContextType>({}as GlobalContextType);
4.Tworzymy nasz typ provider czyli - GlobalProviderProps
type GlobalProviderProps = {
  children: ReactNode[] | ReactNode;
};
5. Tutaj tworzymy juz sam komponent providera
export const GlobalProvider = ({ children} : GlobalProviderProps) => {
  tutaj wpisuje swoje typy ktore chce przekazac w inne komponenty np. const [second, setSecond] = useState("");
return (
  <GlobalContext.Provider value={{ second, setSecond}}>
  {children}
  </GlobalContext.Provider>
)
}
5. Owijamy cala nasza aplikacje w provider zeby my moglismy przekazywac danne we wszystkie komponenty
<GlobalProvider>
<App />
</GlobalProvider>




##Proxy

To wbudowany obiekt w JavaScript, który pozwala stworzyć "otoczkę" (obiekt pośredniczący) wokół innego obiektu lub tablicy, aby przechwytywać i modyfikować jego zachowanie. Posiada tzw. przechwytywacze (ang. handlers) takie jak get i set, które można skonfigurować do przechwytywania operacji takich jak odczyt lub zapis właściwości, wywołanie funkcji, iteracja

Przyklad proxy:
const osoba = {
  imie: "Ala",
  wiek: 25
};

// Tworzymy obiekt Proxy
const proxyOsoba = new Proxy(osoba, {
  get(target, prop) {
    console.log(`Odczytywanie właściwości: ${prop}`);
    return target[prop]; // zwracamy oryginalną wartość
  },
  set(target, prop, value) {
    console.log(`Ustawianie właściwości: ${prop} = ${value}`);
    target[prop] = value; // ustawiamy nową wartość
    return true; // musimy zwrócić true, aby operacja się powiodła
  }
});

// Test działania:
console.log(proxyOsoba.imie);      // -> log: Odczytywanie właściwości: imie
proxyOsoba.wiek = 30;              // -> log: Ustawianie właściwości: wiek = 30
console.log(proxyOsoba.wiek);      // -> log: Odczytywanie właściwości: wiek





#HOF (funkcje wyższego rzędu)

Funkcje wyższego rzędu to takie funkcje, które operują na innych funkcjach — albo przyjmują je jako argumenty, albo zwracają jako wynik.




##HOC (Higher-Order Component / Komponent wyższego rzędu)

To funkcja, która przyjmuje komponent jako argument i zwraca nowy, ulepszony komponent. HOC-y są często spotykane w zewnętrznych bibliotekach, takich jak connect w Redux czy createFragmentContainer w Relay.


HOC:

const withUser = (Component) => (props) => {
  const user = { name: "Jan" };
  return <Component {...props} user={user} />;
};


Hook:

function MyComponent() {
  const user = useUser(); // np. customowy hook
  return <div>Witaj, {user.name}</div>;
}




##Typy danych (Data Types)

Dzielą się na prymitywne i obiektowe number, string, boolean, bigInt, null, object, undefiend, symbol - 8;




##Czysta funkcja

To taka funkcja, która zwraca wynik tylko na podstawie przekazanych argumentów i nie powoduje efektów ubocznych





##CI/CD
CI – Continuous Integration (ciągła integracja)

CD – Continuous Delivery (ciągłe dostarczanie) lub Continuous Deployment (ciągłe wdrażanie)

To sposób automatyzacji rutynowych procesów takich jak budowanie projektu, testowanie, wydawanie wersji i wdrażanie (deploy).

Często wiąże się to z tworzeniem pipeline (ciągu zautomatyzowanych kroków), który uruchamia się np. przed wypchnięciem zmian do głównej gałęzi (master/main)





##Git Merge vs Rebase

To dwa sposoby łączenia gałęzi w jedną.

`git merge` łączy zmiany, tworząc nowy commit scalający (merge commit), zachowując przy tym pełną historię obu gałęzi.
Historia zostaje rozgałęziona, ale nic nie jest tracone. Zachowuje strukturę drzewa commitów (historię rozwidleń)

`git rebase` przepisuje historię commitów – przenosi lokalne commity na szczyt zaktualizowanej głównej gałęzi.
Tworzy prostą linię historii, jakby gałąź była tworzona na świeżo od głównej




##Husky

To narzędzie do zarządzania Git hookami oraz automatyzacji działań wykonywanych przed commitami lub przed pushami do repozytorium.





##Cypress

To narzędzie, które pozwala programistom tworzyć testy symulujące zachowanie użytkownika w przeglądarce
 oraz sprawdzać działanie i poprawność funkcjonalności aplikacji.




 ##Przechowywanie przez wartość i przez referencję

Typy prymitywne (liczby, boolean, stringi) są przechowywane i porównywane przez wartość. Można bezpiecznie zmieniać wartość zmiennej, nie martwiąc się, że wpłynie to na coś innego.

Typy referencyjne (obiekty, tablice) są przechowywane i porównywane przez referencję (adres w pamięci). Przy porównywaniu uwzględniany jest fakt, czy dwie zmienne wskazują na ten sam obiekt. Nawet jeśli dwa obiekty mają identyczne dane, ale są różnymi instancjami, to są różne.

Zmiany wewnątrz obiektu będą widoczne wszędzie tam, gdzie istnieje referencja do tego obiektu. Bezpośrednia modyfikacja danych obiektu nazywa się mutacją. Lepiej unikać mutacji, ponieważ może prowadzić do trudnych do wykrycia błędów.

Aby bezpiecznie zmieniać typ referencyjny, należy najpierw wykonać jego kopię. W ten sposób powstaje nowa referencja i zmiany nie wpływają na oryginalny obiekt.





##Tworzenie obiektu bez prototypu lub bez referencji

Obiekt bez prototypu można utworzyć za pomocą Object.create(null).
Taki obiekt nie dziedziczy żadnych właściwości ani metod z Object.prototype.

Obiekt bez referencji (kopię głęboką) można zrobić przy pomocy structuredClone() lub JSON.parse(JSON.stringify(obj)).
Jednak przy takim podejściu utracimy wszystkie typy danych, które nie podlegają konwersji, np.:

metody obiektu (funkcje) zostaną usunięte,

obiekty Date zostaną zamienione na stringi,

undefined zostanie zignorowane i nie pojawi się w nowym obiekcie.



##Bazy danych SQL i NoSQL

Główne różnice to:

Skalowalność – NoSQL lepiej skalują się dzięki rozdzieleniu danych między wiele serwerów.

Elastyczność danych – NoSQL często używa elastycznych schematów, które pozwalają na dodawanie i zmienianie pól w dokumentach bez konieczności modyfikowania całej struktury.

NoSQL posiada własne API do pracy z bazą danych.

Natomiast bazy SQL mają:

Ścisłą, schematyczną strukturę danych.

Używają języka SQL do wykonywania zapytań.



##GraphQL

Główną zaletą GraphQL jest to, że pozwala na żądanie tylko tych danych, które są potrzebne. Dzięki GraphQL można zmniejszyć ilość kodu zarówno po stronie serwera,
jak i klienta, dzięki precyzyjnemu zapytaniu o dane oraz typowaniu informacji.

Typ Query służy do odczytu danych z API.

Typ Mutation służy do zapisu lub zmiany danych.

Błędy w GraphQL są obsługiwane za pomocą specjalnego typu danych Error i zwracane w polu errors w odpowiedzi.



##Design patterns

1. Wzorce kreacyjne (Pochodzące od "tworzyć"):

  Metoda wytwórcza (Factory Method): umożliwia tworzenie obiektów bez konieczności określania ich konkretnych klas.

  Abstrakcyjna fabryka (Abstract Factory): zapewnia interfejs do tworzenia rodzin powiązanych lub współzależnych obiektów bez wskazywania ich konkretnych klas.

  Budowniczy (Builder): służy do konstruowania złożonych obiektów poprzez wykonywanie prostych kroków konstrukcyjnych.

2. Wzorce strukturalne:

  Adapter (Adapter): pozwala, aby interfejs jednej klasy był kompatybilny z interfejsem innej klasy.

  Dekorator (Decorator): umożliwia dodawanie nowych funkcji do obiektów bez zmieniania ich struktury.

  Pełnomocnik (Proxy): zapewnia zastępstwo lub reprezentanta innego obiektu w celu kontrolowania dostępu do niego.

3. Wzorce behawioralne (Zachowań):

  Obserwator (Observer): definiuje zależność typu „jeden do wielu” pomiędzy obiektami w taki sposób, że zmiana stanu jednego obiektu powoduje automatyczne powiadomienie i aktualizację wszystkich zależnych od niego obiektów.

  Strategia (Strategy): definiuje rodzinę algorytmów, enkapsuluje każdy z nich i umożliwia ich wzajemną wymienność.

  Polecenie (Command): enkapsuluje żądanie jako obiekt, umożliwiając konfigurowanie klientów do przetwarzania żądań, kolejkowanie żądań lub prowadzenie dziennika zmian.



##Sass

Główne funkcje: zmienne, zagnieżdżone style, zagnieżdżone selektory, import plików, funkcje i pętle.

Miksiny – to fragment kodu, który można wielokrotnie wykorzystywać w różnych miejscach za pomocą @include.


Na przyklad:
sass
    @mixin border-radius($radius) {
      -webkit-border-radius: $radius;
      -moz-border-radius: $radius;
      border-radius: $radius;
    }

    .button {
      @include border-radius(5px);
    }

##Mikroserwisy

Mikroserwisy to podejście do tworzenia aplikacji jako zestawu niezależnie wdrażanych usług, które nie są od siebie zależne. Aplikacja jest budowana jako kombinacja mikroserwisów, z których każdy odpowiada za określoną funkcjonalność w swojej domenie (obszarze tematycznym). Mikroserwisy komunikują się ze sobą za pomocą interfejsów API, takich jak REST.


 ## 1.Kiedy API z danymi można nazwać mikroserwisem:
Jeśli to API:

jest niezależne od reszty systemu (może działać osobno),

odpowiada za jedną konkretną funkcjonalność lub domenę (np. „zarządzanie użytkownikami”, „produkty”, „płatności”),

można je wdrożyć i rozwijać niezależnie (np. osobny zespół, osobna baza danych, niezależny deployment),


 ## 2.Kiedy API z danymi nie jest mikroserwisem:
Jeśli to tylko część monolitycznej aplikacji (np. endpointy /users, /orders, ale wszystko działa na jednym serwerze i jednej bazie danych),

Jeśli nie można go uruchomić i rozwijać niezależnie,

Jeśli nie ma jasnego podziału domenowego (np. jeden ogromny kontroler robi „wszystko”),

to wtedy to zwykłe API, a nie mikroserwis.



##Przyklady mikroserwisów:

1. User Service (Serwis użytkowników)
Rejestracja, logowanie, profil użytkownika, zmiana hasła

2. Product Service (Serwis produktów)
Lista produktów, szczegóły, kategorie, dostępność

3. Order Service (Serwis zamówień)
Tworzenie zamówień, statusy, historia zakupów

4. Payment Service (Serwis płatności)
Integracja z PayPal/Stripe, weryfikacja płatności

5. Shipping Service (Serwis dostawy)
Informacje o przesyłce, generowanie etykiet, śledzenie



##Webpack
Module Federation — to wtyczka do Webpacka, która umożliwia dzielenie kodu między niezależnymi aplikacjami
 i dynamiczne ładowanie tego kodu w przeglądarce użytkownika.

Dynamiczne ładowanie modułów – kod jest pobierany tylko wtedy, gdy jest potrzebny.
Rozwój aplikacji webowej w architekturze mikrofrontendów (mikroserwisowej) – każdy moduł może być tworzony i wdrażany niezależnie.


Podział aplikacji na oddzielne moduły:

Można podzielić aplikację na mniejsze, niezależne części – na przykład:
  # moduł główny (np. layout, routing),

  # moduł uwierzytelniania (logowanie, rejestracja),

  # moduł danych (np. dashboard, API).

Każdy z tych modułów:
  # może być rozwijany przez osobny zespół,

  # ma własny cykl życia i wdrożenie,

  # może być ładowany tylko wtedy, gdy użytkownik go potrzebuje.

```
