Первое ДЗ 
Linux terminal (GitBash) commands

1) Посмотреть где я - pwd
2) Создать папку - mkdir qa1
3) Зайти в папку - cd qa1
4) Создать 3 папки - mkdir f1 f2 f3
5) Зайти в любую папку – cd qa2
6) Создать 5 файлов (3 txt, 2 json) - cat > names.txt, cat > names1.txt, cat > names2.txt, cat > names21.json, cat > names22.json
7) Создать 3 папки - mkdir f1 f2 f3
8) Вывести список содержимого папки - ls -la
9) + Открыть любой txt файл – cat names.txt
10) + написать туда что-нибудь, любой текст. – cat >> names.txt (enter – Текст)
11) + сохранить и выйти. – Ctrl + c
12) Выйти из папки на уровень выше – cd ..
—
13) переместить любые 2 файла, которые вы создали, в любую другую папку.- mv qa2/names.txt qa1/names2.txt
14) скопировать любые 2 файла, которые вы создали, в любую другую папку. – cp qa2/names.txt qa1/names2.txt
15) Найти файл по имени find ./ -name “*.txt” – поиск по по окончанию .txt, * название файла.
16) просмотреть содержимое в реальном времени (команда grep) изучите как она работает grep -i ‘1’ names1.txt – показывает существующую строку в файле ‘names1.txt’ по имеющемуся значению ‘1’
17) вывести несколько первых строк из текстового файла - head -n 2 qa2/names.txt
18) вывести несколько последних строк из текстового файла -  tail -n 2 qa2/names.txt
19) просмотреть содержимое длинного файла (команда less) изучите как она работает.- less qa2/names.txt Для выходы ‘q’
20) вывести дату и время - date

=========

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
