# bash-commands
https://www.learnenough.com/command-line-tutorial#sec-editing_the_line

### Редактирование
* **Ctrl A** - _курсор в начало строки_
* **Ctrl E** - _курсор в конец строки_
* **Ctrl U** - _стирает текст слева до начала строки курсор в начало строки_
* **Ctrl C** - _отмена_
* **Ctrl L** - _clear или очистить экран_
* **Ctrl D** - _выход из терминала_

###  Files

* **echo 'text' > file-1.js** create file *file-1* and write 'text' to file
* **echo 'new line text' >> file-1.js**  add 'new line text' to file *file-1*
* **cat file-1.js**  view in console text from file
* **diff file-1.js file-2.js** comparison of two files

###	Listing file in directories
**ls**
**ls *.txt**  _only .txt files_	
**ls -l**     _long form_
**ls -a**	  _show hidden files_


### Rename file
**mv src.js dist.js**

### Copy
**cp src.js dist.js**	

### Delete
**rm src.js**
**rm -f src.js** _force remove_
	
### Tab completion
	
### Alias
*C:\Program Files\Git\etc\profile.d\aliases.sh*
**alias setdir='touch index.html | mkdir ./{css,js,img,assets} && touch ./{js/app.js,css/style.css}'**



##$ Создание директорий
* **mkdir -p $USER/{1,2,3}**

* **mkdir sa{1..50}** _50 directories from sa1 through sa50_

* **mkdir -p sa{1..50}/sax{1..50}** _same but each of the directories will hold 50 times sax1 through sax50 (-p will create parent directories if they do not exist._

* **mkdir** {a-z}12345 	_26 directories from a12345 through z12345_

* **mkdir {1,2,3}** _comma separated list makes dirs 1, 2 and 3._

* **mkdir test{01..10}**	_10 directories from test01 through test10._

* **mkdir -p `date '+%y%m%d'`/{1,2,3}** _same as 4 but with the current date as a directory and 1,2,3 in it._

* **mkdir -p $USER/{1,2,3}** _same as 4 but with the current user as a directory and 1,2,3 in it._
	
### Common
**whoami**	_текущий user_
**pwd**     _текущая директория_

===============================================================
Ключи команды test: # test == []
-d проверяет наличие файла и то, что он является каталогом
-e проверяет существование файла
-f проверяет наличие файла и то, что это обычный файл
-g проверяет наличие у файла SGID-бита
-r проверяет наличие файла и то, что он доступен на чтение
-s проверяет наличие файла и то, что его размер больше нуля
-u проверяет наличие у файла SUID-бита
-w проверяет наличие файла и то, что он доступен на запись
-x проверяет наличие файла и наличие у него прав на запуск

x -eq y x = y (equal)
x -ne y x не равен y (not equal)
x -gt y x больше, либо равен y (greater than)
x -lt y x меньше, либо равен y (lesser than)

Операторы сравнения строк:
x = y строка x идентична y
x != y строка х не совпадает y
-n x выражение истинно, если строка х ненулевой длины
-z x выражение истинно, если строка х имеет нулевую длину

for i in 1 2 3 4 5 6 7 8 9 10; do
echo $i
done 

if ...
then 
else ... 
elif ...
fi
