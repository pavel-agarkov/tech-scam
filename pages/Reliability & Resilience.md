

# Reliability & Resilience  
## (Promise #4)

<!--
<details open>
  <summary>🇵🇱</summary>
  Wysoka niezawodność i odporność na awarie  
</details>
<details>
  <summary>🇷🇺</summary>
  Надежность и отказоустойчивость
</details>
-->

---

# The Promise

- Each service fails independently  
- One failure doesn’t bring down the whole system  
- Circuit breakers, retries, timeouts → built‑in resilience  
- Horizontal scaling improves availability  
- Distributed architecture = fault tolerance by design  

In theory, microservices should make outages smaller and rarer.

<!--
<details open>
  <summary>🇵🇱</summary>

  Obietnica  
  - każdy serwis psuje się niezależnie od pozostałych  
  - circuit breakers, retries, timeouts → wbudowane „z pudełka”  
  - możliwość skalowania horyzontalnego poprawia dostępność  
  - architektura rozproszona jest z definicji odporna na awarie  

  W teorii mikroserwisy powinny więc sprawiać,  
  że awarie będą rzadsze i mniej dotkliwe.
</details>

<details>
  <summary>🇷🇺</summary>

  Обещание  
  - каждый сервис выходит из строя независимо от других  
  - circuit breakers, retries, timeouts → встроенные из коробки  
  - возможность горизонтального масштабирования улучшает доступность  
  - распределённая архитектура устойчива к сбоям по определению  

  Так что, в теории, микросервисы должны сделать сбои менее значимыми и редкими.
</details>
-->

---

# The Reality

- More services → more network calls → more points of failure  
- Cascading failures become the norm  
- Timeouts, retries, backpressure need constant tuning  
- Partial outages are harder to detect and diagnose  
- Distributed tracing becomes mandatory just to understand what broke  
- "Self‑healing" often means "restart everything and hope for the best"  

Reliability doesn’t appear automatically - it must be engineered.

<!--
<details open>
  <summary>🇵🇱</summary>

  Co zwykle wychodzi w praktyce?  

  - więcej serwisów → więcej zapytań sieciowych → więcej punktów awarii  
  - awarie kaskadowe stają się codziennością  
  - timeouty, liczba retry i limity obciążenia  
    wymagają ciągłego dostrajania  
  - niedostępność tylko części funkcji jest trudniejsza do zdiagnozowania  
  - rozproszone śledzenie staje się koniecznością,  
    żeby w ogóle zrozumieć, co się zepsuło  
  - „self‑healing” często oznacza „zrestartować i liczyć na cud”  

  Niezawodność nie pojawia się automatycznie — trzeba ją zaprojektować i wdrożyć samemu.
</details>

<details>
  <summary>🇷🇺</summary>

  Что обычно получается на практике?

  - больше сервисов → больше сетевых запросов → больше точек отказа  
  - каскадные сбои становятся нормой  
  - таймауты, число ретраев и ограничения нагрузки  
    приходится постоянно поднастраивать  
  - недоступность лишь некоторых функций сложнее диагностировать  
  - распределённая трассировка становится обязательной,  
    чтобы понять, что вообще сломалось  
  - «self‑healing» часто означает «перезапустить и надеяться на лучшее»  

  Но надёжность не появляется автоматически — её нужно разработать и внедрить самому.
</details>
-->

---

# Why it happens

- Network is unreliable by nature  
- Latency spikes propagate across services  
- Dependencies create hidden chains of failure  
- Observability becomes a full‑time job  
- Resilience doesn’t simplify systems - it adds layers of complexity you must manage
- Teams underestimate the cost of distributed systems  

<!--
<details open>
  <summary>🇵🇱</summary>

  Dlaczego tak się dzieje?  

  - komunikacja sieciowa z natury nie jest niezawodna  
  - opóźnienia w jednym serwisie mnożą się,  
    przechodząc przez cały łańcuch wywołań  
  - monitoring staje się pracą na pełen etat  
  - dodawanie niezawodności zwiększa złożoność systemu,  
    a tą złożonością trzeba stale zarządzać  
  - zespoły często nie doceniają narzutów wynikających  
    z architektury rozproszonej
</details>

<details>
  <summary>🇷🇺</summary>

  Почему же так получается?

  - сетевое взаимодействие ненадёжно по своей природе  
  - задержки в одном сервисе умножаются,  
    проходя через цепочку всех вызовов  
  - мониторинг превращается в работу на полный день  
  - надёжность добавляет системе сложности,  
    и этой сложностью нужно постоянно управлять  
  - команды недооценивают накладные расходы  
    распределённых систем
</details>
-->

---
class: text-center
---

# Bottom line

### Microservices don’t make systems reliable.  
### They make reliability *your* responsibility.

Resilience isn’t a free benefit -  
it’s an engineering discipline you must build and maintain.

<!--
<details open>
  <summary>🇵🇱</summary>

  Wniosek  
  Mikroserwisy same w sobie nie czynią systemów bardziej niezawodnymi.  
  One jedynie zmuszają zespoły do pełnej odpowiedzialności  
  za niezawodność własnych usług.  

  Niezawodność nie jest darmowym dodatkiem —  
  trzeba ją zaprojektować, wdrożyć i utrzymywać.
</details>

<details>
  <summary>🇷🇺</summary>

  Вывод  
  Микросервисы не делают системы более надёжными.  
  Они лишь заставляют вас отвечать за надёжность своих сервисов.  

  Надёжность — не бесплатный бонус,  
  её нужно разработать, внедрить и сопровождать.
</details>
-->