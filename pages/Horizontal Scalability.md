# Horizontal Scalability  
## (Promise #5)

<!--
<details open>
  <summary>🇵🇱</summary>
  Skalowanie horyzontalne
</details>
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
<details open>
  <summary>🇵🇱</summary>

  Monolit nie oznacza niedostępność skalowania  

  Współczesne monolity mogą być lekkie i uruchamiane w kontenerach.  
  Dzięki temu łatwo je skalować — wystarczy uruchomić więcej instancji  
  albo podzielić je na różne role, takie jak API, worker czy message handler.  

  Nie potrzebujesz do tego całego klastra Kubernetesa,  
  żeby uruchomić dziesięć kopii aplikacji.
</details>

<details>
  <summary>🇷🇺</summary>

  Монолит не означает невозможность масштабирования  

  Современные монолиты могут быть лёгкими и запускаться в контейнерах.  
  Тогда их легко масштабировать, запуская больше копий  
  или распределяя по разным ролям: API, worker, message handler.  

  Так что вам не нужен целый кластер кубера, чтобы запустить десять копий приложения.
</details>
-->