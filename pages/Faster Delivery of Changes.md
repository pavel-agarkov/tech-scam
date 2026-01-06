# Faster Delivery of Changes  
## (Promise #1)

<!--
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
<details>
  <summary>🇷🇺</summary>
  На практике все становится только дольше<br/>
  Если начать пилить монолит без подготовки,<br/>
  то скорее всего бизнес логика окажется размазана по множеству сервисов,<br/>
  за которые возможно отвечают разные команды.<br/>
  Так что для внедрения новых фич понадобится гораздо больше времени, чем прежде.<br/>
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
<details>
  <summary>🇷🇺</summary>
  Так что если вы хотите ускорить внесение изменений, стоит начать с<br/>
  - рефакторинга легаси кода<br/>
   - уменьшения его сложности<br/>
   - улучшения модульности<br/>
  - покрытия кода тестами<br/>
  Даже монолит может быть чистым, модульным и быстрым в разработке<br/>
</details>
-->