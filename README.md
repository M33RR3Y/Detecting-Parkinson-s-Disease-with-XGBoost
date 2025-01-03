# Обнаружение болезни паркинсона с помощью XGBoost

Модель для предсказания ранних стадий болезни Паркинсона предназначена для использования в медицинских исследованиях и клинической практике с целью ранней диагностики заболевания. Это поможет врачам и исследователям своевременно выявлять заболевание и принимать меры для улучшения качества жизни пациентов.
Как работает модель:

1. Обработка данных:
      * Признаки из предоставленного набора данных [UCI ML Parkinsons](https://storage.yandexcloud.net/academy.ai/practica/parkinsons.data)(описание признаков и меток датасета представлены [здесь](https://storage.yandexcloud.net/academy.ai/practica/parkinsons.names)) нормализуются с использованием библиотеки sklearn для приведения их к единому масштабу, что улучшает работу алгоритма.
      * Данные делятся на обучающую (80%) и тестовую (20%) выборки.

2. Классификация:
      * Используется алгоритм XGBoost, известный своей высокой точностью и эффективностью. Он позволяет выявлять сложные зависимости между признаками и метками.

3. Обучение модели:
      * Модель обучается на предоставленном наборе данных, содержащем как признаки пациентов, так и метки, указывающие на наличие или отсутствие болезни Паркинсона.

4. Оценка точности:
      * После обучения модель тестируется на отложенной выборке для оценки точности. Целевой показатель — точность выше 95%, что подтверждает высокую эффективность модели.

Почему это важно:

Ранняя диагностика болезни Паркинсона имеет критическое значение для замедления прогрессирования заболевания. Данная модель может использоваться:

* В медицинских исследованиях для автоматизации диагностики.
* В клинических учреждениях для дополнительной поддержки врачей при постановке диагноза.
* В системах мониторинга здоровья для анализа биометрических данных пациентов.

Основные характеристики проекта:

* Использование передовых технологий, таких как XGBoost, для точной классификации.
* Обработка и нормализация данных с помощью sklearn.
* Высокая точность модели, превышающая 95%, что делает её надежным инструментом для практического применения.
* Пошаговая визуализация работы модели для удобного анализа и интерпретации.
