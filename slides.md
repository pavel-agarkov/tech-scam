---
theme: default
# colorSchema: dark
background: /images/cyberlit-wide-lite.png
title: Tech Scam
titleTemplate: "%s - by Pavel Agarkov"
info: |
  ## You don't need microservices and kubernetes to modernize your app
class: text-center
drawings:
  persist: false
transition: fade-out
mdc: true
duration: 15min
seoMeta:
  ogImage: auto
---

# Tech Scam
### by Pavel Agarkov
<style>
.slidev-layout {
  background-image: url(/images/cyberlit-wide-lite.png)!important;
}
h1 {
  letter-spacing: 0.3em;
  opacity: 0.6
}
h3 {
  opacity: 0.5
}
</style>

<div style="position:absolute;left:0;right:0;bottom:2rem;text-align:center" class="text-md opacity-50">
  You don't need microservices and kubernetes to modernize your app
</div>

<div class="abs-br m-6 text-xl">
  <a href="https://github.com/pavel-agarkov/tech-scam" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

<!--
<details open>
  <summary>🇵🇱</summary>
  
</details>

<details>
  <summary>🇷🇺</summary>
  Хотя презентация и называется "Техно-машейничество"<br/>
  Я, на самом деле, не буду называть микросервисы обманом<br/>
  Как это сделали другие...
</details>
-->

---
src: ./pages/tweet.html
---

---
title: Why “Microservices” Debates Miss the Point - CodeOpinion
---

<Youtube id="xYyLNkTky80" width="865vw" height="480vh" />

<!--
<details>
  <summary>🇷🇺</summary>
  Но я скорее склоняюсь к выводам сделанным Дереком из CodeOpinion<br/>
  Но давайте рассмотрим все по порядку
</details>
-->

---

# Hype as the Driver of Architecture

- Every decade brings a new “silver bullet”
- .com → SOA → blockchain → crypto → microservices → cloud → serverless → AI…
- It often feels like if you’re not using the trendy stack - you’re “behind”
- But hype ≠ solving your actual problems

<!--
<details style="font-size:12px">
  <summary>🇷🇺</summary>
  Каждые несколько лет анонсируется новая технология,<br/>
  которая, на этот раз, должна решить все проблемы...<br/>
  Каждый раз обещается, что нужно всего-лишь добавить вот эту последнюю новинку и тогда точно все взлетит...<br/>
  Но речь не идет о том, что технологии сами по себе плохие,<br/>
  скорее они начинают применяться на лево и на право без разбору...<br/>
    <details>
      Но зачем локальной лавочке вэб-сайт...  
      Про SOA я вообще молчу - на моих глазах контора, в которой внедряли ESB, практически обонкротилась из-за этого,  
      хотя на тот момент в индустрии уже начинали понимать, что так строить системы не стоит...  
      Блокчейн же, например, продавался в электронном голосовании как защита от внешнего вмешательства: мол, никто не сможет подделать голоса. Но если результаты выборов объявляются не по данным системы, а по заранее заданному сценарию, то вмешиваться в саму систему никому и не нужно. Технология становится декоративной - она защищает данные, которые всё равно не используются. Никакая технология не может заставить себя использовать, пока что...
      Эта же проблема, помимо прочих, лежит и в основе крипты...
    </details>
  Но сегодня мы разговариваем о микросервисах и о проблемах,<br/>
  которые на самом деле стоило бы решать, даже если в этом нет никакого хайпа.<br/>
  Хотя, даже если мы и знаем какие проблемы на самом деле нужно решать,<br/>
  мы еще зачастую пытаемся выбрать метод, который нам нравится,<br/>
  а это не всегда самый оптимальный вариант.<br/>
</details>
-->

---
layout: image
# src: ./diagrams/slidev.puml
image: /diagrams/slidev.svg
backgroundSize: contain
---

<!--
<details>
  <summary>🇷🇺</summary>
  Примером такого overengineeringa может служить данная презентация,<br/>
  созданная с помощью Slidev. Такая презентация разрабатывается локально<br/>
  с использованием Markdown, HTML, CSS, PlantUML и других ресурсов,
  затем исходные файлы пушатся в репозитории на GitHub,<br/>
  где с помощью GitHub Actions автоматически собирается статический сайт,<br/>
  который разворачивается на GitHub Pages для публичного доступа.<br/>
  Получается гораздо сложнее, чем просто создать слайды в PowerPoint<br/>
  или Google Slides, но при этом никаких ощутимых преимуществ.
