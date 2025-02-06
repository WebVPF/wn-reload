# Wn-Reload

**Wn-Reload** - это расширение для браузера Chrome, являющееся настраиваемым LiveReload'ером для сайтов работающих на Winter CMS.

Данное расширение подойдёт для людей занимающихся созданием контента на сайте. Например, вы пишете статью в бэкенде сайта, а в другом окне браузера у вас открыта статья на фронтенде. Каждый раз при сохранении статьи в бэкенде, вкладка браузера со статьёй на фронтенде будет автоматически обновляться.

Wn-Reload не является привычным для разработчиков LiveReload'ером и не подходит для классической разработки когда редактируются код, скрипты и стили.

<!-- ## Установка

Маркет Chrome - https://chrome.google.com/webstore/detail/octoreload/idfbcpnoenglohbnkagghmioonmbphkj -->

## Настройки

Для сохранения есть кнопка **Сохранить настройки**, расположенная всегда внизу, а также доступна комбинация клавиш <kbd>Ctrl</kbd> + <kbd>S</kbd>. Рекомендуем переодически сохранять настройки, чтобы не утратить введённые данные.

## Добавление сайта

1. Нажмите кнопку Добавить сайт.
2. Введите hostname* сайта для которого нужно включить Wn-Reload.
3. Установите выключатель в позицию ВКЛ

*hostname - это домен или поддомен без указания протокола. Пример: `example.com` и `subdomen.example.com`.

При добавлении сайта, он также появится в навигационной панели, которая находится слева.

Первым делом необходимо указать Бэкенд URL. Если вы не меняли в конфигурации адрес для бекенда, оставьте `backend`.

## Добавление модели

Для каждого сайта нужно добавить модели. Нажмите кнопку **Добавить модель**. В параметрах сайта добавится блок с настройками для модели. Прежде всего выберите тип модели.

### Модель Category

Путь этой модели выглядит как `/:category` или `path/:category`. У данной модели есть item'ы которым назначается категория.

Заполните таблицу состоящую из двух столбцов. В первом столбце Id-категории укажите цифру являющуюся id-категории, во втором столбце - путь урл до страницы категории на фронте.

Например, у нас есть категория _animals_, доступная по адресу `https://example.com/animals`. В столбце Путь категории укажите `animals`.

Так же на сайте есть категория _fish_, доступная по адресу `https://example.com/animals/fish`. В столбце Путь категории укажите `animals/fish`.

### Модель Item

Путь этой модели выглядит как `/:category/:slug` или `path/:category/:slug`

### Модель Path

Путь такой модели выглядит как `/path/:slug`

## Ссылка на фронт страницу

В настройках каждой модели есть пункт: **Вставить ссылку на фронт-страницу в сайтбаре бекенда**.

## Import и Export настроек

В Wn-Reload есть возможность импортировать и экспортировать настройки расширения. Также доступна синхронизация настроек расширения для гугл-аккаунта.
