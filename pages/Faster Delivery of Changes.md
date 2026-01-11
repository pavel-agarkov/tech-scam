# Faster Delivery of Changes  
## (Promise #1)

<!--
<details open>
  <summary>🇵🇱</summary>
  Szybkie dostarczanie nowych funkcji
</details>

<details>
  <summary>🇷🇺</summary>
  Быстрое внедрение новых фич
</details>
-->

---

# In Reality, It Often Gets Slower

- After splitting a monolith, logic often becomes **scattered across many services**
- To change one business function, you now must:
  - understand which services participate  
  - update APIs and contracts  
  - coordinate with other teams  
  - deploy multiple components  
- What used to take 2 hours can now take 2 days

<!--
<details open>
  <summary>🇵🇱</summary>

  W praktyce wszystko trwa tylko dłużej.  
  Jeśli zacząć dzielić monolit na mikroserwisy bez przygotowania,  
  logika biznesowa szybko rozleje się po wielu komponentach,  
  często rozwijanych przez różne zespoły.  
  W efekcie wdrażanie nowych funkcji zajmuje znacznie więcej czasu niż wcześniej.
</details>

<details>
  <summary>🇷🇺</summary>

  На практике всё становится только дольше.  
  Если начать пилить монолит без подготовки,  
  то бизнес‑логика, скорее всего, окажется размазанной по множеству компонентов,  
  за которые могут отвечать разные команды.  
  В итоге внедрение новых фич займёт гораздо больше времени, чем раньше.
</details>
-->
---

# If Your Goal Is Faster Changes…

## …microservices are not the first step
<br/>

- The real problem is usually **legacy code quality**, not architecture style
- Start with:
  - refactoring  
   - modularization  
   - reducing complexity  
  - improving test automation  
- A monolith can be **clean, modular, and fast to develop**
<!--
<details open>
  <summary>🇵🇱</summary>

  Jeśli naprawdę chcemy przyspieszyć wprowadzanie zmian,  
  warto zacząć od podstaw:  

  - refaktoryzacji legacy  
    - uproszczenia nadmiernie skomplikowanych fragmentów  
    - poprawy modułowości  

  - zwiększenia pokrycia testami  

  Nawet monolit może być czysty, modularny i szybki w rozwoju.
</details>

<details>
  <summary>🇷🇺</summary>

  Так что если вы хотите ускорить внесение изменений, стоит начать с:

  - рефакторинга легаси‑кода  
    - уменьшения его сложности  
    - улучшения модульности  

  - покрытия кода тестами  

  Даже монолит может быть чистым, модульным и быстрым в разработке.
</details>
-->