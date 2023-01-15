
## Пример 5

### `examle5.php`

```php
    define('DB_HOST', 'localhost'); // сервер
    define('DB_USER', 'root');      // пользователь
    define('DB_PASS', '');          // пароль
    define('DB_NAME', 'php_test');  // база данных
        
    // --выполняем подключение к серверу MySQL и выбираем с какой базой будем работать
    $connect = mysqli_connect(DB_HOST, DB_USER, DB_PASS, DB_NAME);
    // --выполняем SQL запрос
    $result = mysqli_query($connect, "SELECT * FROM users ORDER BY name");
    // --Получение количества строк в наборе результатов
    $row_cnt = mysqli_num_rows($result);

    printf("Получено %d строк.\n", $row_cnt);
    /*
      Семейство функций printf() использует символ в качестве заполнителя.
      При обнаружении printf считывает следующие символы % %,
      чтобы определить, что делать например: %s напечатать  целое число
        %s - The next argument print as string
        %d - The next argument print as int
     */
```
