
# Independent teams  
## (Promise #3)

<!--
<details open>
  <summary>🇵🇱</summary>
  Niezależność zespołów
</details>
<details>
  <summary>🇷🇺</summary>
  Независимость команд
</details>
-->

---

# The Promise

- Every team owns its microservice  
- Teams deploy independently  
- No cross‑team coordination  
- No shared release cycles  
- No bottlenecks  
- Full autonomy → full speed

Sounds perfect on paper.
<!--
<details open>
  <summary>🇵🇱</summary>

  Co nam obiecywano?  
  - każdy zespół będzie odpowiadał wyłącznie za swoje mikroserwisy  
  - zespoły będą wdrażać niezależnie od siebie  
  - żadnej koordynacji między zespołami  
  - żadnych wspólnych cykli wydawniczych  
  - żadnych wąskich gardeł  
  - pełna autonomia pozwoli osiągnąć maksymalną prędkość dewelopmentu  

  Brzmi świetnie… na papierze.
</details>

<details>
  <summary>🇷🇺</summary>

  Что нам обещали?  
  - каждая команда будет отвечать только за свои микросервисы  
  - команды будут деплоить независимо друг от друга  
  - никакой координации между командами  
  - никаких общих релизных циклов  
  - никаких узких мест  
  - полная автономия позволит развить максимальную скорость разработки  

  Звучит всё отлично…
</details>
-->

---

# The Reality

- Services depend on each other  
- APIs change → everyone breaks  
- Shared libraries create hidden coupling  
- Shared databases create hard coupling  
- Cross‑team contracts require negotiation  
- "Independent" deployments still require coordination  
- Autonomy turns into meetings, syncs, and versioning hell
<!--
<details open>
  <summary>🇵🇱</summary>

  A jak wygląda rzeczywistość?  

  - serwisy zależą od siebie  
  - każda zmiana w API potrafi zepsuć wszystkie usługi, które z niego korzystają —  
    i tak dalej w łańcuchu  
  - wspólne biblioteki tworzą ukryte zależności  
  - współdzielone bazy danych uniemożliwiają swobodne zmiany w strukturze danych  
  - kontrakty API i komunikatów trzeba uzgadniać między zespołami  
  - „niezależne” wdrożenia i tak wymagają koordynacji  
  - autonomia prowadzi do nadmiaru spotkań, synchronizacji danych i wersjonowania,  
    które zamienia się w koszmar
</details>

<details>
  <summary>🇷🇺</summary>

  Но как обстоят дела на самом деле?  

  - сервисы зависят друг от друга  
  - любое изменение API выводит из строя всех, кто его использует, и далее по цепочке  
  - общие либы создают скрытые зависимости  
  - общие базы данных не позволяют свободно менять структуру данных  
  - контракты API и сообщений приходится согласовывать между командами  
  - «независимые» деплои всё равно приходится координировать  
  - автономность приводит к избыточным митингам, синкам данных и версионному аду
</details>
-->

---

# Why it happens

- Business domains rarely split cleanly  
- Teams need shared data  
- Cross‑cutting concerns bind teams together  
  - auth  
  - logging  
  - tracing  
  - shared libraries  
  - shared infrastructure  
- Organizational structure doesn’t magically become modular  
- Conway’s Law always wins
<!--
<details open>
  <summary>🇵🇱</summary>

  Dlaczego tak się dzieje?  

  - domeny biznesowe rzadko da się wyraźnie wydzielić,  
    ich granice i zakresy odpowiedzialności są rozmyte  

  - różne zespoły mogą potrzebować różnych reprezentacji  
    tych samych danych,  
    a uwaga często skupia się na danych, a nie na procesach  

  - istnieje wiele domen, które nie są częścią kluczowego biznesu,  
    ale są potrzebne niemal w każdym serwisie każdej ekipy  
    zwykle realizuje je zespół platformowy  
    jeszcze gorzej, gdy robią to różne zespoły  
    wtedy nikt nie odpowiada za nie w pełni,  
    a zależy od nich cała architektura  

  - struktura firmy nie staje się modularna od machnięcia różdżką  

  - prawo Conwaya jest silniejsze niż decyzje techniczne
</details>

<details>
  <summary>🇷🇺</summary>

  Почему же так получается?

  - бизнес‑домены на самом деле редко чётко выделимы,  
    их границы и зоны ответственности размыты  

  - разным командам могут быть нужны разные представления  
    всё тех же данных,  
    и фокус зачастую делается не на процессах, а на данных  

  - множество доменов не относится к основному бизнесу,  
    но нужно почти в каждом сервисе каждой команды  
    обычно их реализует платформенная команда  
    ещё хуже, когда их реализуют разные команды  
    тогда за них никто не отвечает полностью,  
    но при этом от них зависит вся система  

  - структура компании не становится модульной по мановению волшебной палочки  

  - закон Конвея сильнее технических решений
</details>
-->

---
# layout: center
class: text-center
---

# Bottom line

### Microservices don’t create independent teams.  
### Independent teams create microservices.

Without organizational autonomy,  
the architecture becomes just another layer of complexity.

<!--
<details open>
  <summary>🇵🇱</summary>

  Wnioski  

  Mikroserwisy same w sobie nie czynią zespołów niezależnymi.  
  To raczej niezależne zespoły są w stanie tworzyć dobre mikroserwisy.  

  Bez autonomii na poziomie struktury organizacji  
  architektura staje się jedynie kolejną warstwą,  
  która zwiększa złożoność systemu,  
  spowalnia wprowadzanie zmian  
  i podnosi liczbę błędów.
</details>

<details>
  <summary>🇷🇺</summary>

  Вывод  

  Микросервисы не делают команды независимыми.  
  У независимых команд иногда могут получаться хорошие микросервисы.  

  Без автономии на уровне структуры компании  
  архитектура становится ещё одним слоем,  
  лишь увеличивающим сложность системы,  
  замедляющим внесение изменений  
  и увеличивающим количество дефектов.
</details>
-->