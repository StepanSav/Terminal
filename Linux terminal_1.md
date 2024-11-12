# Terminal linux Homework №1

1) Посмотреть где я

        pwd
2) Создать папку

       mkdir folder
4) Зайти в папку

        cd folder
5) Создать 3 папки

        mkdir folder{_1,_2,_3}
6) Зайти в любоую папку

       cd folder_1
8) Создать 5 файлов (3 txt, 2 json)

       touch f{_1,_2,_3}.txt f{_4,_5}.json
10) Создать 3 папки

        mkdir d{_1,_2,_3}
8. Вывести список содержимого папки

        ls -l
   
9) Открыть любой txt файл

        vim f_1.txt
10) Написать туда что-нибудь, любой текст.

        -press button 'i' and write text
        Hello.
        My name is Maxim.
        This is my first homework in the author's courses by Vadim Kzentsov.
11) Сохранить и выйти.

        press 'esc' and write :wq press "Enter"
12) Выйти из папки на уровень выше

        cd ..
13) переместить любые 2 файла, которые вы создали, в любую другую папку.

        mv -v folder_1/f{_1,_2}.txt folder_2
14) скопировать любые 2 файла, которые вы создали, в любую другую папку.

        cp folder_1/f{_4,_5}.json folder_2
15) Найти файл по имени

        find . -name 'f*.txt'
16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает.

        tail -f folder_2/f_1.txt

        -открываем файл f_1.txt через текстовый редактор, добавляем новую информацию и сохраняем файл f_1.txt;
        -добавленная информация отображается в окне терминала;
        -открываем файл f_1.txt через текстовый редактор, удалить добавленную информацию и сохраняем файл f_1.txt;
        -изменения отображаются в окне терминала;
        -для завершения отображения лога нажимаем Cntr+C.
        -для фильтрации информации в реальном времени используем команду tail -f folder_2/f_1.txt | grep "параметр"
18) вывести несколько первых строк из текстового файла

        head -n2 folder_2/f_1.txt
20) вывести несколько последних строк из текстового файла

        tail -n2 folder_2/f_1.txt
22) просмотреть содержимое длинного файла (команда less) изучите как она работает.

        less folder_2/f_1.txt
23) вывести дату и время

        date
-----

Задание *
1) Отправить http запрос на сервер. http://162.55.220.72:5005/terminal-hw-request

       curl http://162.55.220.72:5005/terminal-hw-request

ответ сервера содержит дополнительное задание

    curl 'http://162.55.220.72:5005/get_method?name=Maxim&age=30'
2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13

        vim script_hw_#1.sh
        press button 'i' and write:
        #!/bin/bash
        cd folder
        mkdir folder{_1,_2,_3}
        cd folder_1
        touch f{_1,_2,_3}.txt f{_4,_5}.json
        mkdir d{_1,_2,_3}
        ls -la
        mv f{_1,_2}.txt d_1
        press 'esc' and write :wq press "Enter"

        ./script_hw_#1.sh
-----
1) Посмотреть где я - pwd

       pwd
3) Создать папку - mkdir foldername

       mkdir foldername
5) Зайти в папку - cd foldername

       cd foldername
