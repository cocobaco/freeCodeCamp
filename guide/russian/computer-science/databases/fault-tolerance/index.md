---
title: Fault Tolerance
localeTitle: Отказоустойчивость
---
## Отказоустойчивость

Отказоустойчивость - это свойство, позволяющее системе продолжать свою предполагаемую операцию, возможно, на более низком уровне, а не полностью отказываться, когда какая-то часть системы выходит из строя.

**База данных** является отказоустойчивой, когда она может получить доступ к вторичному осколку, когда основное недоступно.

Это достигается за счет:

*   Репликация базы данных
*   Поиск и устранение неисправностей

База данных, которая поддерживает несколько копий всех данных в разных физических узлах, расположенных в независимых физических подсистемах, таких как серверные стойки и сетевые маршрутизаторы, имеет более высокую вероятность продолжения работы, когда первичная копия данных недоступна из-за ее способности читать данные из нескольких повторений.

В крупномасштабных системах распределения становится все более важным иметь надежные системы обнаружения сбоев, которые могут идентифицировать отказоустойчивые накопители и предоставлять отказоустойчивые блоки, чтобы максимизировать время безотказной работы.