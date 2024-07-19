# CV_Bot
AI bot/ AI assistant that browses HR channels in Telegram and evaluates vacancies according to specified criteria

# Job Search Assistant / Ассистент по Поиску Работы
This project is an AI job search assistant that analyzes messages from various Telegram channels and job websites, filters them based on specified parameters, and notifies the user about relevant job vacancies via Telegram.
Этот проект представляет собой ИИ ассистента по поиску работы, который анализирует сообщения из различных Telegram каналов и сайтов вакансий, проводит их анализ по заданным параметрам и уведомляет пользователя о подходящих вакансиях через Telegram.

## Table of Contents / Оглавление
- [Description / Описание](#description--описание)
- [Features / Функциональность](#features--функциональность)
- [Installation / Установка](#installation--установка)
- [Usage / Использование](#usage--использование)
- [Configuration / Настройка](#configuration--настройка)
- [Contributing / Вклад](#contributing--вклад)
- [License / Лицензия](#license--лицензия)
## Description / Описание
The AI job search assistant is designed to automate the job search process. It collects data from specified Telegram channels and job websites, analyzes it based on specified parameters, and notifies the user about relevant job vacancies via Telegram.

ИИ ассистент по поиску работы предназначен для автоматизации процесса поиска вакансий. Он собирает данные из заданных Telegram каналов и сайтов вакансий, анализирует их по заданным параметрам и уведомляет пользователя о подходящих вакансиях через Telegram.

## Features / Функциональность

- **Data Collection from Telegram Channels and Websites**: Connects to the Telegram API and parses messages, collects data from job websites.
- **Job Analysis**: Filters and evaluates the relevance of job vacancies based on specified parameters.
- **User Notification**: Sends messages to the user with links to interesting job vacancies.
- **Telegram Management Interface**: Handles user commands and configures search parameters.

- **Сбор данных из Telegram каналов и сайтов**: Подключение к Telegram API и парсинг сообщений, сбор данных с сайтов вакансий.
- **Анализ вакансий**: Фильтрация и оценка релевантности вакансий по заданным параметрам.
- **Уведомление пользователя**: Отправка сообщений пользователю с ссылками на интересные вакансии.
- **Интерфейс управления в Telegram**: Обработка команд от пользователя и настройка параметров поиска.

## Installation / Установка

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/job-search-assistant.git
    cd job-search-assistant
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Configure environment variables in the `.env` file:
    ```plaintext
    TELEGRAM_BOT_API_KEY=your_telegram_bot_api_key
    DATABASE_URL=your_database_url
    ```

1. Клонируйте репозиторий:
    ```bash
    git clone https://github.com/yourusername/job-search-assistant.git
    cd job-search-assistant
    ```

2. Установите зависимости:
    ```bash
    pip install -r requirements.txt
    ```

3. Настройте переменные окружения в файле `.env`:
    ```plaintext
    TELEGRAM_BOT_API_KEY=your_telegram_bot_api_key
    DATABASE_URL=your_database_url
    ```

## Usage / Использование

1. Run the data collection from Telegram channels and websites:
    ```bash
    python collect_data.py
    ```

2. Run the data analysis process:
    ```bash
    python analyze_data.py
    ```

3. Run the Telegram bot for management and notifications:
    ```bash
    python bot.py
    ```

1. Запустите сбор данных из Telegram каналов и сайтов:
    ```bash
    python collect_data.py
    ```

2. Запустите процесс анализа данных:
    ```bash
    python analyze_data.py
    ```

3. Запустите Telegram бота для управления и уведомлений:
    ```bash
    python bot.py
    ```

## Configuration / Настройка

### Data Collection from Telegram Channels / Сбор данных из Telegram каналов

The `collect_data_from_telegram_channels` function connects to the Telegram API and parses messages from specified channels. Messages are sent to the message broker for further processing.

Функция `collect_data_from_telegram_channels` подключается к Telegram API и парсит сообщения из заданных каналов. Сообщения отправляются в брокер сообщений для дальнейшей обработки.

### Data Collection from Job Websites / Сбор данных с сайтов вакансий

The `collect_data_from_websites` function parses data from job websites and sends it to the message broker.

Функция `collect_data_from_websites` парсит данные с сайтов вакансий и отправляет их в брокер сообщений.

### Job Analysis / Анализ вакансий

The `analyze_vacancies` function filters and evaluates the relevance of job vacancies based on specified parameters. The analysis results are stored in the database.

Функция `analyze_vacancies` фильтрует и оценивает релевантность вакансий по заданным параметрам. Результаты анализа сохраняются в базе данных.

### User Notification / Уведомление пользователя

The `notify_user` function sends messages to the user in Telegram with links to relevant job vacancies.

Функция `notify_user` отправляет сообщения пользователю в Telegram с ссылками на подходящие вакансии.

### Telegram Management Interface / Интерфейс управления в Telegram

The `handle_commands` function handles user commands such as `/start`, `/help`, and `/settings`.

Функция `handle_commands` обрабатывает команды от пользователя, такие как `/start`, `/help`, и `/settings`.

## Contributing / Вклад

We welcome contributions to the project! Please fork the repository, make your changes, and submit a pull request. You can also open an issue to discuss new ideas and improvements.

Мы приветствуем вклад в развитие проекта! Пожалуйста, создайте форк репозитория, внесите изменения и отправьте pull request. Также вы можете открыть issue для обсуждения новых идей и улучшений.

## License / Лицензия

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

Этот проект лицензирован под лицензией MIT. Подробности см. в файле [LICENSE](LICENSE).
