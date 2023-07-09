###  Linux terminal (GitBash) commands 

>1. Посмотреть где я
   ```
      $ pwd
   ```
>2. Создать папку
 ```
   $ mkdir Homework
 ```
>3. Зайти в папку
 ```
 $ cd Homework
```
>4.  Создать 3 папки
```
 $ mkdir Folder_1 Folder_2 Folder_3
```
>5. Зайти в любую папку
   ```
   $ cd Folder_1
```
>6. Создать 5 файлов (3 txt, 2 json)
 ```
$ touch first.txt second.txt third.txt first.json second.json
```
>7. Создать 3 папки
 ```
 $ mkdir papka_1 papka_2 papka_3
```
>8. Вывести список содержимого папки
 ```
$ ls -la
```
>9.  Открыть любой txt файл
 ```
$ vim third.txt
```
>10.  Hаписать туда что-нибудь, любой текст.
 ```
  i                      Lee Copeland is an internationally known consultant in
                          software testing, with over 30 years of experience
                          as an information systems professional. 
                          He has held a number of technical and 
                          managerial positions with commercial and
                          nonprofit organizations in the areas
                          of software development, testing, and 
                          process improvement. He has taught 
                          seminars and consulted extensively
                          throughout the United States and internationally
```
>11. Cохранить и выйти.
 ```
 esc :wq
```
>12. Выйти из папки на уровень выше
 ```
$cd ..
```
>13. переместить любые 2 файла, которые вы создали, в любую другую папку.
 ```
$ mv first.txt first.json papka_1
```
>14. Cкопировать любые 2 файла, которые вы создали, в любую другую папку.
 ```
$ cp second.txt second.json papka_2
```
>15. Найти файл по имени
 ```
$ find third.txt
```
>16. просмотреть содержимое в реальном времени 
 ```
$ less +F third.txt                               
 Ctrl+c   (прервать )        q  (выйти из представления)
```
или
```
$ tail -F third.txt
```
>17. Bывести несколько первых строк из текстового файла
 ```
$ head -4 third.txt
```
>18. Bывести несколько последних строк из текстового файла
 ```
$ tail -3 third.txt
```
>19. просмотреть содержимое длинного файла 
 ```
less third.txt
 Ctrl+c   (прервать )        q  (выйти из представления)
```
>20. Bывести дату и время
 ```
$ date
```
---

### Задание *
A) Отправить http запрос на сервер.
http://162.55.220.72:5005/terminal-hw-request
      curl http://162.55.220.72:5005/terminal-hw-request
Answer     404 Not Found
```
        curl http://162.55.220.72:5005/
Answer    Hello!!!!!!!!!188.146.12.159
```
B) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13
                
Создать файл в корневой папке  и открыть его для редактирования         
```
touch homework_script.sh
vim homework_script.sh  
         i
```
Строка Шебанг
```
   #!/bin/bash
 ```
Bыполнить следующие пункты:

  3) Зайти в папку   `cd Homework`
  
  4) Создать 3 папки ` mkdir Folder_4 Folder_5 Folder_6`
     
  5) Зайти в любую папку                    ` cd Folder_4 `
     
  6) Создать 5 файлов (3 txt, 2 json) `touch first.txt second.txt third.txt first.json second.json`
 
  7)  Создать 3 папки 1 `mkdir papka_1 papka_2 papka_3`
  
  8)  Вывести список содержимого папки  `ls -la`
      
  13)переместить любые 2 файла, которые вы создали, в любую другую папку. `mv first.txt first.json papka_1`
  
Выйти из режима редактирования `Esc :x`

Выполнить скрипт   `sh homework_script.sh`







