# Laravel

## Blade

## Controllers

### Особенности
Контроллеры должны быть строго в единственном числе, без пробелов между словами и заканчиваться на «Controller».

Создание CRUD
php artisan make:controller Api/CountriesController -m Models/Country


## DB

### Особенности:
- может быть несколько DB; 
- можно использовать мягкое удаление;
- стоит использовать индексы;
- создание внешних ключей, лучше делать отдельной миграцией, после создания всех требуемых таблиц;
- Eloquent has one по умолчанию таблицы
- lazy загрузка

### Различные команды:
#### Создание таблицы:
-таблицы создаются во множественном числе, модели создаются в единичном числе, модель  - представление одной сущности.  

```php
php artisan make:migration create_construction_types_table
```

#### Создание Модели
- модели создаются в единичном числе, модель  - представление одной сущности. Таблицы создаются во множественном числе. 
- ключ help покажет требуемые поля;
- можно использовать различные ключи, чтобы создать сразу модель, контроллер и фабрику
- чтобы поместить в папку Model - "Model/Accaunt"

```php
php artisan help make:model Accaunt
```

```php
php artisan make:model Accaunt
```

```php
php artisan make:model Model/Accaunt
```

#### Создание Сидов
- при ручном создании сидов надо выполнять  очистку "composer dumpautoload" , для всего, что есть в папке database

#### Кеширование
- Lock
- Rememberable


#links

##Convention
https://github.com/alexeymezenin/laravel-best-practices#follow-laravel-naming-conventions