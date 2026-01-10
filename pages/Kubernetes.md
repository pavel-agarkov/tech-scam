# Kubernetes: What We Expected

1. Easy zero‑downtime deployments  
2. Automatic metric based scaling  
3. Independent teams deploying independently  
4. Built‑in reliability & resilience  
5. Cost efficiency through optimal resource usage  
6. Infrastructure as Code for everything  
7. Unified platform for all workloads

<!--
<details open>
  <summary>🇵🇱</summary>

  Załóżmy, że jednak zdecydowaliście się na mikroserwisy  
  i zastanawiacie się, czy potrzebujecie Kubernetesa.  
  Czego ludzie zwykle oczekują od niego „z pudełka”?  

  - aktualizacji bez przestojów  
  - automatycznego skalowania na podstawie metryk  
  - wbudowanej niezawodności i odporności na awarie  
  - oszczędności kosztów dzięki optymalnemu wykorzystaniu zasobów  
  - pełnego opisu infrastruktury w formie kodu  
  - obsługi różnych typów aplikacji (API, Worker, Job)

  Ale czy wszystkie te funkcje są dostępne wyłącznie w Kubernetesie?
</details>

<details>
  <summary>🇷🇺</summary>

  Ок, вы всё‑таки решились на микросервисы  
  и раздумываете, нужен ли вам кубер.  
  Что же люди ожидают от него «из коробки»?  

  - обновления без остановки работы  
  - автоматическое масштабирование на основе метрик  
  - встроенная надёжность и отказоустойчивость  
  - выгодная стоимость за счёт оптимального использования ресурсов  
  - полное описание инфраструктуры в виде кода  
  - поддержка разных типов приложений (API, Worker, Job)

  Но доступны ли все эти фишки только для Кубера?
</details>
-->

---

# How to Achieve the Same (Without Kubernetes)

1. **Zero‑downtime deployments**  
   → App Service blue‑green deployments with deployment slots

2. **Automatic metric based scaling**  
   → App Service autoscale rules / Function App consumption plan

3. **Independent deployments for teams**  
   → Separate App Services / Function Apps per domain + isolated pipelines

4. **Reliability & resilience**  
   → Built‑in health checks, auto‑healing, retries, regional redundancy

5. **Cost efficiency**  
   → App Service Plans are cheaper than Container Apps under constant load

6. **Infrastructure as Code**  
   → Terraform / CDKTF modules for App Service, Function App, storage, networking

7. **Unified platform**  
   → Azure App Platform (App Service + Functions + API Management)

<!--
<details open>
  <summary>🇵🇱</summary>

  Jak to wszystko zrealizować bez Kubernetesa?  
  Zamiast tego wykorzystajmy App Service, Function App i CDKTF.  

  - **aktualizacje bez przestojów**  
    → stosujemy **blue‑green na deployment slotach**:  
      dla każdej wersji tworzymy nowy slot, uruchamiamy aplikację,  
      **stopniowo przekierowujemy ruch**,  
      a poprzedni slot wyłączamy dopiero po pewnym czasie.  

      **Dlaczego nie używamy slot swap?**  
      Swap przełącza całe środowisko i powoduje restart aplikacji,  
      co może przerwać aktualnie obsługiwane żądania —  
      dlatego bezpieczniej jest tworzyć nowy slot, uruchamiać go  
      i stopniowo przekierowywać ruch.  

  - **automatyczne skalowanie na podstawie metryk**  
    → zarówno App Service, jak i Function App potrafią automatycznie  
      skalować się na podstawie metryk,  
      np. liczby żądań lub długości kolejki wiadomości  

  - **wbudowana niezawodność i odporność na awarie**  
    → App Service ma natywnie health checks, auto‑healing, retries  
      oraz możliwość redundancji regionalnej  

  - **korzystna cena dzięki optymalnemu wykorzystaniu zasobów**  
    → jeśli aplikacja ma stabilne obciążenie,  
      App Service będzie prawdopodobnie znacznie tańszy  
      niż np. Container Apps  

  - **pełny opis infrastruktury w kodzie**  
    → do IaC wcale nie trzeba używać YAML  
      My korzystamy z Terraform i CDKTF,  
      które w pełni wspierają Azure  
      CDKTF pozwala opisywać infrastrukturę w ulubionym języku  
      w naszym przypadku w C#, co daje ogromne korzyści  
      zarówno względem statycznych definicji,  
      jak i języków, w których nie jesteśmy ekspertami  

  - **różne typy aplikacji (API, Worker, Job)**  
    → App Service może działać nie tylko jako API, ale również jako worker,  
      np. do obsługi wiadomości z kolejki  
      Function App również to potrafi,  
      a dodatkowo może działać jako cron‑job
</details>

<details>
  <summary>🇷🇺</summary>

  Как можно всё это реализовать без Кубера?  
  Вместо этого возьмём App Service, Function App и CDKTF.

  - обновления без остановки работы  
    → используем **blue‑green на deployment слотах**:  
      для каждого релиза создаётся новый слот, приложение прогревается,  
      **трафик постепенно переводится**,  
      а предыдущий слот отключается только спустя время.  
      **Почему не используем slot swap?**  
      Swap переключает всё окружение и перезапускает приложение,  
      что может оборвать выполняющиеся запросы —  
      поэтому надёжнее создавать новый слот, прогревать его  
      и постепенно переводить трафик.  

  - автоматическое масштабирование на основе метрик  
    → и App Service, и Function App могут автоматически  
      масштабироваться на основе метрик,  
      например количества запросов или длины очереди сообщений  

  - встроенная надёжность и отказоустойчивость  
    → в App Service уже есть health checks, auto‑healing, retries  
      и региональная избыточность  

  - выгодная стоимость за счёт оптимального использования ресурсов  
    → если приложение имеет стабильную нагрузку,  
      App Service, скорее всего, будет значительно дешевле,  
      чем, например, Container Apps  

  - полное описание инфраструктуры в коде  
    → для IaC необязательно использовать YAML  
      Мы, например, используем Terraform и CDKTF,  
      которые полностью покрывают Azure  
      CDKTF позволяет описывать инфраструктуру на любимом языке  
      в нашем случае на C#, что даёт огромные преимущества  
      как по сравнению со статическими описаниями,  
      так и с языками, в которых мы не специалисты  

  - различные типы приложений (API, Worker, Job)  
    → App Service может быть не только API, но и worker’ом,  
      например для обработки сообщений из очереди  
      Function App тоже это умеет,  
      а ещё может работать как cron‑job
</details>
-->