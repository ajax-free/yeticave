# Личный проект «YetiCave»

[Опубликованная версия](https://yeticave.efiand.ru)

## Установка

```
composer install
sudo mysql -u root -p
  CREATE DATABASE yeticave;
  USE yeticave;
  GRANT all ON yeticave TO root IDENTIFIED BY '<YOUR_ROOT_PWD>';
  FLUSH PRIVILEGES;
  \q
sudo mysql -u root -p yeticave < schema.sql
sudo mysql -u root -p yeticave < data.sql
```

На 2 уровня выше создается файл env.php:

```php
<?php

$_ENV['DB_PASS'] = 'MY_DB_PASS';
```

---

<a href="https://htmlacademy.ru/intensive/adaptive"><img align="left" width="50" height="50" alt="HTML Academy" src="https://up.htmlacademy.ru/static/img/intensive/adaptive/logo-for-github.svg"></a>

Репозиторий создан для обучения на интенсивном онлайн‑курсе «[Базовый PHP](https://htmlacademy.ru/intensive/php)» от [HTML Academy](https://htmlacademy.ru).
