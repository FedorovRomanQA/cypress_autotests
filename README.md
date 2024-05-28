<h2>UI Автотесты на фреймворке Cypress</h2>

> **Статус проекта:**
> Публичный проект: https://login.qa.studio/
> 
> 🟢 Поддерживается (активный) 

## Описание проекта и задачи
Автоматизировать часть проверок регресса с помощью Cypress

## Тест-кейсы, которые автоматизировали
* Авторизация с верным паролем и верным логином
* Авторизация c верным логином и неверным паролем
* Проверка работы валиадации на наличие @ в логине
* Проверка флоу восстановления пароля

## Детали реализации

1. baseUrl вынесен в переменные конфига
![image](https://raw.githubusercontent.com/FedorovRomanQA/cypress_autotests/main/1.png)

2. Применение хуков beforeEach и afterEach
![image](https://raw.githubusercontent.com/FedorovRomanQA/cypress_autotests/main/2.png)

3. Переменные данные для авторизации вынесены в отдельный файл
![image](https://raw.githubusercontent.com/FedorovRomanQA/cypress_autotests/main/3.png)

4. Каждая страница описана в формате объекта с локаторами
![image](https://raw.githubusercontent.com/FedorovRomanQA/cypress_autotests/main/4.png)

## Локальный запуск тестов (из терминала)
1. Скачать проект
2. Перейти в терминале в директорию проекта
2. Выполнить команду:
```
npx cypress run --spec cypress/e2e/lesson_locators.cy.js --browser chrome
```
Ожидаемый результат: получим отчет о прохождении тестов.
![image](https://raw.githubusercontent.com/FedorovRomanQA/cypress_autotests/main/5.png)




## Автор

Федоров Роман ([@snape777](https://t.me/snape777))
