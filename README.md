# Задание на 17.10 по системному программированию: Развертывание окружения в WSL

**Выполнил:** Травкин М. Г.
**Пользователь Linux:** travkin-m-g

## 1. Установка WSL и Ubuntu

Установлены компоненты WSL и платформа виртуальной машины.
![Установка WSL](screenshotsWSL/01-wsl-start.png)
![Успешная установка WSL](screenshotsWSL/02-wsl-success.png)

Выполнено переключение на вторую версию WSL.
![Версия WSL](screenshotsWSL/03-wsl-version.png)

Дистрибутив Ubuntu 24.04 импортирован на диск D.
![Импорт Ubuntu](screenshotsWSL/04-wsl-import.png)

Стартовое окно документации WSL после установки.
![Приветствие WSL](screenshotsWSL/05-wsl-welcome.png)

Первый запуск системы под пользователем `root`.
![Первый запуск](screenshotsWSL/06-wsl-first-boot.png)

## 2. Настройка пользователя

Создан пользователь `travkin-m-g` и ему выданы права администратора.
![Выдача прав sudo](screenshotsWSL/07-sudo-rights.png)

Настроен файл `wsl.conf` для автоматического входа под пользователем `travkin-m-g`.
![Вход под пользователем](screenshotsWSL/08-user-login.png)

Проверка работы `sudo` и обновление списков пакетов системы.
![Обновление системы](screenshotsWSL/09-apt-update.png)
![Завершение обновления](screenshotsWSL/10-update-done.png)

## 3. Установка компилятора (SDK)

Установлен пакет `build-essential` (компиляторы GCC, G++).
![Установка компилятора](screenshotsWSL/11-gcc-install.png)
![Завершение установки](screenshotsWSL/12-gcc-done.png)

Проверка версии компилятора.
![Версия GCC](screenshotsWSL/13-gcc-version.png)

## 4. Установка PostgreSQL

Установлен сервер базы данных PostgreSQL и дополнительные утилиты.
![Установка PostgreSQL](screenshotsWSL/14-pg-install.png)
![Завершение установки](screenshotsWSL/15-pg-done.png)

Проверка версии установленного клиента.
![Версия PostgreSQL](screenshotsWSL/16-pg-version.png)

Запуск службы и проверка её статуса.
![Статус службы](screenshotsWSL/17-pg-status.png)

## 5. Создание базы данных

Вход в консоль PostgreSQL под системным пользователем.
![Вход в консоль](screenshotsWSL/18-pg-login.png)

Создание тестовой базы данных `testdb`.
![Создание БД](screenshotsWSL/19-pg-createdb.png)

Попытка подключения по TCP-протоколу выявила отсутствие пароля.
![Ошибка пароля](screenshotsWSL/20-pg-error.png)

Установка пароля для пользователя `postgres`.
![Установка пароля](screenshotsWSL/21-pg-password.png)

Финальная проверка: успешное подключение к базе данных и вывод версии СУБД.
![Успешное подключение](screenshotsWSL/22-pg-success.png)
