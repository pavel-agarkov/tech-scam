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
duration: 20min
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

  Mimo że prezentacja nazywa się „Techno‑oszustwa”,  
  nie zamierzam nazywać mikroserwisów oszustwem.  
  W przeciwieństwie do niektórych innych…
</details>

<details>
  <summary>🇷🇺</summary>

  Хотя презентация и называется "Техно-машейничество"  
  Я, на самом деле, не буду называть микросервисы обманом  
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
<details open>
  <summary>🇵🇱</summary>

  Bardziej zgadzam się z wnioskami Dereka z CodeOpinion.  
  Ale zacznijmy wszystko po kolei.
</details>

<details>
  <summary>🇷🇺</summary>

  Но я скорее склоняюсь к выводам, сделанным Дереком из CodeOpinion.  
  Но давайте рассмотрим всё по порядку.
</details>
-->


---
hide: true
---

# Hype as the Driver of Architecture

- Every decade brings a new “silver bullet”
- .com → SOA → blockchain → crypto → microservices → cloud → serverless → AI…
- It often feels like if you’re not using the trendy stack - you’re “behind”
- But hype ≠ solving your actual problems

<!--
<details open>
  <summary>🇵🇱</summary>

  Co kilka lat pojawia się nowa technologia, która rzekomo ma rozwiązać wszystkie problemy.  
  Za każdym razem słyszymy, że wystarczy dodać tę „ostatnią nowość” i wszystko wreszcie zacznie działać idealnie.  

  Same technologie nie są złe — problem w tym, że zaczyna się je stosować wszędzie, bez zastanowienia i bez kontekstu.  

  <details>
    <summary>Przykłady</summary>

    Po co małemu lokalnemu biznesowi rozbudowana strona internetowa?  
    Z SOA też bywało ciekawie — widziałem firmę, która prawie zbankrutowała przez wdrażanie ESB,  
    mimo że branża już wtedy zaczynała rozumieć, że to nie jest właściwy sposób budowania systemów.  

    Blockchain sprzedawano w e‑głosowaniu jako ochronę przed manipulacją: niby nikt nie podrobi wyników.  
    Tylko że jeśli wyniki i tak ogłasza się według z góry ustalonego scenariusza,  
    to nikt nie musi ingerować w samą technologię.  
    Staje się dekoracją — chroni dane, których nikt nie używa.  
    Żadna technologia nie zmusi nikogo do korzystania z niej.  

    Podobny problem, choć w innej formie, leży u podstaw kryptowalut.  
  </details>

  Dziś jednak mówimy o mikroserwisach i o problemach,  
  które naprawdę warto rozwiązać — nawet jeśli nie są modne.  

  <details>
    Nawet kiedy wiemy, jakie problemy są kluczowe,  
    często wybieramy metod, który nam się podoba,  
    a nie ten, który jest optymalny.  
  </details>
</details>

<details style="font-size:12px">
  <summary>🇷🇺</summary>

  Каждые несколько лет анонсируется новая технология,  
  которая, на этот раз, должна решить все проблемы.  

  Каждый раз обещается, что нужно всего лишь добавить вот эту последнюю новинку — и тогда точно всё взлетит.  

  Но речь не о том, что технологии сами по себе плохие,  
  скорее они начинают применяться направо и налево, без разбора.  

  <details>
    <summary>Примеры</summary>

    Но зачем локальной лавочке сложный веб‑сайт?  
    Про SOA я вообще молчу — на моих глазах компания, внедрявшая ESB, практически обанкротилась,  
    хотя в индустрии уже начинали понимать, что так строить системы не стоит.  

    Блокчейн, например, продавался в электронном голосовании как защита от вмешательства:  
    мол, никто не сможет подделать голоса.  
    Но если результаты выборов объявляются не по данным системы, а по заранее заданному сценарию,  
    то вмешиваться в систему никому и не нужно.  
    Технология становится декоративной — она защищает данные, которые всё равно не используются.  
    Никакая технология не может заставить себя использовать.  

    Эта же проблема, среди прочих, лежит и в основе криптовалют.  
  </details>

  Но сегодня мы говорим о микросервисах и о проблемах,  
  которые действительно стоило бы решать, даже если вокруг них нет хайпа.  
  
  <details>
    И даже когда мы понимаем, какие проблемы важны,  
    мы всё равно часто выбираем метод, который нам нравится,  
    а не тот, который действительно оптимален.  
  </details>
</details>
-->

---
layout: image
# src: ./diagrams/slidev.puml
image: /images/slidev.svg
backgroundSize: contain
hide: true
---

<!--
<details open>
  <summary>🇵🇱</summary>

  Dobrym przykładem takiego „przeinżynierowania” jest właśnie ta prezentacja.  
  Powstała w Slidev — tworzona lokalnie w Markdownie, HTML‑u, CSS‑ie, z użyciem PlantUML i innych narzędzi.  
  Potem pliki źródłowe trafiają do repozytorium na GitHubie,  
  gdzie GitHub Actions buduje statyczną stronę i publikuje ją na GitHub Pages.  

  W efekcie cały proces jest znacznie bardziej skomplikowany  
  niż po prostu przygotowanie slajdów w PowerPoint lub Google Slides,  
  a realnych korzyści z tego — niewiele.  
</details>

