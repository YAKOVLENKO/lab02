## Laboratory work II

Данная лабораторная работа посвещена изучению утилит для разработки проектов

## Tasks

- [x] 1. Ознакомиться со ссылками учебного материала
- [x] 2. Выполнить инструкцию учебного материала
- [x] 3. Составить отчет и отправить ссылку личным сообщением в **Slack**
 
## Tutorial
Присваивание переменным GITHUB_USERNAME и GITHUB_TOKEN значения, после настройка редактор
```bash
$ export GITHUB_USERNAME=YAKOVLENKO # Присваиваем GITHUB_USERNAME значение YAKOVLENKO
$ export GIST_TOKEN=<сохраненный_токен> # Присваиваем GITHUB_TOKEN значение token, что мы получили из lab01
$ alias edit=vim # Настраиваем редактор vim
```
Работа с пакетным менеджером
```bash
$ npm install -g gistup 
```
Создание и заполнение файла .gistup.json
```bash
$ cat > ~/.gistup.json <<EOF #Создаем файл .gistup.json
{
  "token": "${GIST_TOKEN}" #Прописываем токен в файл .gistup.json
}
EOF
```
Переход в домашнюю папку и создание в ней новых папок
```bash
$ cd ~ # домашняя папка
$ mkdir -p workspace/labs/projects/ # Создаем папку projects
$ mkdir -p workspace/labs/tasks/ # Создаем папку tasks
$ mkdir -p workspace/labs/reports/ # Создаем папку projects, tasks, reports
```

## Report

```bash
$ cd ~/workspace/labs/ # Переходим в папку labs
$ export LAB_NUMBER=02 # Присваиваем LAB_NUMBER значение 02
$ git clone https://github.com/tp-labs/lab${LAB_NUMBER} tasks/lab${LAB_NUMBER} # Получаем информацию с github
$ mkdir reports/lab${LAB_NUMBER} # Создаем новую папку
$ cp tasks/lab${LAB_NUMBER}/README.md reports/lab${LAB_NUMBER}/REPORT.md # Переименовываем README.md и копируем в созданную папку
$ cd reports/lab${LAB_NUMBER} # Входим в папку
$ edit REPORT.md # Редактируеме файл
$ gistup -m "lab${LAB_NUMBER}"
```

## Links

### Unix commands

- [ar](https://en.wikipedia.org/wiki/Ar_(Unix))
- [cat](https://en.wikipedia.org/wiki/Cat_(Unix))
- [cd](https://en.wikipedia.org/wiki/Cd_(command))
- [cp](https://en.wikipedia.org/wiki/Cp_(Unix))
- [cut](https://en.wikipedia.org/wiki/Cut_(Unix))
- [echo](https://en.wikipedia.org/wiki/Echo_(command))
- [env](https://en.wikipedia.org/wiki/Env_(shell))
- [ex](https://en.wikipedia.org/wiki/Ex_(editor))
- [file](https://en.wikipedia.org/wiki/File_(command))
- [find](https://en.wikipedia.org/wiki/Find)
- [ls](https://en.wikipedia.org/wiki/Ls)
- [man](https://en.wikipedia.org/wiki/Man_page)
- [mkdir](https://en.wikipedia.org/wiki/Mkdir)
- [mv](https://en.wikipedia.org/wiki/Mv)
- [nm](https://en.wikipedia.org/wiki/Nm_(Unix))
- [ps](https://en.wikipedia.org/wiki/Ps_(Unix))
- [pwd](https://en.wikipedia.org/wiki/Pwd)
- [rm](https://en.wikipedia.org/wiki/Rm_(Unix))
- [sed](https://en.wikipedia.org/wiki/Sed)
- [touch](https://en.wikipedia.org/wiki/Touch_(Unix))

### Package Managers

- [apt](http://help.ubuntu.ru/wiki/apt) | [dnf](https://en.wikipedia.org/wiki/DNF_(software)) | [yum](https://fedoraproject.org/wiki/Yum/ru)
- [brew](https://brew.sh) | [linuxbrew](http://linuxbrew.sh)
- [npm](https://docs.npmjs.com)

### Software

- [curl](https://www.gitbook.com/book/bagder/everything-curl/details)
- [wget](https://www.gnu.org/software/wget/manual/wget.pdf)
- [clang](https://clang.llvm.org)
- [g++](https://gcc.gnu.org/onlinedocs/gcc-4.0.2/gcc/G_002b_002b-and-GCC.html)
- [make](https://en.wikipedia.org/wiki/Make_(software))
- [open](https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man1/open.1.html)
- [openssl](https://www.openssl.org)
- [nano](https://www.nano-editor.org)
- [tree](https://linux.die.net/man/1/tree)
- [vim](http://www.vim.org)

```
Copyright (c) 2017 Братья Вершинины
```
