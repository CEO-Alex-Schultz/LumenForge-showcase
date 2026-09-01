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

<img width="1906" height="938" alt="image" src="https://github.com/user-attachments/assets/f274b8b4-511e-4b12-bb91-9a40ad4821f5" />
<img width="1910" height="932" alt="image" src="https://github.com/user-attachments/assets/015843a0-bc6a-4006-b201-7128bc36e91c" />
<img width="1914" height="916" alt="image" src="https://github.com/user-attachments/assets/90571578-d9ed-4352-993f-a95a285ad96f" />
<img width="1722" height="796" alt="image" src="https://github.com/user-attachments/assets/309ba1c6-ff2f-49a1-9d1f-0ea1302f8183" />
<img width="1919" height="916" alt="image" src="https://github.com/user-attachments/assets/7ce7dda0-31d2-43c8-9bc4-beacc23677c3" />
<img width="1883" height="909" alt="image" src="https://github.com/user-attachments/assets/45da2799-942e-4c3c-8c80-fa3829e48369" />
<img width="1875" height="595" alt="image" src="https://github.com/user-attachments/assets/3f4ab295-3006-4c63-b673-13086632b14d" />
<img width="1809" height="849" alt="image" src="https://github.com/user-attachments/assets/d34062e6-ef5a-45fe-a296-f758f5fecc02" />
<img width="1728" height="858" alt="image" src="https://github.com/user-attachments/assets/4f70a87d-e881-4f74-bfb4-3176932ee060" />
<img width="1703" height="918" alt="image" src="https://github.com/user-attachments/assets/8c67c274-033c-4054-a868-ed195be22463" />
<img width="1701" height="915" alt="image" src="https://github.com/user-attachments/assets/18181fbd-b3c7-4781-b9d7-9594c227f678" />
<img width="1528" height="887" alt="image" src="https://github.com/user-attachments/assets/219d4e53-d6f2-442e-bdc4-348dbd0f2b06" />
<img width="1831" height="910" alt="image" src="https://github.com/user-attachments/assets/dbbfa122-267b-4998-b093-d83a501cac5a" />
<img width="1751" height="702" alt="image" src="https://github.com/user-attachments/assets/8a17e3b6-881d-4c88-9284-2b71bd23241d" />
<img width="676" height="668" alt="image" src="https://github.com/user-attachments/assets/b6b5915b-0d2c-40a0-b1c4-e03700053729" />
<img width="1881" height="930" alt="image" src="https://github.com/user-attachments/assets/3fe2217a-13f3-498f-8b8f-1563a03f72ce" />

## Контакты

📧 lumenforge@yandex.ru
