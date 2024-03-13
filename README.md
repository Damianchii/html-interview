
# HTML Interview Questions 
<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=html" />
  </a>
</p>

## ➡️ What does a `doctype` do? | Co robi `doctype` ?
> Specifies the HTML standard, helping browsers interpret and render the content correctly
> Określa standard języka HTML. Polecenie jest wystawiane jeszcze przed definicja wlaciwego dokumentu 
## ➡️ How do you serve a page with content in multiple languages? | Jak udostępnić stronę z treścią w wielu językach?
> Use the `lang` attribute to specify the language in tag
> Użyj atrybutu `lang`, aby określić język w znaczniku
```bash
  <html lang="en">
```
```bash
  <span lang="en">Hello</span>
```
## ➡️ How do you serve a page with content in multiple languages? | Jak udostępnić stronę z treścią w wielu językach?
> Be wary of layout or overflow issues in the design
> Trzyba uważać na problemy z układem lub przepełnieniem projektu.
## ➡️ What are `data-` attributes good for? | Do czego `data-` są dobre ?
> `data-attributes` are used to store custom data for elements. They are helpful for JavaScript interaction
> `data-attributes` służą do przechowywania niestandardowych danych elementów. Są pomocne w interakcji JavaScript
## ➡️ Consider HTML5 as an open web platform. What are the building blocks of HTML5? | Rozważ HTML5 jako otwartą platformę internetową. Jakie są elementy składowe HTML5?
> <b>Semantics</b> HTML tags describe the content.
> <b>Styling - CSS</b> Customizing appearance of HTML tags
> <b>Connectivity</b> Communicate with the server in new and innovative ways.
> <b>Offline and storage</b> Allows webpages to store data on the client-side locally and operate offline more efficiently.
> <b>Multimedia</b> Makes video and audio first-class citizens in the Open Web.
> <b>2D/3D graphics and effects</b> Allows a much more diverse range of presentation options.
> <b>Performance and integration</b> Provides greater speed optimization and better usage of computer hardware.
> <b>Device access</b> Allows for the usage of various input and output devices.
<br/>

> <b>Semantyka</b> Tagi HTML opisują zawartość.
> <b>Stylizacja - CSS</b> Dostosowywanie wyglądu tagów HTML.
> <b>Łączność</b> Komunikacja z serwerem w nowych i innowacyjnych sposób.
> <b>Tryb offline i przechowywanie</b> Pozwala stronie internetowej przechowywać dane po stronie klienta lokalnie i efektywnie działać w trybie offline.
> <b>Multimedia</b> Wprowadza wideo i dźwięk na pierwszy plan w otwartym internecie.
> <b>Grafika 2D/3D i efekty</b> Oferuje znacznie bardziej zróżnicowane opcje prezentacji.
> <b>Wydajność i integracja</b> Zapewnia optymalizację szybkości i lepsze wykorzystanie sprzętu komputerowego.
> <b>Dostęp do urządzeń</b> Umożliwia korzystanie z różnych urządzeń wejściowych i wyjściowych.

## ➡️ Describe the difference between a `cookie`, `sessionStorage` and `localStorage` ? Jaka jest rożnica pomiędzy `cookie`, `sessionStorage` i `localStorage`
> All mechanisms serve to store data on the client side. `cookie` are primarily used for communication with the server, `sessionStorage` for short-term data storage during a page session, and `localStorage` for long-term data storage between different sessions.

> * `cookie` - Used to store small data, typically for tracking and authentication purposes.
> * `sessionStorage` - Used for storing data during the duration of a page session and gets cleared upon closing the tab (session).
> * `localStorage` - Used for persistent storage of data between browser sessions, and the data remains even after closing the page.
> Wszystkie mechanizmy służą do przechowywania danych po stronie klienta. `cookie` są głównie używane do komunikacji z serwerem, `sessionStorage` do krótkotrwałego przechowywania danych w trakcie sesji strony, a `localStorage` do długotrwałego przechowywania danych między różnymi sesjami.
> * `cookie` - Służą do przechowywania małych danych, zazwyczaj w celach śledzenia i uwierzytelniania niektóre sie usuwają po zamkneciu strony, trwale cookie zostaja na dłużej
> * `sessionStorage` - Służy do przechowywania danych na czas trwania sesji strony i usuwanją sie po zamknieciu karty (sesji)
> * `localStorage` -  Służy do trwałego przechowywania danych między sesjami przeglądarki i dane pozostają nawet po zamknięciu strony

## ➡️ Describe the difference between `<script>`, `<script async>` and `<script defer>` | Jaka jest różnica między`<script>`, `<script async>` i `<script defer>`.

> `<script>` tags are used to include JavaScript on a web page. The `<script async>` and `<script defer>` attributes are used to change how/when the loading and execution of the script happens.

> * The `async` attribute means that if the browser, while reading the page code, encounters a file with a script, it will start loading it in the background while reading the rest of the page code. If the entire script file is loaded, the code will be fired.

> * The `defer` attribute works somewhat similarly. The script file will also be loaded in the background. The difference is that if the browser has already loaded the entire script file, it will run it after loading the entire document (but just before firing the DOMContentLoaded event). This can be compared to a situation where a given script would be placed just before the end of the body.

> The difference between these attributes is that scripts with the defer attribute will be fired in the order in which they were inserted into the document. In the case of async, scripts will be fired in the "first come, first served" order, i.e. whichever script is loaded first will be fired first.

