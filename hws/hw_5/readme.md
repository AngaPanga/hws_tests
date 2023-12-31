Задание 1:

Представьте, что вы работаете над разработкой простого приложения для записной книжки, которое позволяет пользователям добавлять, редактировать и удалять контакты. Ваша задача - придумать как можно больше различных тестов (юнит-тесты, интеграционные тесты, сквозные тесты) для этого приложения. Напишите название каждого теста, его тип и краткое описание того, что этот тест проверяет.

**Ответ:**

***Юнит-тесты.***
1. Проверки отдельных объектов класса (используя Mock() ) 
* Корректное создание объектов
* Корректные типы данных
* Проверка пограничных случаев
2. Проверка методов объекта и его модель поведения на mock объекте

***Интеграционные тесты.***
1. Проверка наличия связи между классами
2. Проверка соответствия (нужный метод вызвает нужную функцию, метод другого обекта)
3. Проверка пограничных случаев (отсутствие зависимого объекта и т.п.)

***Сквозные тесты.***
1. Проверка логики поведения
2. Проверка корректности выполнения логики поведения (добавление, удаление, редактирование и т. д.)
3. Проверка не логичного поведения пользователя (ввод пустых данных, неправильных типов и прочее)
4. Проверка критического поведения системы (внезапное прерывание и т.п.)


Задание 2:

Ниже список тестовых сценариев. Ваша задача - определить тип каждого теста (юнит-тест, интеграционный тест, сквозной тест) и объяснить, почему вы так решили.

1. Проверка того, что функция addContact корректно добавляет новый контакт в список контактов.
2. Проверка того, что при добавлении контакта через пользовательский интерфейс, контакт корректно отображается в списке контактов.
3. Проверка полного цикла работы с контактом: создание контакта, его редактирование и последующее удаление.

**Ответ:**
1. В зависимости от модели программы данный тест будет либо Юнит, либо Сквозной
* Если данный метод проверяют на исполнение без вызова зависимого класса (используется заглушка) - Юнит
* Если метод не только вызывается но и создат объект класса - Сквозной
2. Данный вид теста Сквозной, т.к. есть связь между объектами классов и проверка логики и корректности поведения.
3. По скольку по условию не используется нтерфейс пользователя, так же не указано о проверки данных, можно считать данный тест интеграционным т.е. проверка корректных зависимостей.