</details>
-->

---

# What Microservices are often expected to bring

- 🚀 Faster delivery of changes  
- ⚡ Faster deployments  
- 🧩 Independent teams  
- 🔄 Reliability and resilience  
- 📈 Horizontal scalability  

<!--
<details>
  <summary>🇷🇺</summary>
  Давайте посмотрим, что обычно ассоциируется с микросервисами,<br/>
  хотя на деле скорее является предусловием их внедрения.<br/>
  - Быстрое внедрение новых фич<br/>
  - Быстрое развертывание<br/>
  - Горизонтальное масштабирование<br/>
  - Независимость команд<br/>
  - Надежность и отказоустойчивость<br/>
</details>
-->

---
src: ./pages/Faster Delivery of Changes.md
---

---
src: ./pages/Faster Deployments.md
---

---
src: ./pages/Independent Teams.md
---

---
src: ./pages/Reliability & Resilience.md
---

---
src: ./pages/Horizontal Scalability.md
---

---
src: ./pages/Kubernetes.md
---

---

# When Microservices Actually Make Sense

- You have a **very large team** (100+ developers)
- Your product has **clear, independent domains**
- You need **technology stack independence**
- You require **isolated scalability** for specific components
- You have **skills and resources** to operate complex infrastructure

<!--
<details>
  <summary>🇷🇺</summary>
  Когда же Микросервисы на самом деле имеют смысл<br/>
  - Если у вас очень большая команда<br/>
  - В вашем безнесе четко выделимы независимые домены<br/>
  - Вам нужна технологическая независимость (возможно из-за санкций)<br/>
  - Вам нужно масштабировать определенные компоненты<br/>
  - И у вас есть навыки и ресурсы, чтобы поддреживать всю эту сложную инфраструктуру
</details>
-->

---
layout: two-cols-header
---

# What To Do Instead of Microservices  
## Microservices don’t fix fundamental development problems  
<br/>
<br/>

<div class="grid grid-cols-3 gap-8">
<div>

### Improve architecture
<br/>

- Extract modules  
- Introduce layers / slices  
- Remove cyclic dependencies  

</div><div>

### Invest in automation  
<br/>

- Tests  
- CI/CD  
- Infrastructure as Code  

</div><div>

### Add observability
<br/>

- Logging  
- Metrics  
- Tracing  

</div></div>

<!--
<details>
  <summary>🇷🇺</summary>
  Что же делать вместо Микросервисов<br/>
  Микросервисы не решают базовых проблем разработки,<br/>
  поэтому стоит начать именно с них<br/>

  - Улучшить архитекруру<br/>
    - Выделить модули<br/>
    - Разделить на уровни / ломтики<br/>
    - Убрать циклические зависимости<br/>

  - Вложиться в автомотизацию<br/>
    - Тесты<br/>
    - CI/CD<br/>
    - Infrastructure as Code<br/>

  - Расширить наблюдаемость системы<br/>
    - логирование<br/>
    - метрики<br/>
    - трассировка<br/>
</details>
-->

---
# layout: center
class: text-center
---

# Bottom line

### A monolith can be fast, maintainable, and modern.  
### Microservices are an evolution — not a rescue plan.  

If the basics are broken, no architecture will save the project.

<!--
<details>
  <summary>🇷🇺</summary>
  Вывод<br/>
  Монолит тоже может быть бастрым, легким для разработки и современным<br/>
  Внедрение Микросервисов это эволюционный шаг, а не спасательный круг...<br/>
  Если фундамент проседает, никакая архитектура не спасет здание...<br/>
</details>
-->

---

# Thank You!

<style>
.slidev-layout {
  text-align: center;
}
h1 {
  opacity: 0.8
}
h2 {
  opacity: 0.6
}
h3 {
  opacity: 0.5
}
h4 {
  opacity: 0.45
}
</style>

## Questions & Discussion
#### also online in [GitHub issue #1](https://github.com/pavel-agarkov/tech-scam/issues/1)


<img src="/images/qr.png" style="display: inline; margin: 1rem;" width="200px">

### Link to the presentation

<br/>

<PoweredBySlidev mt-10 opacity-50 />

<!--
<details>
  <summary>🇷🇺</summary>
  Спасибо за внимание<br/>
  Вопросы можно задать сейчас либо в Issue на GitHub<br/>
  Вот ссылка на эту презентацию
</details>
-->