<br/>

> `<script>` służą do umieszczania kodu JavaScript na stronie internetowej. The `<script async>` and `<script defer>` służą do zmiany sposobu/czasu ładowania i wykonywania skryptu.

> * Atrybut `async` powoduje, że jeżeli przeglądarka czytając kod strony natrafi na plik ze skryptem zacznie go wczytywać w tle, równocześnie czytając dalszą część kodu strony. Jeżeli cały  plik ze skryptem się wczyta, wtedy kod zostanie odpalony.

> * Atrybut `defer` działa w miarę podobnie. Plik ze skryptem też będzie wczytywany w tle. Różnica jest taka, że jeżeli przeglądarka wczyta już cały plik ze skryptem, odpali go po załadowaniu całego dokumentu (ale tuż przed odpaleniem zdarzenia DOMContentLoaded). Można to przyrównać do sytuacji, gdy dany skrypt byłby umieszczony tuż przed końcem body. 

> Różnica między tymi atrybutami jest też taka, że skrypty z atrybutem defer będą odpalane w kolejności w jakiej zostały wstawione do dokumentu. W przypadku async skrypty będą odpalane w kolejności "kto pierwszy ten lepszy", czyli który skrypt wczyta się wcześniej, ten zostanie wcześniej odpalony.


## ➡️ Why is it generally a good idea to position CSS <link>s between <head></head> and JS <script>s just before </body>? Do you know any exceptions? | Dlaczego dobrym pomysłem jest zeby pozycjonować css `<link>` 

>  In a nutshell, such a placement of CSS `<link>` and JavaScript `<script>` allows for faster rendering of the page and better overall performance.
 Also, placing `<script>` at the bottom means that the browser cannot start downloading the scripts until the entire document is parsed. This ensures your code that needs to manipulate DOM elements will not throw an error and halt the entire script. If you need to put `<script>` in the `<head>`, use the `defer` attribute, which will achieve the same effect of running the script only after the HTML is parsed but the browser can kick off the network request earlier to download the script.

>  Krótko mówiąc, takie rozmieszczenie CSS `<link>` i JavaScript `<script>` pozwala na szybsze renderowanie strony i lepszą ogólną wydajność.

Umieszczenie `<script>` na dole oznacza, że przeglądarka nie może rozpocząć pobierania skryptów, dopóki cały dokument nie zostanie przeanalizowany. Dzięki temu Twój kod wymagający manipulacji elementami DOM nie wygeneruje błędu i nie zatrzyma całego skryptu. Jeśli chcesz umieścić `<script>` w `<head>`, użyj atrybutu `defer`, który osiągnie ten sam efekt, uruchamiając skrypt dopiero po przeanalizowaniu kodu HTML, ale przeglądarka może wcześniej wystartować z żądaniem sieciowym, aby pobrać skrypt .

## ➡️ What is progressive rendering? | Co to jest progresywne renderowanie ?

> In a nutshell, progressive rendering is a technique used in web development to improve website performance and user experience by displaying content as it becomes available, rather than waiting for the entire page to load. It prioritizes loading critical content first, such as text and basic layout elements, while asynchronously loading non-critical resources like images and scripts. This approach provides immediate feedback to users, reduces perceived load times, and creates a smoother browsing experience.

> W skrócie, progresywne renderowanie to technika stosowana w tworzeniu stron internetowych, która poprawia wydajność strony oraz doświadczenie użytkownika poprzez wyświetlanie zawartości w miarę jej dostępności, zamiast czekać na pełne załadowanie całej strony. Priorytetowo traktuje się ładowanie kluczowej zawartości, takiej jak tekst i podstawowe elementy układu, podczas gdy nieistotne zasoby, takie jak obrazy i skrypty, są ładowane asynchronicznie. Takie podejście zapewnia użytkownikom natychmiastową informację zwrotną, zmniejsza odczuwany czas ładowania oraz tworzy bardziej płynne doświadczenie przeglądania

## ➡️ Why you would use a `srcset` attribute in an image tag? Explain the process the browser uses when evaluating the content of this attribute. | Dlaczego miałbyś używać atrybutu `srcset` w tagu obrazu? Wyjaśnij proces stosowany przez przeglądarkę podczas oceny zawartości tego atrybutu.

> In a nutshell, the `srcset` attribute in an image tag allows the browser to receive a set of different images with various sizes or resolutions. The process of evaluating the content of this attribute involves selecting the best image based on the device's resolution, available space, and other factors. This helps optimize the display of images for different devices and network conditions, improving performance and user experience.

> W skrócie, atrybut `srcset` w znaczniku obrazu pozwala na dostarczenie przeglądarce zestawu różnych obrazów o różnych rozmiarach lub rozdzielczościach. Proces oceny zawartości tego atrybutu polega na wyborze najlepszego obrazu na podstawie rozdzielczości urządzenia, dostępnej przestrzeni i innych czynników. Dzięki temu można zoptymalizować wyświetlanie obrazów dla różnych urządzeń i warunków sieciowych, poprawiając wydajność i doświadczenie użytkownika.

## ➡️ Have you used different HTML templating languages before? | Czy korzystałeś już wcześniej z różnych języków szablonów HTML?

> Yes i have, I use React (JSX)

> Tak, korzystalem z React (JSX)
