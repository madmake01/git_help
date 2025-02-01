#Шпаргалка по работе с Git
все < > должны игнорироваться при использовании команд   

##1.	Команды Git Bash 
pwd - адрес текущей директории  
cd <адрес вида /c/papka> переход в указанную директорию по абсолютному пути  
cd переход по относительному пути  
cd ~ домашняя директория  
cd .. переход на уровень выше  
cd / переход в корневую директорию  
---
mkdir <название> создать папку  
touch <название> создать файл (или несколько)  
rm <название> удаление файла  
rmdir <название> удаление пустой папки  
rm -r <название> удаление папки со всем её содержимым  
##2.	Команды непосредственно Git  
git init создание репозитория в текущей директории  
git status отображение статуса репозитория (содержит информацию о недобавленных файлах или изменённых)  
git add <название файла> добавление файла в индекс  
git add . добавляет в индекс все новые, изменённые и удалённые файлы в текущей директории и её поддиректориях.  
git add --all аналогичен предыдущему пункту, только добавляет все новые, изменённые и удалённые файлы во всём репозитории, независимо от того, в какой директории вы находитесь.  
git commit -m "<какой-то текст>" создание коммита на основе добавленных файлов, добавленных через git add  
git log отображение коммитов текущей ветки в хронологическом порядке (альтернативы с говорящими названиями: git log --all, git log --all --graph, git log branch_name, git log --all -n 10, git log --all --oneline и прочее)  
git remote add origin <ссылка> привязка удалённого репозитория к локальному  
git remote -v проверка  
git push отправка изменений на удалённый репозиторий. В первый раз для синхронизации веток нужно выполнить git push -u origin main (или master)  
git clone <ссылка> клонировать репозиторий  
git diff показать разницу между текущими изменениями и последним коммитом  
git branch список локальных веток  
git checkout -b <имя_ветки> создать и переключиться на новую ветку  
git merge <ветка> слить указанную ветку с текущей  
git pull скачать и применить изменения с удалённого репозитория  

