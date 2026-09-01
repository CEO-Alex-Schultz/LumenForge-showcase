<div align="center">
  <img width="890" height="464" alt="image-Photoroom" src="https://github.com/user-attachments/assets/666fe86f-113d-4031-8988-db2baf864ed1" />

  # LumenForge - студия веб-разработки и дизайна

  ![Status](https://img.shields.io/badge/status-скоро%20запуск-yellow)
  ![Type](https://img.shields.io/badge/type-web%20studio-blue)
  ![License](https://img.shields.io/badge/code-closed%20source-lightgrey)

  🔗 **Сайт доступен на → [lumenforge.website](https://lumenforge.website)**

</div>

---

## О проекте

**LumenForge** - студия, которая занимается веб-разработкой и дизайном: сайты, интерфейсы, брендинг под ключ.

Помимо витрины услуг, на своём же сайте студия обкатывает собственные технологические фишки - например, умную обработку входящих заявок.

## Стек

![PHP](https://img.shields.io/badge/PHP-777BB4?logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?logo=mysql&logoColor=white)
![Apache](https://img.shields.io/badge/Apache-D22128?logo=apache&logoColor=white)
![YandexGPT](https://img.shields.io/badge/YandexGPT-FF0000?logo=yandexcloud&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
</br>
![SCSS](https://img.shields.io/badge/SCSS-CC6699?logo=sass&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)
![Three.js](https://img.shields.io/badge/Three.js-000000?logo=threedotjs&logoColor=white)
![PHPMailer](https://img.shields.io/badge/PHPMailer-6C63FF?logo=maildotru&logoColor=white)
![Docker Compose](https://img.shields.io/badge/Docker%20Compose-2496ED?logo=docker&logoColor=white)
![GSAP](https://img.shields.io/badge/GSAP-88CE02?logo=greensock&logoColor=white)

## Что реализовано

- 🎬 Hero-блок с "бегущей строкой" (marquee-анимация) из фраз "WEB ДИЗАЙН & WEB РАЗРАБОТКА"
- 🌐 3D-элементы на Three.js
- 🖱️ Кастомный скролл и разнообразные анимации на GSAP - от плавного скроллинга страницы до hover-эффектов на карточках
- 🎴 Карточки услуг и тарифных "протоколов" (Product Design, Web App, Web App+, Logo Design) - у каждой свой стек и сроки разработки
- 🗂️ Блок портфолио/кейсов студии с каруселью
- 💬 Плавающий чат-виджет с YandexGPT-ассистентом
- 📱 Полностью адаптивная вёрстка под все экраны
- ⚙️ Полный набор SEO/OG метатегов для соцсетей и поисковиков

## Архитектура и подробная техническая реализация

### 🔌 Интеграции
- **YandexGPT API** - ИИ-ассистент на лету читает входящие заявки и классифицирует их (вопрос / заказ / сотрудничество) ещё до того, как они попадут к менеджеру
- **PHPMailer + Yandex SMTP** - кастомный скрипт защищённой маршрутизации писем через SSL/TLS
- **Yandex SmartCaptcha** - серверная и клиентская валидация от спам-ботов

### 🏗️ Backend
Кастомная CRM на PHP со строгой структурой директорий - бизнес-логика отделена от публичной папки `public`. Зависимости управляются через Composer (изолированный `vendor`).

### 🔒 Безопасность
- Конфиги с доступами к БД и API-ключами вынесены за пределы публичного корня сервера
- Защита от SQL-инъекций
- Авторизация в админке - через безопасное хеширование паролей

### ☁️ DevOps и сервер (VDS/Linux)
- Реальные пути веб-сервера скрыты через symlink-маршрутизацию - например, `/admin` безопасно ссылается на `/feedback-system/public/admin`
- Самостоятельный траблшутинг серверного окружения: установка пакетов-архиваторов, настройка прав доступа

### 🗄️ База данных
- MySQL/MariaDB, структура разворачивается не хаотично, а через файлы миграций (например, `001_init.sql`)
- Выделенные пользователи БД с ограниченными правами

### 🔗 Frontend ↔ Backend
Данные из форм отправляются асинхронно через Fetch API (JS) на выделенные эндпоинты (например, `/api/feedback.php`).

## Админ-панель

Для обработки заявок написана отдельная веб-панель:

- 🗂️ Все заявки из чата стекаются в единую панель - ничего не теряется
- ✅ Модерация - заявки можно посмотреть, обработать, отметить статус
- 📊 Дашборд с графиками - визуальная аналитика по заявкам: сколько пришло, каких типов, динамика по времени

## Скриншоты

<img width="1901" height="924" alt="image" src="https://github.com/user-attachments/assets/1c4255d7-b44f-4d5d-916a-f445a884099b" />
<img width="1914" height="922" alt="image" src="https://github.com/user-attachments/assets/048c9c61-349b-4ce1-8022-0a99d488230a" />
<img width="1877" height="890" alt="image" src="https://github.com/user-attachments/assets/b98131be-ad64-4329-bfe3-345747394d11" />
<img width="1804" height="870" alt="image" src="https://github.com/user-attachments/assets/3b86f169-cbff-4c0b-8ccc-e69867beb4d4" />
<img width="1880" height="881" alt="image" src="https://github.com/user-attachments/assets/5c054da4-4f02-4668-a45b-181023cab1d2" />
<img width="1891" height="760" alt="image" src="https://github.com/user-attachments/assets/f66fff9b-0c6b-4587-b7a7-10773e74469e" />
<img width="1909" height="926" alt="image" src="https://github.com/user-attachments/assets/5d2c3e39-de25-4177-933b-c015ba443bf1" />
<img width="1750" height="776" alt="image" src="https://github.com/user-attachments/assets/120cc059-8614-4cdf-b4ca-12ac70028a50" />
<img width="1502" height="875" alt="image" src="https://github.com/user-attachments/assets/a9fb3068-1b02-4844-9981-d237b770a1fe" />
<img width="1796" height="718" alt="image" src="https://github.com/user-attachments/assets/8d8558b7-bdc7-4af5-b893-c8005eb45f2c" />
<img width="1873" height="921" alt="image" src="https://github.com/user-attachments/assets/6ad1a366-6880-492e-8bd4-4c34aee85098" />
<img width="1074" height="725" alt="image" src="https://github.com/user-attachments/assets/3d99ad70-c807-43a6-86df-1e477c96a0a7" />
<img width="1900" height="932" alt="image" src="https://github.com/user-attachments/assets/81c6fe3d-5fba-43b7-a767-bd851a2c49b0" />
<img width="1907" height="937" alt="image" src="https://github.com/user-attachments/assets/522edce3-febf-45c4-8f91-d973bda66b9c" />




## Контакты

📧 lumenforge@yandex.ru