<details>
  <summary>🇷🇺</summary>

  Примером такого оверинжиниринга может служить эта презентация,  
  созданная с помощью Slidev. Такая презентация разрабатывается локально  
  с использованием Markdown, HTML, CSS, PlantUML и других ресурсов.  
  Затем исходные файлы пушатся в репозиторий на GitHub,  
  где GitHub Actions автоматически собирает статический сайт,  
  который разворачивается на GitHub Pages для публичного доступа.  

  В итоге всё получается гораздо сложнее, чем просто сделать слайды  
  в PowerPoint или Google Slides, и при этом почти без ощутимых преимуществ.  
</details>
-->

---

# What Microservices are often expected to bring

- 🚀 Faster delivery of changes  
- ⚡ Faster and often deployments  
- 🧩 Independent teams  
- 🔄 Reliability and resilience  
- 📈 Horizontal scalability  
<!--
<details open>
  <summary>🇵🇱</summary>

  Spójrzmy, z czym najczęściej kojarzy się architektura mikroserwisowa —  
  choć w praktyce są to raczej warunki wstępne,  
  które trzeba spełnić, aby w ogóle móc ją wdrożyć.  

  - szybkie dostarczanie nowych funkcji  
  - szybkie i częste wdrażanie  
  - niezależność zespołów  
  - wysoka niezawodność i odporność na awarie  
  - skalowanie horyzontalne  
</details>

<details>
  <summary>🇷🇺</summary>

  Давайте посмотрим, что обычно ассоциируется с микросервисами,  
  хотя на деле это скорее предусловия для их внедрения.  

  - быстрое внедрение новых фич  
  - быстрое развертывание  
  - независимость команд  
  - надёжность и отказоустойчивость  
  - горизонтальное масштабирование  
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

- You have a **very large team** (or a few smaller)
- Your product has **clear, independent domains**
- You need **technology stack independence**
- You require **isolated scalability** for specific components
- You have **skills and resources** to operate complex infrastructure
<!--
<details open>
  <summary>🇵🇱</summary>

  Kiedy mikroserwisy naprawdę mają sens?  

  - gdy zespół jest bardzo duży (albo kilka mniejszych)  
  - gdy w biznesie da się jasno wydzielić niezależne domeny  
  - gdy potrzebna jest niezależność technologiczna  
    (np. z powodów regulacyjnych lub geopolitycznych)  
  - gdy trzeba skalować tylko wybrane komponenty  
  - i gdy organizacja ma kompetencje oraz zasoby,  
    aby utrzymać całą tę złożoną infrastrukturę
</details>

<details>
  <summary>🇷🇺</summary>

  Когда же микросервисы на самом деле имеют смысл?  

  - если у вас очень большая команда  
  - если в вашем бизнесе чётко выделяются независимые домены  
  - если вам нужна технологическая независимость (возможно, из‑за санкций)  
  - если вам нужно масштабировать только определённые компоненты  
  - и если у вас есть навыки и ресурсы, чтобы поддерживать всю эту сложную инфраструктуру  
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
<details open>
  <summary>🇵🇱</summary>

  Co robić zamiast mikroserwisów?  
  Mikroserwisy nie rozwiązują podstawowych problemów inżynierskich,  
  więc właśnie od nich warto zacząć.  

  - poprawa architektury  
    - wyodrębnienie modułów  
    - podział na warstwy lub „plastry”  
    - eliminacja zależności cyklicznych  

  - inwestycja w automatyzację  
    - testy  
    - CI/CD  
    - Infrastructure as Code  

  - zwiększenie obserwowalności systemu  
    - logowanie  
    - metryki  
    - tracing  

</details>

<details>
  <summary>🇷🇺</summary>

  Что же делать вместо микросервисов?  
  Микросервисы не решают базовых проблем разработки,  
  поэтому стоит начать именно с них.  

  - улучшить архитектуру  
    - выделить модули  
    - разделить на уровни или «ломтики»  
    - убрать циклические зависимости  

  - вложиться в автоматизацию  
    - тесты  
    - CI/CD  
    - Infrastructure as Code  

  - расширить наблюдаемость системы  
    - логирование  
    - метрики  
    - трассировка  
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
<details open>
  <summary>🇵🇱</summary>

  Wnioski  
  Monolit również może być szybki, nowoczesny i wygodny w rozwoju.  
  Wprowadzenie mikroserwisów to krok ewolucyjny, a nie koło ratunkowe.  
  Jeśli fundament jest słaby, żadna architektura nie uratuje całej konstrukcji.  
</details>

<details>
  <summary>🇷🇺</summary>

  Вывод  
  Монолит тоже может быть быстрым, современным и удобным в разработке.  
  Внедрение микросервисов — это эволюционный шаг, а не спасательный круг.  
  Если фундамент проседает, никакая архитектура не спасёт здание.
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
<details open>
  <summary>🇵🇱</summary>

  Dziękuję za uwagę.  
  Pytania można zadać teraz albo zgłosić w Issue na GitHubie.  
  Tutaj znajduje się link do tej prezentacji.  
</details>

<details>
  <summary>🇷🇺</summary>

  Спасибо за внимание.  
  Вопросы можно задать сейчас либо оставить в Issue на GitHub.  
  Вот ссылка на эту презентацию.
</details>
-->
