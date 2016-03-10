# bitrix-debug-toolbar

##Отладочная панель для 1С-Битрикс.

Позволяет выводить отладочную информацию из панели внизу экрана.
Создано под впечателением от фреймворка Yii.

Отладочная информация доступна после клика на числе возле надписи Debug.

###Для того, чтобы выводилась нужная информация нужно:

1. Подключить класс.
2. В любом месте вызвать `CDebug::add($var, "Variable description");` 
3. Подключить компонент панели. Пример в файле footer.php.
4. Можно установить префикс для удобной сортировки `CDebug::setPrefix("news.detail_");`

###На панели можно увидеть:

1. Версию PHP на сервере.
2. Статус ответа сервера.
3. Пиковое значение использованной памяти.
4. Время генерации страницы на сервере.
5. Время между запросом страницы и готовностью DOM.
6. Значения переменных `$_SERVER`, `$_SESSION`, `$_COOKIE`, `$_GET`, `$_POST`.