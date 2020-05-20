Tренировочный проект regExp
=====

#### Cсылка на рабочую версию формы: ...

Это тренировочный проект онлайн-курсов Я.Практикума по веб-разработке. Разметка и вёрстка написаны разработчиками курса. Мною написаны только регулярные выражения, позволяющие делать валидацию полей формы.

####Критерии для валидации полей:


###### Name
* только кириллица;
* первая буква заглавная;
* можно ввести от 2 до 20 символов — это можно задать в атрибутах minlength и maxlength;
* возможна запись двойных имён — например, Анна-Мария;
* шаблон должен находить имена таких форматов:

Примеры:
```
Ян
Максим
Серёга
Ёль
Джон-дон
Джон-Дон
```


###### Email
* только латиница;
* «собака» @ — обязательный символ;
* точка . — тоже обязательный символ;
* цифры, подчерк, тире — разрешённые символы;

Шаблон должен находить e-mail таких форматов:

```
ya2@2ya.ru - имя и домен могут содержать цифры
ya-e@ya-ya.ru - имя и домен могут содержать тире
ya@x.ru - доменное имя может состоять из одного символа
y@ya.ru - имя ящика может состоять из одного символа
some@mail.ya.ru - доменное имя может содержать поддомен
```


######  Телефон

Шаблон для телефона должен находить номера таких форматов:

```
+7(925)900-90-90
+7(925) 900-90-90
+7 925-900-90-90
+79259009090
89259009090
```

Помните о пробелах — они могут встречаться в номере.


###### Сайт

Адрес сайта должен:

* начинаться с http:// или https://;
* затем www. — это необязательная группа;
* IP-адрес — 255.255.255.255 или доменное имя — stasbasov.ru;
* порт — тоже необязательная группа. Порт начинается с двоеточия, за которым идут от 2 до 5 цифр. Например: :8080;
* путь — последовательность из цифр, слешей и латинских букв, на конце которого может стоять решётка #;


Шаблон должен находить url таких форматов:

```
http://ya.ru
https://www.ya.ru
http://2-domains.ru
http://ya.ru:98/
http://ya.com:30
http://ya.ru/path/to/deep/
http://ya-ya-ya.ru
http://8.8.8.8:8080
http://8.8.8.8:8080/page/to/deep#
```
