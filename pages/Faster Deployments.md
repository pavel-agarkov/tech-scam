# Faster Deployments  
## (Promise #2)

<!--
<details>
  <summary>🇷🇺</summary>
  Быстрое развертывание
</details>
-->

---

# Why Are Deployments Slow?

- Usually because of **manual steps**:
  - manual or sequential testing  
  - manual approvals  
  - manual deployments  
  - manual resource provisioning  
- Microservices don’t magically fix this  
- In fact, they multiply the problem if it is not solved upfront  

<!--
<details>
  <summary>🇷🇺</summary>
  Обычно деплойменты медленные из-за множества ручных шагов.<br/>
  Будь то ручные тесты, ручная подготовка инфраструктуры,<br/>
  согласования или сам процесс выкладки путем копирования файлов.<br/>
  Микросервисы никак не решают эти проблемы,<br/>
  даже наоборот - делают их более явными.
</details>
-->

---

# Want Fast Deployments?

## Invest in Automation First
<br/>

- CI/CD **must** be fully automated:
  - build  
  - parallel testing  
  - static analysis  
  - deployment  
- Automation speeds up deployments **in monoliths just as well**
- Microservices is just an architecture choise - not a cure for slow processes

<!--
<details>
  <summary>🇷🇺</summary>
  Для ускорения развертывания обязательно нужна полная автоматизация.<br/>
  Автоматизация ускоряет развертывание и в монолитах ни чуть не хуже.<br/>
  Микросервисы это лишь архитектурное решение<br/>
  а не понацея от медленных процессов
</details>
-->