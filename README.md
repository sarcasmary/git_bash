# Работа с git и bash
## Задание 1
### 1. Перейти в домашнюю директорию
cd

### 2. Вывести текущий рабочий каталог
pwd

### 3. Создать каталог test1
mkdir test1

### 4. Перейти в каталог test1
cd test1

### 5. Создать три файла (file1.txt, file2.txt, file3.txt)
touch file{1,2,3}.txt

### 6. Просмотр содержимого текущего каталога
ls

### 7. Вернуться в домашнюю директорию
cd

### 8. Создать каталог test2
mkdir test2

### 9. Удалить пустой каталог test2
rmdir test2

### 10. Удалить файл file2.txt в каталоге test1
rm test1/file2.txt

### 11. Создать каталог test3
mkdir test3
cd test3

### 12. Создать два файла (file1.txt, file2.txt)
touch file{1,2}.txt

### 13. Удалить каталог test3 и все его содержимое
rm -rf test3

### 14. Создать каталог test4
mkdir test4

### 15. Переместить файлы file1.txt и file3.txt из test1 в test4
mv ~/test1/file{1,3}.txt ~/test4

### 16. Перейти в каталог test4
cd test4

### 17. Добавить строки в файл file1.txt
echo "line1" >> file1.txt
echo "line2" >> file1.txt
echo "line3" >> file1.txt

### 18. Просмотр содержимого файла file1.txt
cat file1.txt

### 19. Добавить строки в файл file3.txt
echo "line4" >> file3.txt
echo "line5" >> file3.txt
echo "line6" >> file3.txt

### 20. Просмотр содержимого обоих файлов (file1.txt и file3.txt)
cat file1.txt file3.txt

### 21. Открыть файл file1.txt в редакторе nano и выполнить ручную замену
nano file1.txt  # В редакторе вручную выполните замену текста

## Задание 2

### 1. Создать каталог test3
mkdir test3

### 2. Перейти в каталог test3
cd test3

### 3. Создание трех файлов с данными
echo -e "row1\nrow2\nrow3\nrow4" > file4.txt
echo -e "row1\nrow2\nrow3\nrow4" > file5.txt
echo -e "row1\nrow2\nrow3\nrow4" > file6.txt

### 4. Найти строку "row2" в файле file5.txt
grep "row2" file5.txt

### 5. Найти все строки, содержащие "row", рекурсивно во всей текущей директории
grep -R "row" .

### 6. Подсчитать количество строк с "row" в файле file6.txt
grep -c "row" file6.txt

### 7. Найти файл с именем "file5.txt" в текущей директории и подкаталогах
find . -name "file5.txt"

### 8. Найти и удалить файл "file5.txt" в текущей директории и подкаталогах
find . -name "file5.txt" -delete

### 9. Перезаписать содержимое файла file4.txt строкой "test"
echo test > file4.txt

### 10. Заменить все вхождения "test" на "fail" в файле file4.txt с использованием sed
sed 's/test/fail/g' file4.txt

### 11. Добавить строку "test" в конец файла file4.txt
echo test >> file4.txt

### 12. Просмотр всех процессов на системе
ps aux

### 13. Убить процесс с PID 666 
kill 666 

### 14. Отправить ping запрос на rusau.net
ping rusau.net

### 15. Отправить 5 ping запросов на rusau.net
ping -c 5 rusau.net

### 16. Выполнить GET запрос с использованием curl на Swagger API для поиска зарегистрированных питомцев
curl https://petstore.swagger.io/v2/pet/findByStatus?status=registered 

### 17. Выполнить POST запрос с использованием curl для добавления нового пользователя в Swagger API
curl -X POST https://petstore.swagger.io/v2/user --data "id=1" \
--data "username=Mishka_Kakabu" \
--data "firstName=Mishka" \
--data "lastName=Kakabu" \
--data "email=MishKabu@gmail.com" \
--data "password=rule210about" \
--data "phone=7695423659" \
--data "userStatus=0"
