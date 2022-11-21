# Здравствуйте, дорогие студенты! Перед Вами пятая (третья) лабораторная работа по дисциплине "Языки программирования"

Лабораторная работа #3 выполняется по вариантам. Варианты считаются так: переводите свою фамилию на английский, смотрите на `ASCII`-код первой буквы фамилии по [этой таблице](https://www.johndcook.com/ascii.png) и берёте (остаток от деления `ASCII`-кода на 2) + 1. Выполнение неправильного варианта будет приравнено к нулю.
## Жесткий дедлайн пулл-реквеста — 20:00 28.11

При форке репозитория Вы редактируете свой README.md файл таким образом:

```README.md```:
```Markdown
<# Варианта> + <ФИО> + <Группа> + < t.me/<ваш юзернейм в телеграме> >

 ```
К защите приглашаются те, кому ассистенты напишут в телеграме. Остальные могут сдавать лабу без защиты.

СКБ221_1 СКБ223_1 СКБ223_2 защищаются во вторник, 29.11

СК221_2 защищается в четверг, 01.12

## Задание для первого варианта:

Дано натуральное число строк `0 < T <= 10000`, в каждой из которых заданы 2 вещественных числа с точностью до второго знака после запятой - это отрезки на числовой прямой. В выводе запишите отрезки в том же формате, которые являются объединениями заданных отрезков. Учитывайте, что отрезки в выводе не должны иметь пересечений и должны идти по порядку. В случае отсутствия выведите сообщение *"NOTHING FOUND"*. 
Код программы должен содержать ввод с консоли флага `--tofile` и `--fromfile`. Первый говорит нам, что ввод будет задан в заданный пользователем в командной строке файл (в случае отсутствия файла создать его), а второй говорит о считывании из файла заданного пользователем. Предусмотреть возможность исполнения обоих флагов. Учесть возможность некорректного ввода и обработать исклюючения. На дополнительный балл (на 10 баллов) добавьте тесты, по возможности Google-Tests. 
```
Пример ввода:

5
1.2 3.4
-1.8 0.1
0.5 1.5
1.3 2.8 
-2 -1

Вывод для примера выше:

-2 0.1
0.5 3.4

```


## Задание для второго варианта:

Вводится последовательность предложений, оканчивающихся точкой. Предложения могут занимать более одной строки. Выведите все предложения в порядке неубывания длин ровно по одному на строку, заменяя перенос строки в исходном вводе пробельным символом. Код программы должен содержать ввод с консоли флага `--tofile` и `--fromfile`. Первый говорит нам, что ввод будет задан в заданный пользователем в командной строке файл (в случае отсутствия файла создать его), а второй говорит о считывании из файла заданного пользователем. Предусмотреть возможность исполнения обоих флагов. Учесть возможность некорректного ввода и обработать исклюючения. На дополнительный балл (на 10 баллов) добавьте тесты, по возможности Google-Tests. 
```
Пример ввода:

Alice's Adventures in Wonderland is a children's novel. The title is usually shortened to Alice in Wonderland. Charles Lutwidge Dodgson wrote the book. He wrote it using the pen name Lewis Carroll. John Tenniel drew the 42 pictures in the book. The book was published by Macmillan and Co in London. It was released on 26 November 1865. It has been adapted to numerous movies. In 2010, it has been adapted to Hollywood movie.

Вывод для примера выше. 

It was released on 26 November 1865.
It has been adapted to numerous movies.
Charles Lutwidge Dodgson wrote the book.
He wrote it using the pen name Lewis Carroll.
John Tenniel drew the 42 pictures in the book.
In 2010, it has been adapted to Hollywood movie.
The book was published by Macmillan and Co in London.
The title is usually shortened to Alice in Wonderland.
Alice's Adventures in Wonderland is a children's novel.

```
 Чтобы получить оценку 9, необходимо в отдельный файл `NINE.txt` выписать самое длинное предложение и, не используя средств языка `C++`, без выделения дин. памяти, перевернуть его, не переворачивая слова. То есть:
```
Пример ввода:
... (тут какие-то короткие предложения)
I love bananas

Вывод:
bananas love I
```

## Для обоих вариантов создать `Makefile` с возможностью сборки, `clean` и `distclean`. В случае использования `gtest`, использовать систему `CMake`. 
### Отчёты обязательны для всех. Необходимо описать функционал, используемые функции, приложить код (не скриншоты), сохранить в формате .pdf (иные форматы оцениваются в 0 баллов) в своём репозитории. 
Для удобства можете (и крайне рекомендуется) использовать Doxygen (имеется документация на оф. сайте).

Использование STL-контейнеров и `std::string` делит Вашу оценку пополам.


---

Спасибо [Анастасии Труфановой](https://github.com/neko-nyashka) за увиденный недочёт. +0.5 балла за внимательность.
