# QuikPy
Библиотека-обертка, которая позволяет получить доступ к функционалу QUIK на основе [Документации по языку LUA в QUIK](https://arqatech.com/ru/support/files/) из Python. В качестве коннектора используются lua-скрипты [проекта QUIKSharp](https://github.com/finsight/QUIKSharp).

### Для чего нужна
С помощью этой библиотеки можно создавать автоматические торговые системы любой сложности на Python для QUIK. Также библиотека может быть использована для написания дополнений на Python к системам Технического Анализа. Например, для тестирования и автоматической торговли в [BackTrader](https://www.backtrader.com/).

### Установка коннектора
1.	Скопируйте папку **QUIK\lua** в папку установки QUIK. В ней находятся скрипты LUA.
2.	Скопируйте папку **QUIK\socket** в папку установки QUIK.
3.	Запустите QUIK. Из меню **Сервисы** выберите **Lua скрипты**. Нажмите кнопку **Добавить**. Выберете скрипт **QuikSharp.lua** Нажмите кнопку **OK**. Выделите скрипт из списка. Нажмите кнопку **Запустить**.

Скрипт должен запуститься без ошибок, в окне сообщений QUIK выдать **QUIK# is waiting for client connection...**

### Начало работы
В папке **Examples** находится хорошо документированный код примеров. С них лучше начать разбираться с библиотекой.

1. **Connect.py** - Подключение к терминалу QUIK. Singleton класс коннектора. Проверка соединения. Сервисные функции. Пользовательские обработчики событий. Просмотр изменений состояния соединения терминала QUIK с сервером брокера. Просмотр изменений параметров.
[Видео разбора кода >>>](https://finlab.vip/connectpy/)
2. **Accounts.py** - Список всех торговых счетов с лимитами, позициями, заявками и стоп заявками. Аналогично для заданного торгового счета.
3. **Ticker.py** - Информация о тикере
4. **Bars.py** - Получение свечек в файл. [Видео разбора кода >>>](https://finlab.vip/barspy/) [Видеоразбор удаления дожи 4-х цен >>>](https://finlab.vip/fourpricedoji/) [Видеоразбор удаления баров первого/последнего дня >>>](https://finlab.vip/skipdates/)
5. **Stream.py** - Подписки на получение стакана, обезличенные сделки, новые свечки. [Видео разбора кода >>>](https://finlab.vip/streampy/)
6. **Transactions.py** - Выставление новой лимитной/рыночной заявки, стоп заявки, отмена заявки.

### Авторство, право использования, развитие
Автор данной библиотеки Чечет Игорь Александрович.

Библиотека написана в рамках проекта [Финансовая Лаборатория](https://finlab.vip/) и предоставляется бесплатно. При распространении ссылка на автора и проект обязательны.

Исправление ошибок, доработка и развитие библиотеки осуществляется автором и сообществом проекта [Финансовая Лаборатория](https://finlab.vip/).
### Что дальше
- Бесплатный курс "Автоторговля" по идеям, концепциям и процессам алгоритмической/автоматической торговли [смотрите здесь >>>](https://finlab.vip/wpm-category/autotrading2021/)


- Бесплатный курс "BackTrader: Быстрый старт" [ждет вас здесь >>>](https://finlab.vip/wpm-category/btquikstart/)


- [Подписывайтесь на Telegram канал "Финансовой Лаборатории",](https://t.me/finlabvip) чтобы быть в курсе всех новинок алгоритмической и автоматической торговли.