# Работа с git и bash
## Задание 1
```bash 
1. Переход в домашнюю директорию
cd

2. Вывод текущего рабочего каталога
pwd

3. Создание каталога test1
mkdir test1

4. Переход в каталог test1
cd test1

5. Создание трех файлов (file1.txt, file2.txt, file3.txt)
touch file{1,2,3}.txt

6. Просмотр содержимого текущего каталога
ls

7. Возвращение в домашнюю директорию
cd

8. Создание каталога test2
mkdir test2

9. Удаление пустого каталога test2
rmdir test2

10. Удаление файла file2.txt из каталога test1
rm test1/file2.txt

11. Создание каталога test3
mkdir test3
cd test3

12. Создание двух файлов (file1.txt, file2.txt)
touch file{1,2}.txt

13. Удаление каталога test3 и всего его содержимого
rm -rf test3

14. Создание каталога test4
mkdir test4

15. Перемещение файлов file1.txt и file3.txt из test1 в test4
mv ~/test1/file{1,3}.txt ~/test4

16. Переход в каталог test4
cd test4

17. Добавление строк в файл file1.txt
echo "line1" >> file1.txt
echo "line2" >> file1.txt
echo "line3" >> file1.txt

18. Просмотр содержимого файла file1.txt
cat file1.txt

19. Добавление строк в файл file3.txt
echo "line4" >> file3.txt
echo "line5" >> file3.txt
echo "line6" >> file3.txt

20. Просмотр содержимого обоих файлов (file1.txt и file3.txt)
cat file1.txt file3.txt

21. Открытие файла в редакторе nano и ручная замена всех строк
nano file1.txt  
```

## Задание 2
``` bash
1. Создание каталога test3
mkdir test3

2. Переход в каталог test3
cd test3

3. Создание трех файлов с данными
echo -e "row1\nrow2\nrow3\nrow4" > file4.txt
echo -e "row1\nrow2\nrow3\nrow4" > file5.txt
echo -e "row1\nrow2\nrow3\nrow4" > file6.txt

4. Поиск строки "row2" в файле file5.txt
grep "row2" file5.txt

5. Поиск всех строк, содержащих "row", рекурсивно во всей текущей директории
grep -R "row" .

6. Подсчет количества строк с "row" в файле file6.txt
grep -c "row" file6.txt

7. Поиск файла с именем "file5.txt" в текущей директории и подкаталогах
find . -name "file5.txt"

8. Поиск и удаление файла "file5.txt" в текущей директории и подкаталогах
find . -name "file5.txt" -delete

9. Перезапись содержимого файла file4.txt строкой "test"
echo test > file4.txt

10. Замена слова "test" на "fail" в файле file4.txt с использованием sed
sed 's/test/fail/g' file4.txt

11. Добавление строки "test" в файл file4.txt
echo test >> file4.txt

12. Просмотр всех процессов в системе
ps aux

13. Уничтожение процесса с PID 666 
kill 666 

14. Отправление ping запроса на rusau.net
ping rusau.net

15. Отправление 5 ping запросов на rusau.net
ping -c 5 rusau.net

16. Выполнение GET запроса с использованием curl на Swagger API для поиска зарегистрированных питомцев
curl https://petstore.swagger.io/v2/pet/findByStatus?status=registered 

17. Выполнение POST запроса с использованием curl для добавления нового пользователя в Swagger API
curl -X POST https://petstore.swagger.io/v2/user --data "id=1" \
--data "username=Mishka_Kakabu" \
--data "firstName=Mishka" \
--data "lastName=Kakabu" \
--data "email=MishKabu@gmail.com" \
--data "password=rule210about" \
--data "phone=7695423659" \
--data "userStatus=0"
```
