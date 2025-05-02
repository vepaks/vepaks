<p align="center">
  <img src="https://github.com/vepaks/vepaks/blob/main/public/gif/rf.gif" alt="animated" />
</p>

<h1 align="center">Александър Камбуров - DevOps & Инфраструктура</h1>

<p align="center">
  <a href="https://linkedin.com/in/vepaks"><img src="https://img.shields.io/badge/LinkedIn-Александър_Камбуров-blue?style=flat-square&logo=linkedin" alt="LinkedIn"></a>
  <a href="https://vepaks.dev"><img src="https://img.shields.io/badge/Website-vepaks.dev-green?style=flat-square&logo=safari" alt="Website"></a>
  <img src="https://img.shields.io/badge/OS-Linux-orange?style=flat-square&logo=linux" alt="OS">
  <img src="https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square" alt="License">
</p>

<p align="center"><i>DevOps инженер специализиран в автоматизацията, инфраструктурата и облачните решения</i></p>

---

## 📋 Съдържание

- [🚀 Въведение](#-въведение)
- [🛠️ Технологичен стак](#️-технологичен-стак)
- [📊 Проекти](#-проекти)
  - [Ansible Роли](#-ansible-роли)
  - [Linux Скриптове](#-linux-скриптове)
  - [Self-Hosted Услуги](#-self-hosted-услуги)
- [💡 Експертиза](#-експертиза)
- [📚 Текущо обучение](#-текущо-обучение)
- [📞 Контакти](#-контакти)

---

## 🚀 Въведение

Това хранилище съдържа моето професионално портфолио и документация на проектите, върху които работя. Специализирам в:

- **Инфраструктура като код** с Terraform и Ansible
- **Контейнеризация и оркестрация** с Docker и Kubernetes
- **Автоматизация** на CI/CD процеси
- **Мониторинг** на системи и услуги
- **Облачни решения** и системна администрация

> *"Всичко е файл"* - философията на Linux, която прилагам в ежедневната си работа

---

## 🛠️ Технологичен стак

<div align="center">

| Категория | Технологии |
|-----------|------------|
| 🐳 **Контейнеризация** | `Docker` `Docker Compose` `Kubernetes` `Minikube` |
| ☁️ **Облак & IaC** | `AWS` `Terraform` `Ansible` |
| 🔄 **CI/CD** | `GitHub Actions` `GitLab CI/CD` `Jenkins` |
| 📊 **Мониторинг** | `Prometheus` `Grafana` |
| 🔒 **Сигурност** | `HashiCorp Vault` `SSL/TLS` |
| 🌐 **Сървъри** | `Nginx` |
| 📜 **Скриптове** | `Bash` `Python` |
| 💾 **OS** | `Linux (Ubuntu/openSUSE/Arch)` |

</div>

---

## 📊 Проекти

### 🔸 Ansible Роли

Колекция от модулни, многократно използваеми Ansible роли, проектирани за автоматизирана конфигурация и управление на различни аспекти на Linux сървъри и облачна инфраструктура.

#### Основни компоненти:

* **Базова инфраструктура**
  * `common` - Основна настройка на сървъра: име на хоста, часова зона, системни настройки
  * `docker` - Инсталация и конфигурация на Docker Engine и Docker Compose
  * `nginx` - Настройка на NGINX уеб сървър с оптимизирани конфигурации
  * `php` - Инсталация на PHP с PHP-FPM, Composer и разширения
  * `mysql` - Инсталация и оптимизация на MySQL/MariaDB сървър

* **Облачни технологии**
  * `aws` - AWS интеграционни инструменти и конфигурации
  * `terraform` - Terraform интеграция за инфраструктура като код
  * `kubernetes` - Инсталация и конфигурация на Kubernetes клъстер
  * `minikube` - Локална Kubernetes среда за разработка

* **Сигурност и мониторинг**
  * `vault` - HashiCorp Vault за управление на тайни
  * `certificates` - Управление на SSL/TLS сертификати
  * `monitoring` - Инструменти за мониторинг с Prometheus и Grafana
  * `security` - Подобряване на системната сигурност

* **Помощни инструменти**
  * `zsh` - Конфигурация на ZSH обвивка с Oh-My-Zsh
  * `database_backup` - Автоматизирано решение за архивиране на бази данни
  * `ansible_bootstrap` - Подготовка на сървъри за управление с Ansible

#### Използване:

```yaml
---
- hosts: webservers
  become: true
  roles:
    - role: common
      vars:
        timezone: "Europe/Sofia"
        
    - role: nginx
      vars:
        nginx_sites:
          - server_name: example.com
            root: /var/www/example
```

### 🔸 Linux Скриптове

Колекция от лични скриптове за инсталация и управление на Linux приложения и услуги, създадени и използвани за автоматизация на ежедневни задачи в Linux среда.

#### Основни категории:

* **Системна администрация**
  * Управление на потребители, процеси и планирани задачи
  * Автоматизация на рутинни административни задачи
  
* **Мрежова конфигурация**
  * Настройка на мрежови интерфейси, DNS, DHCP
  * Конфигуриране на Nginx като reverse proxy с SSL поддръжка
  
* **Сигурност**
  * Настройка на защитни стени, SSH, SSL/TLS сертификати
  * Инструменти за одит и наблюдение на сигурността
  
* **Контейнеризация и виртуализация**
  * Управление на Docker, Kubernetes, Podman
  * Инструменти за KVM, libvirt, VirtualBox
  
* **CI/CD и автоматизация**
  * Скриптове за Jenkins, GitLab CI, GitHub Actions
  * Интеграция с Terraform и Ansible
  
* **Мониторинг и логиране**
  * Настройка на Prometheus, Grafana, ELK
  * Управление и ротация на логове

### 🔸 Self-Hosted Услуги

Система от самостоятелно хоствани услуги за разработка и операции:

* **Gitea репозиторий сървър** на vepaks.dev
  * Алтернатива на GitHub за частни проекти
  * Интеграция с CI/CD пайплайни
  
* **Jenkins CI/CD инструмент**
  * Автоматизирано тестване и деплойване
  * Интеграция с контейнери и облачни услуги
  
* **Grafana мониторинг платформа**
  * Визуализация на метрики и алармиране
  * Интеграция с различни източници на данни

---

## 💡 Експертиза

```
🏗️ Инфраструктура като код (Terraform, Ansible)
🐳 Контейнеризация и оркестрация (Docker, Kubernetes)
🔄 CI/CD пайплайни (GitHub Actions, GitLab CI/CD, Jenkins)
📊 Мониторинг и алармиране (Prometheus, Grafana)
🔒 Сигурност (Vault, SSL/TLS, съответствие)
🌐 Уеб сървъри и прокси (Nginx)
📜 Скриптове за автоматизация (Bash, Python)
```

---

## 📚 Текущо обучение

Текущо изучавам и усъвършенствам умения в следните области:

* AWS Essential Training
* Ansible Advanced
* GitHub Actions CI/CD
* Kubernetes & Docker
* Bash Scripting Advanced

---

## 📞 Контакти

- **LinkedIn**: [linkedin.com/in/vepaks](https://linkedin.com/in/vepaks)
- **Уебсайт**: [vepaks.dev](https://vepaks.dev)

---

<p align="center">
  <i>всичко е файл</i>
</p>

