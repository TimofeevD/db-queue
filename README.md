[![Build Status](https://travis-ci.org/yandex-money/db-queue.svg?branch=master)](https://travis-ci.org/yandex-money/db-queue)


# Описание

Реализация очередей поверх базы данных.

# Использование

## Ручная конфигурация

TODO

## Spring конфигурация

TODO

## Описание пакетов

* ru.yandex.money.common.dbqueue.internal

Внутренние классы реализации. 

*В классах данного пэкеджа, обратная совместимость 
между любыми релизами библиотеки не гарантируется*

* ru.yandex.money.common.dbqueue.api

Клиенту библиотеки необходимо предоставить реализацию 
интерфейсов этого пакета. Некоторые из интерфейсов предоставляют 
реализацию по умолчанию для упрощения конфигурирования.
Также содержит классы данных, участвующие в обработке очереди 
и постановке на выполнение.

* ru.yandex.money.common.dbqueue.settings

Пакет с классами, отвечающими за настройку очередей.

* ru.yandex.money.common.dbqueue.dao

Вспомогательные классы для управления и получения данных по очередям.
В случае стандартной реализации вам не потребуется доступ к методам данных классов.

* ru.yandex.money.common.dbqueue.init

Классы данного пэкеджа необходимо проинициализировать для запуска очередей

* ru.yandex.money.common.dbqueue.spring

Классы отвечающие за spring конфигурацию очередей.
