---
title: "Недостаточно средств"
date: 2018-06-01 00:01:00
tags:
  - недостаточно
  - средства
  - средства
categories:
  - 
    - common-issues
primary_category: common-issues
primary_category_display_name: "Распространенные проблемы"
alias:
  - gas/error-insufficient-funds-message.html
---

# **Ошибка: недостаточно средств**

###### {% read_time title "Insufficient Funds" %} минут на чтение

* * *

Если вы видите ошибку, которая выглядит подобным образом: `Недостаточно средств. На аккаунте, с которого вы пытаетесь осуществить отправку, недостаточно средств. Требуется XXXXXXXXXXXXXXXXXXX, а есть: XXXXXXXXXXXXXXXX`, это значит, что на вашем аккаунте недостаточно ETH, чтобы оплатить стоимость газа.

Для каждой транзакции (включая транзакции с токенами и контрактами) нужен газ, который покупается за ETH. Вы можете рассматривать это как комиссию за транзакцию.

## **Решение: отправьте 0,01 ETH на этот аккаунт, чтобы иметь возможность совершить транзакцию.**

В стандартной операции лимит газа составляет `21 000 единиц`, а цена газа — `0,00000002 ETH`, то есть общий операционный сбор будет `0,00042 ETH`. С токенами количество газа обычно `50 000 — 100 000 единиц`, поэтому общий операционный сбор увеличивается до `0,001–0,002 ETH`.

Число, отображенное в данном сообщении об ошибке, — это сумма, нужная для оплаты транзакции в Wei. Возьмите это число и разделите на `1 000 000 000 000 000 000`. Это даст вам сумму эфира, которую вам нужно отправить на данный аккаунт, чтобы совершить транзакцию.

## **Подробнее о газе**

* Стандартная транзакция будет стоить `21 000` единиц газа, а цена газа — `0,00000002 ETH`, поэтому общий операционный сбор составит `0,00042 ETH`.
* С токенами количество газа обычно 50 000 — 100 000 единиц, поэтому общий операционный сбор увеличивается до `0,001–0,002 ETH`.
* Количество ETH или токенов, которые вы отправляете, не влияет на нужное вам количество газа.
* ***Лимит* газа** — это максимальное количество газа, которое вы отправите во время транзакции. Это в единицах газа.
* ***Цена* газа**, которую вы не увидите нигде, за исключением офлайн-страницы, — это стоимость каждой единицы газа. Мы установили ее в размере `0,00000002 ETH`.