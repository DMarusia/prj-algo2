# Возможные задачи для курсового проекта

## Codename "RAR"

Задание: Реализовать утилиту компрессии файла, которая получает на вход ключ (`-c` (compress) или `-d` (decompress)) и имя входного файла, который сжимает/расжимает в файл с таких же именем и дополнительным расширением `.out`.

Пример запуска: 

```
$ compress -c file.txt
>> file.txt.out
$ compress -d file.txt.out
>>> file.text.out.out
```

Сжатие должно быть не меньше, чем для алгоритма LZW, но может быть больше. В качестве алгоритма компрессии можно использовать любой из известных алгоритмов, собственное улучшение какого-то алгоритма или свой вариант.


## Codename "Нова пошта"

Задание: Реализовать утилиту поиска кратчайшего маршрута на карте города Киева для грузовой машины, осуществляющей адресную доставку. Машина за один рейс выезжает со склада, объезжает несколько десятков точек и возвращается назад на склад. Координаты склада и точек-адресатов даются на вход в виде текстового файла в формате:

```
depot: 50.4655667,30.5109117
point1: 50.4434411,30.5134431
...
```

## Codename "Friend Suggest"

Cоциальный сервис twitter предлагает для зарегистрированных пользователей на кого бы подписаться.

![](twitter.png)

Задание: Реализовать утилиту/сервис предложения таких кандидатов для пользователя, используя список пользователей, на которых он подписан, а также, возможно, другие параметры (биографию, твиты и ретвиты).


## Codename "Wikipedia Search"

Задание: Реализовать утилиту поиска наиболее релевантного документа по поисковому запросу в коллекции документов с перекрестными ссылками, полученной из Википедии. Релевантность файла определяется наличием в нем максимального совпадения поисковой строки или хотя бы количества ключевых слов поискового запроса, а также его весом среди других документов (на основе алгоритма Pagerank или подобного ему).


## Codename "Grammarly"

Задание: Реализовать утилиту проверки правописания слов в украинских текстах использя словарь [dict_uk](https://github.com/arysin/dict_uk). Для несловарных слов утилита должна предлагать 1 кандидата на исправление. Качество ее работы будет проверено на специальном корпусе текстов, которые содержат ошибки используя метрику качества [f1](https://en.wikipedia.org/wiki/F1_score).


## Codename "Last.fm"

Задание: Реализовать утилиту, которая бы выдавала рекомендации музыки для пользователей Last.fm на основании данных о их предпочтениях и социальных связей, взятых из соответствующего [набора данных](http://ir.ii.uam.es/hetrec2011//datasets/hetrec2011-lastfm-2k.zip).


## Codename "Github"

Задание: Реализовать утилиту, которая бы осуществляла эффективное хранение истории изменений папки с файлами, подобной утилите `git`. Будучи запущенной в какой-то папке, она должна обрабатывать такие ключи:

- `-s` (snapshot) - создать новый снимок состояния директории и записать его в журнал изменений
- `-h` (history) - вывести всю историю изменений
- `-r <id снимка>` (rollback) - вернуться к состоянию директории, которое было на момент снимка с заданным id


## Codename "Uber"

Задание: Реализовать утилиту поиска кратчайшего пути на карте Киева между точками A и B, которые заданы в виде координат (например, `A: 50.4655667,30.5109117, B: 50.4434411,30.5134431`), для оптимизации работы службы такси. В идеале, утилита должна учитывать текущую сокорость движения по улицам с учетом пробок (эта информация предоставляется сервисом Yandex.Пробки или Google Maps Traffic). 


## Codename "6 handshakes"

Задание: Проанализировать социальную сеть [пользователей Livejournal](https://snap.stanford.edu/data/soc-LiveJournal1.html), содержащую несколько миллионов пользователей и их связей. Построить распределение расстояния между отдельными пользователями (проверить "Теорию шести рукопожатий"), найти самых влиятельных пользователей (т.н. Hubs) и т.д.


## Codename JPEG

Задание: Реализовать утилиту компрессии графических файлов по алгоритму JPEG, которая получает на вход имя входного файла и процент компресии (`-c`) (0 - без компрессии, 10 - максимальная компрессия), и сжимает его в новый файл с расширением `.jpg`.

Пример запуска: 

```
$ jpeg -c 5 image.png
>> image.jpg
```
