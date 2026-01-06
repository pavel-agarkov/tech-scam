

# Reliability & Resilience  
## (Promise #4)

<!--
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
<details>
  <summary>🇷🇺</summary>
  Обещание<br/>
  - Каждый сервис выходит из строя независимо от других<br/>
  - Circuit breakers, retries, timeouts → встроенные из коробки<br/>
  - Возможность горизонтального масштабирования улучшает доступность<br/>
  - Распределенная архитектура устойчива к сбоям по определению<br/>

  Так что, в теории, микросервисы должны сделать сбои менее значимыми и редкими<br/>
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
<details>
  <summary>🇷🇺</summary>
  Что обычно получается на практике<br/>
  - Больше сервисов → больше сетевых запросов → больше точек отказа<br/>
  - Каскадные сбои становятся нормой<br/>
  - Таймауты, число ретраев, ограничение нагрузки<br/>
    приходится постоянно поднастраивать<br/>
  - Недоступность лишь некоторых функций сложнее диагностировать<br/>
  - Распределенная трассировка становится обязательной,<br/>
    чтобы понять что вообще сломалось<br/>
  - "Self‑healing" часто означает "рестартануть и надейться на лучшее"<br/>

  Но надежность не появляется автоматически - ее нужно разработать и внедрить самому
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
<details>
  <summary>🇷🇺</summary>
  Почему же так получается<br/>
  - Сетевое взаимодействие не надежно по своей природе<br/>
  - Задержки в одном сервисе умножаются,<br/>
    проходя через цепочку всех вызовов<br/>
  - Мониторинг становится должностью на полную ставку<br/>
  - Надежность добавляет сложности системе<br/>
    и этой сложностья нужно постоянно управлять<br/>
  - Команды недооценивают накладные расходы распределенных систем<br/>
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
<details>
  <summary>🇷🇺</summary>
  Вывод<br/>
  Микросервисы не делаю системы более надежными<br/>
  Они заставляют вас отвечать за надежность своих сервисов<br/>
  <br/>
  Надежность не бесплатный бонус - ее нужно разработать, внедрить и сопровождать<br/>
</details>
-->