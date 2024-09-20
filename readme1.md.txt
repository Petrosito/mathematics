# Лабораторная работа 1. Web как источник данных

## Исполнитель
ФИО: [Ованнисян Петрос Абгарович]  
Группа: [СГН3-44Б]  

## Описание API
Для выполнения лабораторной работы были выбраны следующие публичные API:

1. [Python Programming](https://petrosito.github.io/python_programming/index.html)
2. [Web Programming](https://petrosito.github.io/web_programming/index.html)
3. [Mathematics](https://petrosito.github.io/mathematics/index.html)
4. [Informatics](https://petrosito.github.io/informatics/index.html)
5. [Russian](https://petrosito.github.io/russian/index.html)

### Методы вызова API
Было выполнено два метода API:
- Получение данных из веб-страниц по указанным URL-адресам.
- Сохранение собранных данных в базе данных.

## Описание ресурсов для парсинга
В рамках лабораторной работы были использованы следующие веб-страницы для парсинга данных:

1. [Web Programming](https://petrosito.github.io/web_programming/index.html)
2. [Python Programming](https://petrosito.github.io/python_programming/index.html)

## Коллекции в базе данных
База данных "Lab1" содержит следующие коллекции:
- `python_programming` - Данные из веб-ресурса по программированию на Python.
- `web_programming` - Данные из веб-ресурса по веб-программированию.
- `mathematics_index` - Данные из веб-ресурса по математике.
- `informatics_index` - Данные из веб-ресурса по информатике.
- `russian_index` - Данные из веб-ресурса по русскому языку.

## Алгоритм работы кода
1. Код запускает функцию `scrape_and_store_data`, которая проходит по списку URL-адресов.
2. Для каждого URL выполняется HTTP-запрос, после чего контент страницы парсится с использованием библиотеки BeautifulSoup.
3. Заголовок страницы и параграфы нормализуются и сохраняются в соответствующие коллекции MongoDB для дальнейшего использования.
