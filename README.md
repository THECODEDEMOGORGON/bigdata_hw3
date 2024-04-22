# bigdata_hw3

Ссылка на видео доклада: https://drive.google.com/file/d/1_kDxJDtbWiXdjfBptw43pH2WTS32STdl/view?usp=sharing

Ссылка на презентацию: https://docs.google.com/presentation/d/1lGEUj-0YdjDOXjHoypmCOYr1fI4uJJxcPxMqAxuhBwI/edit?usp=sharing

# Краткое сравнение Kappa и Lambda архитектур

**1. Как устроены Kappa и Lambda архитектуры**

Kappa и Lambda - это две распространенные архитектуры для обработки данных в реальном времени. Архитектура Lambda, разработанная AWS, ориентирована на масштабируемость и обработку больших объемов данных. Архитектура Kappa, разработанная Twitter, ориентирована на высокую производительность и низкую задержку.

**2. Ключевые особенности двух этих архитектур**

* **Lambda**: масштабируема, может обрабатывать большие объемы данных, но не оптимизирована для низкой задержки; поддерживает несколько pipeline (батч, поток); может обрабатывать события, но не оптимизирована для них.
* **Kappa**: оптимизирована для обработки событийных потоков данных, имеет низкую задержку и высокую производительность; масштабируема, но не настолько как Lambda; предназначена для потоковых источников данных.

**3. Сравнение архитектур и их различия**

В таблице ниже сравниваются Kappa и Lambda архитектуры:

| Характеристика | Архитектура Lambda | Архитектура Kappa |
| --- | --- | --- |
| Масштабируемость | Горизонтально масштабируема | Горизонтально масштабируема |
| Обработка в реальном времени | Не оптимизирована для низкой задержки | Оптимизирована для низкой задержки |
| Хранение данных | Flexible слой хранения данных | Потоковая система хранения данных |
| Pipelines обраб-ки данных | Поддерживает несколько pipeline | Проведена для одного pipeline |

**4. Указатели на то, когда стоит использовать Lambda архитектуру**

* Для обработки больших объемов данных
* Для масштабируемости и высокой производительности
* Когда нужна гибкость в хранении данных

**5. Указатели на то, когда стоит использовать Kappa архитектуру**

* Для высокопроизводительных приложений с низкой задержкой
* Для обработки событийных потоков данных
* Когда необходима высокая производительность и низкая задержка

**6. Как выбрать архитектуру - алгоритм**

1. Записать остальные требования (возможно есть инфраструктурные ограничения, доступные БД и т.д.)
2. Определить требования (требования к масштабируемости, допустимая задержка и т. д. )
3. Оценить характеристик входных данных (объем, event–driven или batch-oriented)
4. Оценить количество пайплайнов проепроцессинга (сколько их, real-time или batch)
5. Оценить насколько подходит Lambda и Kappa

**7. Итоги и заключение**

Kappa и Lambda - это две важные архитектуры для обработки данных в реальном времени. Каждая имеет свои сильные стороны и слабые стороны. Вам нужно выбрать ту, которая лучше подходит для вашего проекта, учитывая его требования и особенности.
