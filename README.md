# Директория local разработанного сайта на 1C-Битрикс

### Компонент отображения актуального курса валют
* Получает информацию с сервера ЦБ
* Кеширует запрос
* Выбор валюты из настроек
* Изменение кеширование из настроек
* При недоступности сервера ЦБ информация берется из кеша, если кеша нет выводится сообщение.


### Класс помошник
* Подключен через автозагрузчик Битрикса
* Доступен при подключенном ядре Битрикса
* Метод для вывода на экран в обёрнутого в тег содержимого
* Метод получения варианта окончания существительных после чисел

### Класс обработки заказов
* Подключен через автозагрузчик Битрикса
* Метод очистки полей пользователя при изменении статуса заказа на "Выполнен"
* Метод добавления поля адреса пункта выдачи в почтовый шаблон если выбран самовывоз. Адрес берется из склада выдачи.
* Вспомогательный метод для получения номера склада по номеру заказа
* Вспомогательный метод получения информации о складе

### Включены файлы миграции
Добавлены файлы миграции https://github.com/andreyryabin/sprint.migration
Изменен почтовый шаблон события отправки сообщения о новом заказе
Добавлено поле #ADDRESS# - Адрес пункта выдачи