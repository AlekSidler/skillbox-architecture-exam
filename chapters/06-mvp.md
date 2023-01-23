[Heading](../heading.md)

[Previous chapter](05-risks.md)

[Next chapter](07-critical-processes.md)

# План поэтапной разработки и расширения системы, анализ критически важных компонентов

Для начала нам нужно реализовать MVP (Minimal Viable Product). Разобьём наш проект на домены:
* Core
    1. Возможность интеграции с фитнес устройствами
    1. Функционал ССС.
* Generic:
    1. Механизм аутентификации
    1. Хранение и защита данных
* Support:
    1. Компоновка и отображение данных


К MVP я бы отнёс компоненты ССС со следующим функционалом:
* Обработка данных фитнес трекера и сохранение их в базу
* Аутентификаця
* Обработка трафика приложения/web версии (лучше сосредоточиться на чём-то одном, особенно в отсутствии необходимых людей, например приложение)
* Бизнес логику (основной функционал ССС)
* База данных социальной сети
* База данных фитнес трекеров


Также необходимо разработать в MVP API для работы с фитнес устройствами. В MVP это будет альфа версия, которая может в будущем измениться, но в дальнейшем её нужно будет зафиксировать, и потом, в случае изменений, увиличить номер версии.

Для MVP достаточно, чтобы все компоненты были в одном единственном экземпляре, можно даже "захардкодить" адреса используемых компонент, возможно также сделать это всё модульным монолитом. MVP можно выложить в сеть и дать на тестирование заинтересованным пользователям.


В дальнейшем нужно расширять как и функционал ССС, так и инфраструктуру проекта. Нужно обязательно добавить как средства мониторинга приложений (метрики, триггеры, обработка логов), так и API Gateway. Для ускорения разработки необходимо договориться о соглашениях между компонентами, чтоб ускорить разработку. Желательно делать компоненты независимыми друг от друга.

Для самостоятельной разработки инфраструктурного функционала необходимо много DevOps специалистов, но исходя из описания, у нас их нет, поэтому можно либо отдать инфраструктурную часть проекта на outsourcing или же воспользоваться готовым PaaS решением.

В таком случае мы сможем сократить время разработки и сконцентрироваться на бизнес логике нашего проекта.