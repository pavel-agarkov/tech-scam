# Horizontal Scalability  
## (Promise #5)

<!--
<details>
  <summary>🇷🇺</summary>
  Горизонтальное масштабирование
</details>
-->

---

# Monolith ≠ Not Scalable

- Modern monoliths:
  - run in containers  
  - are lightweight  
  - scale easily by running more copies  
- One image can serve multiple roles:
  - API  
  - worker  
  - scheduler  
  - message consumer  
- You don’t need Kubernetes to run 10 instances of your app

<!--
<details>
  <summary>🇷🇺</summary>
  Современные монолиты могут быть легкими и запускаться в контейнерах,<br/>
  тогда их легко масштабировать запуская больше копий или в разных ролях:<br/>
  API, worker, message handler...<br/>
  Так что вам не нужен целый класстер кубера, чтобы запустить 10 копий приложения...
</details>
-->