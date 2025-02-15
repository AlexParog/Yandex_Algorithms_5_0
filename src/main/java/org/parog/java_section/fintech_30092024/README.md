# Задача: Реализация системы перевода денежных средств между счетами

Вы разрабатываете часть ФинТех-приложения, которая реализует переводы денежных средств между счетами пользователей в
одной
системе. Задача заключается в проектировании и реализации функциональности перевода денег с одного банковского счета на
другой без использования сторонних фреймворков.

## Основные требования:

1. Моделирование сущностей:
    - Имеются класс Account (счет).
    - Счета должны хранить уникальный идентификатор, имя владельца, баланс (в валюте, например, BigDecimal).

2. Функциональные требования:
    - Реализовать перевод денег с одного счета на другой:
        - Проверка, достаточно ли средств на счете отправителя.
        - Если средств недостаточно, выбросить корректную обработку исключений.
    - Все операции перевода должны быть атомарными и защищены от проблем с многопоточностью.
    - Учесть возможные ошибки (например, невозможность перевода или недостаток средств).

3. Необходимые возможности:
    - Поддержка многопоточных операций перевода (синхронизация данных между потоками).
    - Обработка исключений.