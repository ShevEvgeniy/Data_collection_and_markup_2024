## Урок 1. Основы клиент-серверного взаимодействия. Парсинг API

1. Ознакомиться с некоторые интересными API. https://docs.ozon.ru/api/seller/ https://developers.google.com/youtube/v3/getting-started https://spoonacular.com/food-api

[Решение задачи 1 для Озон (скриншот)](https://github.com/ShevEvgeniy/Data_collection_and_markup_2024/blob/main/Seminar_1/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%20Ozon.png)

[Решение задачи 1 для YouTube (скриншот)](https://github.com/ShevEvgeniy/Data_collection_and_markup_2024/blob/main/Seminar_1/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%20YouTube.png)

[Решение задачи 1 для Spoonacular (скриншот)](https://github.com/ShevEvgeniy/Data_collection_and_markup_2024/blob/main/Seminar_1/%D0%A1%D0%BA%D1%80%D0%B8%D0%BD%20Spoonacular.png)

2. Потренируйтесь делать запросы к API. Выберите публичный API, который вас интересует, и потренируйтесь делать API-запросы с помощью Postman. Поэкспериментируйте с различными типами запросов и попробуйте получить различные типы данных.

[Решение задачи 2 - запрос по client id через API сервиса Open Library](https://github.com/ShevEvgeniy/Data_collection_and_markup_2024/blob/main/Seminar_1/Client%20id.png)

[Решение задачи 2 - запрос по client ID и городу через API сервиса Open Library](https://github.com/ShevEvgeniy/Data_collection_and_markup_2024/blob/main/Seminar_1/Client_id%26city.png)

3. Сценарий Foursquare
4. Напишите сценарий на языке Python, который предложит пользователю ввести интересующую его категорию (например, кофейни, музеи, парки и т.д.).
5. Используйте API Foursquare для поиска заведений в указанной категории.
6. Получите название заведения, его адрес и рейтинг для каждого из них.
7. Скрипт должен вывести название и адрес и рейтинг каждого заведения в консоль.

[Решение задач 3 - 7](https://github.com/ShevEvgeniy/Data_collection_and_markup_2024/blob/main/Seminar_1/Lesson.ipynb)


## Урок 2. Парсинг HTML. BeautifulSoup
Выполнить скрейпинг данных в веб-сайта http://books.toscrape.com/ и извлечь информацию о всех книгах на сайте во всех категориях: название, цену, количество товара в наличии (In stock (19 available)) в формате integer, описание.

[Решение задачи 1 - код в файле .ipynb](https://github.com/ShevEvgeniy/Data_collection_and_markup_2024/blob/main/Seminar_2/Lesson.ipynb)

Затем сохранить эту информацию в JSON-файле.
[Решение задачи 2 - ссылка на JSON-файл](https://github.com/ShevEvgeniy/Data_collection_and_markup_2024/blob/main/Seminar_2/books_from_books.toscrape.com.json)

### Домашняя работа к уроку № 3:
### Системы управления базами данных MongoDB и Кликхаус в Python

1. Установите MongoDB на локальной машине, а также зарегистрируйтесь в онлайн-сервисе. https://www.mongodb.com/ https://www.mongodb.com/products/compass
2. Загрузите данные который вы получили на предыдущем уроке путем скрейпинга сайта с помощью Buautiful Soup в MongoDB и создайте базу данных и коллекции для их хранения.
3. Поэкспериментируйте с различными методами запросов.
4. Зарегистрируйтесь в ClickHouse.
5. Загрузите данные в ClickHouse и создайте таблицу для их хранения.