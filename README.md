# Безопасный удалятор файлов SRM

## Описание проекта
SRM - это скрипт, который позволяет без страха удалять файлы. Скрипт перемещает выбранный файл в корзину. Файлы, лежащие в корзине дольше семи дней, удаляются безвозвратно.

## Установка
Для того, что бы установить скрипт, нужно скачать файл srm и посместить его в папку ~/bin. Затем набрать в коммандной строке следующие комманды:
```
chmod +x ~/bin/srm
echo 'export PATH="${PATH}:~/bin' >> ~/.bash_profile
. ~/.bashrc
```

## Как работать
Для того, что бы безопасно удалить файл, нужно набрать в коммандной строке ```srm <имя файла>```, например:

```srm testfile.txt```

если файл расположен в текущей директории, либо

```srm /file_path/testfile2.txt```

если файл находится за её пределами.

### Будьте внимательны, файлы, пролежавшие в корзине более семи дней будут удаляться!
