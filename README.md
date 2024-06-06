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

[Решение.](https://github.com/ShevEvgeniy/Data_collection_and_markup_2024/blob/main/Seminar_3/Lesson.ipynb)

4. Зарегистрируйтесь в ClickHouse.
5. Загрузите данные в ClickHouse и создайте таблицу для их хранения.


### Домашняя работа к уроку № 4:
#### Парсинг HTML. XPath

Выберите веб-сайт с табличными данными, который вас интересует.

Напишите код Python, использующий библиотеку requests для отправки HTTP GET-запроса на сайт и получения HTML-содержимого страницы.

Выполните парсинг содержимого HTML с помощью библиотеки lxml, чтобы извлечь данные из таблицы.

Сохраните извлеченные данные в CSV-файл с помощью модуля csv.

Ваш код должен включать следующее:

Строку агента пользователя в заголовке HTTP-запроса, чтобы имитировать веб-браузер и избежать блокировки сервером.
Выражения XPath для выбора элементов данных таблицы и извлечения их содержимого.
Обработка ошибок для случаев, когда данные не имеют ожидаемого формата.
Комментарии для объяснения цели и логики кода.


### Домашняя работа к уроку № 5
#### Урок 5. Scrapy

Найдите сайт, содержащий интересующий вас список или каталог. Это может быть список книг, фильмов, спортивных команд или что-то еще, что вас заинтересовало.

Создайте новый проект Scrapy и определите нового паука. С помощью атрибута start_urls укажите URL выбранной вами веб-страницы.

Определите метод парсинга для извлечения интересующих вас данных. Используйте селекторы XPath или CSS для навигации по HTML и извлечения данных. Возможно, потребуется извлечь данные с нескольких страниц или перейти по ссылкам на другие страницы.

Сохраните извлеченные данные в структурированном формате. Вы можете использовать оператор yield для возврата данных из паука, которые Scrapy может записать в файл в выбранном вами формате (например, JSON или CSV).

Конечным результатом работы должен быть код Scrapy Spider, а также пример выходных данных. Не забывайте соблюдать правила robots.txt и условия обслуживания веб-сайта, а также ответственно подходите к использованию веб-скрейпинга.

Обработка ошибок для случаев, когда данные не имеют ожидаемого формата.

Комментарии для объяснения цели и логики кода.

Примечание: Пожалуйста, не забывайте соблюдать этические и юридические нормы при веб-скреппинге.


### Домашняя работа к уроку № 6
#### Урок 6. Scrapy. Парсинг фото и файлов

1. Создайте новый проект Scrapy. Дайте ему подходящее имя и убедитесь, что ваше окружение правильно настроено для работы с проектом.
2. Создайте нового паука, способного перемещаться по сайту www.unsplash.com. Ваш паук должен уметь перемещаться по категориям фотографий и получать доступ к страницам отдельных фотографий.
3. Определите элемент (Item) в Scrapy, который будет представлять изображение. Ваш элемент должен включать такие детали, как URL изображения, название изображения и категорию, к которой оно принадлежит.
4. Используйте Scrapy ImagesPipeline для загрузки изображений. Обязательно установите параметр IMAGES_STORE в файле settings.py. Убедитесь, что ваш паук правильно выдает элементы изображений, которые может обработать ImagesPipeline.
5. Сохраните дополнительные сведения об изображениях (название, категория) в CSV-файле. Каждая строка должна соответствовать одному изображению и содержать URL изображения, локальный путь к файлу (после загрузки), название и категорию.
