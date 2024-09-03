## Подготовка окружения в Ubuntu

Команды в терминале:
```
sudo apt-get update
sudo apt-get install flex
sudo apt-get install bison

sudo apt install build-essential gcc-multilib libncurses5-dev qemu-system-x86 qemu-system-arm
sudo apt install gdb
sudo apt install netcat-openbsd

git clone https://github.com/linux-kernel-labs/linux.git
```

Переходим в папку `../linux/tools/labs`
Перед работой, желательно очистить лабораторию от файлов, которые остались после компиляции.
Для этого выполним команду в директории `../linux/tools/labs`:
```
make clean
```

Выбрать лабораторию можно через использование переменной `LABS`:
```
LABS=kernel_modules make skels
```
// *Что такое skels?*\
// *TODO: Узнать что такое skels и что мы делаем переменной LABS*