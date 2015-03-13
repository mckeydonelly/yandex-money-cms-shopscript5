#[Y.CMS Shop-Script5](https://github.com/yandex-money/yandex-money-cms-shopscript5/raw/master/ss5.zip) 

Мы собрали все основные сервисы Яндекса в одном месте,чтобы вам было удобно работать со своим сайтом, сделанном на CMS Prestashop. Подробнее о возможностях этого модуля:

##[Яндекс.Касса](http://kassa.yandex.ru/) и на вашем сайте будут самые популярные способы оплаты.
> Доступные платежные методы, если вы работаете как юридические лицо:
>* **Банковские карты** -  Visa (включая Electron), MasterCard и Maestro любого банка мира
>* **Электронные деньги** - Яндекс.Деньги и WebMoney
>* **Наличные** - [Более 170 тысяч пунктов](https://money.yandex.ru/pay/doc.xml?id=526209) оплаты по России
>* **Баланс телефона** - Билайн, МегаФон и МТС
>* **Интернет банкинг** - Альфа-Клик и Сбербанк Онлайн
>

##[Яндекс.Деньги](https://money.yandex.ru/) - начните получать деньги прямо сейчас — от любых пользователей рунета.
> Переводы будут мгновенно зачисляться на ваш счет в Яндекс.Деньгах.
> Доступные платежные методы, если вы осуществляете p2p переводы:
>* **Банковские карты** -  Visa (включая Electron), MasterCard и Maestro любого банка мира
>* **Электронные деньги** - Яндекс.Деньги
>

##[Яндекс.Метрика](https://metrika.yandex.ru/) - бесплатный сервис, предназначенный для оценки посещаемости веб-сайтов, и анализа поведения пользователей.
> Метрика позволяет находить «узкие места» сайта и оптимизировать их, чтобы увеличивать число покупателей: https://metrika.yandex.ru/list/
>

##[Яндекс.Маркет](http://market.yandex.ru/) ([CPC](http://welcome.advertising.yandex.ru/market/), [CPA](http://help.yandex.ru/partnermarket/purchase/about.xml)) 
###Модуль CPA – программа "Покупка на Маркете"
> Модуль позволяет участвовать в программе «Покупка на Маркете». Заказать товары из магазинов, подключённых к программе, можно прямо на Маркете — не переходя на сайт продавца. «Покупка на Маркете» сокращает путь пользователя до покупки и повышает доверие к магазину. 
>

###Модуль СРС – размещение на Маркете 
> Модуль предназначен для размещения товарных предложений на Яндекс.Маркете. Так магазины могут привлекать на свой сайт больше посетителей, действительно заинтересованных в покупке. YML-формат обеспечивает максимально корректную передачу данных о товарах в Маркет.
>


###Лицензионный договор
Любое использование Вами программы означает полное и безоговорочное принятие Вами условий лицензионного договора, размещенного по адресу https://money.yandex.ru/doc.xml?id=527052 (далее – «Лицензионный договор»). Если Вы не принимаете условия Лицензионного договора в полном объёме, Вы не имеете права использовать программу в каких-либо целях.


##Инструкция по установке модуля
Для установки данного модуля необходимо распаковать [архив](https://github.com/yandex-money/yandex-money-cms-shopscript5/raw/master/ss5.zip) в корень вашего сайта!

Пожалуйста, обязательно делайте бекапы!

Для установки следует перейти в директорию ваш_сайт/wa-config/apps/shop/ и добавить запись о плагине в файле plugins.php.
Если в указанной папке нет файла plugins.php, то его необходимо создать.
И добавить строку 'yamodule' => true

Пример файла plugins.php:

```php
<?php
return array (
	'brands' => true,
	'yamodule' => true,
);
```

Далее заходим в админку сайта, жмём сверху ссылку "Магазин" и справа сверху "Плагины".
Слева мы увидим плагин Ya CMS Shop-Script 5.
Выбираем его и настраиваем.

Для использования платежных методов Кассы или p2p внесите необходимые настройки и активируйте нужный вам тип оплаты (p2p или Касса).

Для этого переходим в раздел "Настройки" (сверху справа). Переходим в раздел "Оплаты". Справа сверху экрана выбираем "Добавить способ оплаты" и выбираем Яндекс.Деньги. Вносим необходимые настройки и сохраняем.

Всё! Модуль приема платежей настроен.

**Внимание!**

Если вы хотите использовать p2p,то вам сначала необходимо [зарегистрировать своё приложение](https://tech.yandex.ru/money/doc/dg/tasks/register-client-docpage/).

Для сервисов Метрика и Маркет необходимо [зарегистрировать приложение](https://tech.yandex.ru/oauth/doc/dg/tasks/register-client-docpage/) на OAuth-сервере.

Все необходимые ссылки вы найдёте в настройках модуля!


##Нашли ошибку или у вас есть предложение по улучшению модуля?
Пишите нам cms@yamoney.ru
