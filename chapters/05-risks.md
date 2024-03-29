[Heading](../heading.md)

[Previous chapter](04-conceptual-architecture.md)

[Next chapter](06-mvp.md)

# Описание рисков реализации

Возможные риски:

Бизнес риски:
* Нехватка бюджета:
  Основной риск, по которому нужно планировать нашу архитектуру и план разработки. В нашем случае не является риском так как у нас бюджет неограничен, но в реальных проектах такого не бывает
* Риск того, что приложение "не взлетит":
  При наличии похожих приложений конкурентов с аналогичным функционалом ([1](https://www.sportifico.com/), [2](https://www.strava.com/), [3](https://sportening.com/)) есть шанс, что приложение не будет популярным. Нам нужно, чтобы приложение чем-то отличалось от уже существующих и было лучше. Неграмотно настроенный интерфейс также уменьшает вероятность того, что приложение будет пользоваться спросом
* Отсутствие бизнес плана:
  Важно чёткое понимание и согласование того как приложение будет развиваться, какие будут шаги развития, как и когда приложение начнёт приносить прибыль
* Неверно выбранная целевая аудитория:
  Прежде всего у приложения должна быть целевая аудитория, которая будет заинтересована в продукте. Если мы не сможем привлечь целевую аудиторию, то нечего говорить о привлечении новых клиентов

Технические риски:
* Неверно выбранные технологии:
  Технологии,которые безнадёжно устаревают. На такие технологии сложнее найти людей и их сложнее будет со временем поддерживать, нужно будет переписывать
  Также любые технологии могут устареть. Нужно быть к этому готовым и иметь возможность заменить на аналоги.
* Неверно выбранная архитектура:
  Может повлечь за собой много усилий со стороны поддержки или же невозможность получить желаемый результат.
* Инфраструктурные проблемы:
  Инфраструктура имеет крайне важное значение в сервис-ориентированной архитектуре и её неправильная настройка может иметь такие же последствия, как и неверно выбранная архитектура
* Привязка к одному облачному провайдеру:
  В случае использования облачного провайдера, нужно иметь возможность абстрагироваться от API конкретного облачного провайдера, чтобы в будущем иметь возможность выбирать более подходящие решения, в том числе и свои сервера
* Сетевые проблемы:
  В сервис-ориентированной архитектуре большая нагрузка ложится на сеть. Нужно помнить про это при разработке и учитывать пропускную способность и задержки сети


Другие риски:
* Отсутствие людей нужной специальности:
  Для сервис-ориентированной архитектуры важен не только сам код, но и наличие хорошей инфраструктуры, для которой нужны администраторы, DevOps. Также нужны тестировщики, которые будут тестировать сервисы и их интеграцию. Так как проект большой, важно и наличие руководящих людей, вроде технического директора
* Потеря персональных данных:
  Влечёт за собой финансовые и репутационные потери
* Неучтённые юридические риски:
  Для того, чтобы не попасть в данный пункт нужно нанять хорошего юриста, который сможет проконсультировать по всем нюансам стран, в которых планируется вестись работа
* Политические риски:
  Всегда есть риски того, что спецслужбы будут заинтересованы в определённых данных или применят санкции, ограничивающие или затрудняющие работу приложений. Нужно быть к этому готовым
