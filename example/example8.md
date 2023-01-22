# [POST и GET]

##  Работа с GET И POST запросами

### Содержание
* 1 Формируем запрос GET
* 2 Формируем запрос POST
* 3

## Описание

    Для обработки запроса используют...

### `examle8.php`

```php

    // Ссылка с одним GET параметром
    echo "<a href='example8.php?animals=Мишка'> Мой зверь <a> <br>";
    // Ссылка с двумя GET параметрами
    echo "<a href='example8.php?width=150'>Он Весит <a> <br>";

    // index.php?animals=Мишка
    echo $_GET['animals'];

    // index.php?animals=Мишка&width=150
    echo $_GET['width'];

    // проверка существует ли элемент запроса
    if (isset($_GET['animals'])) {
    	// Вылавливаем элемент animals
      echo " наконец ты к нам пришел: ".$_GET['animals'];
    }



```
