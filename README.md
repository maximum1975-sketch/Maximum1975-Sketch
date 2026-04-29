# 👋 Привет! Я Максим Горячев

<p align="left">
  <img src="https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54" alt="Python">
  <img src="https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi" alt="FastAPI">
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain" alt="LangChain">
  <img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white" alt="OpenAI">
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv" alt="OpenCV">
  <img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white" alt="PyTorch">
  <img src="https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white" alt="TensorFlow">
  <br>
  <img src="https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas">
  <img src="https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy">
  <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux">
  <img src="https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="Windows">
  <img src="https://img.shields.io/badge/macOS-000000?style=for-the-badge&logo=apple&logoColor=white" alt="macOS">
</p>

Я **Full-Stack AI / ML Engineer** и **Vibe Coder** нового поколения.

У меня фундаментальное техническое образование (МГТУ им. Баумана) и более 20 лет опыта управления бизнес-процессами и IT-инфраструктурой. Я перешел в машинное обучение, потому что люблю создавать сложные продукты с нуля до выхода в продакшн своими руками. Объединяю глубокое понимание бизнеса (PnL, риск-менеджмент, системный анализ) с современными технологиями.

Я выступаю в роли Архитектора: проектирую логику, алгоритмы, структуры данных и бизнес-требования, активно используя AI-помощников для кратного ускорения написания production-кода. Это позволяет мне двигаться от идеи до готового продукта за считанные дни.

🛠 **Что я умею:**
* **Machine Learning & AI:** RAG-архитектуры, LLM, LangChain, Computer Vision (YOLO, SAM-2), Time Series Analysis (XGBoost, CatBoost, LSTM), Big Data и Feature Engineering.
* **Engineering:** Python, FastAPI, Uvicorn, SQL, FAISS, Git.
* **Production:** Создание Telegram-ботов (Aiogram), веб-интерфейсов (Streamlit), интеграция API, асинхронные высоконагруженные серверы (HFT).
* **ИИ-агенты:** HR, Аналитика, Юристы, Поддержка для организаций и индивидуальные ИИ-помощники **"под заказ"** для боссов и сотрудников.

---

## 💼 Ключевые проекты полного цикла (End-to-End, built single-handedly)

### ⚖️[Нейроюрист по ФЗ-229 "Об исполнительном производстве"](https://github.com/goryachev-ml/neurojurist-fz229-bot)
Полноценный AI-ассистент с **голосовым вводом (Whisper)** для юридических консультаций — RAG-система в виде Telegram-бота с многошаговым пайплайном, включая **LLM-as-judge**, исключающим галлюцинации LLM.
* **Архитектура:** LangChain + FAISS + Qwen3 (Local LLM) + Async Telegram Bot (имеется рабочий вариант для изолированного контура без выхода в интернет).
* **Фишка:** Нулевой уровень галлюцинаций за счет 3-шагового пайплайна (Анализ → Генерация → Валидатор) и структурного парсинга федерального закона.

### 📈 NeuroTrader (ML HFT System)
Система прогнозирования движения цены кросс-курса на основе временных рядов и геометрии Фибоначчи.
* Обработка датасета за 25 лет (парсинг и агрегация M1 → H1/D1).
* **Инженерия:** Event-Based Structural Labeling и кастомный парсер на базе алгоритма `Sparse Tables (RMQ)` для молниеносного поиска локальных экстремумов (алгоритм "матрешки").
* **Деплой:** Асинхронный FastAPI-сервер для связи с MetaTrader 4 в реальном времени.

### 🐔[AgroTech CV Tracker](https://github.com/goryachev-ml/neurojurist-fz229-bot)
End-to-end Computer Vision пайплайн для трекинга объектов (подсчет цыплят на птицефабрике) с 99% точностью и отсевом аномалий.
* **Стек:** YOLO + SAM-2 + OpenCV + Streamlit/Gradio. 
* **Обработка и аугментация:** Подготовка, авторазметка и корректировка датасета (LabelStudio, RoboFlow, VGG)
* **ML:** обучение, тесты метрик и инференс yolo8n-11x - seg.
* **Инженерия:** вложенные эллиптические зоны трекинга, HSV-сегментация, морфология, контуры. Оптимизация параметров ByteTrack.
* Реализована математическая логика фильтрации "фантомных" треков и интерфейс для конечного пользователя. 

### 💱 Crypto Arbitrage Bot
Высокочастотный бот на PHP для межбиржевого арбитража. Асинхронный опрос стаканов, учет комиссий и управление ликвидностью. Бот работал с плюсовым PnL на реальных средствах.

---

🚀 **Что я могу:** воплотить любой проект автоматизации на любой известной платформе (Windows, Linux, macOS), в том числе для изолированных систем без доступа в интернет **(!)**, будь то корпоративный сервер или ноутбук руководителя в локальной сети предприятия.

---

## 🧬 Инженерная ДНК (Language-Agnostic Engineer)
Мой подход к инженерии формировался десятилетиями и не зависит от модных фреймворков. Благодаря современным AI-помощникам (Vibecoding) я окончательно стер границу между языками программирования. Написал клиент-серверное Android-приложение (v8+) за 1 день (фотогалерея на удаленном компьютере), хотя до этого никогда не брался за подобные задачи. 

Я решаю инженерные задачи даже «без документации», потому что делал это еще до появления интернета в каждом доме:
* **1998 (Робототехника и космос):** В рамках диплома МГТУ им. Баумана сделал реверс-инжиниринг аппаратных протоколов промышленного робота KUKA. Расшифровал сигналы ручного пульта и перевел управление на ПК (i386) через RS-232, написав алгоритмы имитации автоматической стыковки космических аппаратов.
* **2000-е (IoT & Monitoring):** Разработал на Perl систему централизованного мониторинга 20+ промышленных источников бесперебойного питания на электроподстанциях Северного Кавказа. 

Для меня не существует незнакомого стека. Есть только бизнес-задача, архитектура и оптимальный алгоритм её решения.

---

📫 **Как со мной связаться:**
* Telegram: [@okey_people](https://t.me/okey_people) (предпочтительный способ связи)
* Email:[ai@goryachev.ru](mailto:ai@goryachev.ru)
* Телефон: +7 (925) 781-94-22
* Локация: Москва. Готов к командировкам.
* Открыт к позициям **ML Engineer / AI Researcher & Developer** или проектным работам с нуля до продакшена.
