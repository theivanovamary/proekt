# Проект в рамках "Сириус ИИ". Инструмент для анализа клиентских отзывов.

Команда разработки: 

- :white_check_mark: [Kravtsova Helen (в роли Python-разработчика)](https://github.com/lenakravt)
- :white_check_mark: [Ivanova Maria (в роли Python-разработчика)](https://github.com/theivanovamary)

## Описание проекта:
Проект содержит отзывы с сайта 

Файл parser.ru парсит отзывы клиентов https://www.banki.ru/services/responses/list/. При этом использованы стандартные библиотеки requests и BeautifulSoup.

Файл  содержит анализ отзывов клиентов, а также классификацию отзывов на основе оценки поставленной клиентом (негативная, позитивная).

Производится предварительная обработка текста посредством nltk (stop-слова, пунктуация, разбиение на токены) и лемматизация посредством pymorphy2

С помощью word2vec создается 1000 мерный вектор и производится вычисление значений токенов.

Далее для получения предсказания мы вычисляем среднее значение по всем векторам токенов в предложении
Обучение классификатора настроений клиентов производится в качестве примера с помощью DecisionTreeClassifier и Xgboost. Accuracy 75% на мой взгляд неплохо.
В последующем будет реализована модель на Pytorch
## Инструкция по установке:

## Надеемся Вам понравится наш проект!)
![Logo](https://static.theceomagazine.net/wp-content/uploads/2018/09/18094615/2018.08.13_AndrewCannington_AI-revolution-gender-biased_subbed.jpg)