# Выбор и настройка оркестратора

## Статус

Accepted

## Контекст

Для автоматизации деплоя, управления запущенными контейнерами и машинами используются оркестраторы. Есть несколько вариантов внедрения оркестратора в нашу систему

Опции:
1. Использование PaaS
1. Разработка и настройка на основе open-source решений
1. Отдать эту часть на outsourcing (DaaS)

У каждого варианта есть свои преимущества и недостатки

Так как у нас отсутствуют необходимые специалисты (DevOps) для поддержания и настройки оркестратора, нам вариант с самостоятельной настройкой не очень подходит.
Недостатком PaaS является отсутствие гибкости и привязка к определённому облачному решению, чего мы тоже хотели бы избежать.

Самым подходящим для нас вариантом является передача этой части проекта на outsourcing. 

В нашем случае стоит воспользоваться оркестратором kubernetes так как это активно развивающийся с большим сообществом.

## Решение

Используем kubernetes в качестве оркестратора и передаём его на outsourcing так как этот вариант является самым гибким и не требуется нанимать новый персонал.

## Последствия

* Быстрый старт
* Возможен перехват разработки/настройки в будущем