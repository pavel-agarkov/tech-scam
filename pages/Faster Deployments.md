# Faster and Often Deployments  
## (Promise #2)

<!--
<details open>
  <summary>🇵🇱</summary>
  Szybkie i częste wdrażanie
</details>
<details>
  <summary>🇷🇺</summary>
  Быстрое и частое развертывание
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
<details open>
  <summary>🇵🇱</summary>

  Czemu mamy wolne wdrożenia?  

  Wolne wdrożenia najczęściej wynikają z dużej liczby ręcznych kroków —  
  manualnych testów, ręcznego przygotowania infrastruktury, uzgodnień  
  czy samego procesu publikacji opartego na kopiowaniu plików.  

  Mikroserwisy nie rozwiązują tych problemów.  
  Wręcz przeciwnie — sprawiają, że stają się jeszcze bardziej widoczne.
</details>

<details>
  <summary>🇷🇺</summary>

  Почему развертывание медленное?  

  Обычно деплойменты медленные из‑за множества ручных шагов —  
  будь то ручные тесты, ручная подготовка инфраструктуры, согласования  
  или сам процесс выкладки путём копирования файлов.  

  Микросервисы никак не решают эти проблемы,  
  а наоборот — делают их более явными.
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
<details open>
  <summary>🇵🇱</summary>

  Aby przyspieszyć wdrażanie, pełna automatyzacja jest absolutnie konieczna.  
  Automatyzacja przyspiesza deploymenty również w monolitach — i to wcale nie gorzej.  
  Mikroserwisy są jedynie decyzją architektoniczną,  
  a nie lekarstwem na wolne procesy.
</details>

<details>
  <summary>🇷🇺</summary>

  Для ускорения развертывания обязательно нужна полная автоматизация.  
  Автоматизация ускоряет развертывание и в монолитах ничуть не хуже.  
  Микросервисы — это лишь архитектурное решение,  
  а не панацея от медленных процессов.
</details>
-->