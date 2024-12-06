# Самый простой гайд на zapret от bol-van для арчеводов
### Все команды выполняем под
```
sudo -s
```
Иначе придётся перед каждой писать `sudo` (для выхода набрать `exit`)

Также может убряться каталог пользователя то есть заместо `layder` в данном случае моё имя пользователя будет `~` и чтобы вернуться в домашнюю папку пишем
```
cd layder
```
`layder` заменить на ваше имя пользователья
## Установка зависимостей
`pacman -S --needed curl ipset bind git jq` строчка для арча и производных

`dnf install -y curl ipset dnsutils git jq` строчка для федоры

`apt install -y curl ipset dnsutils git jq` строчка для убунты

`pacman -S nftables` установка nftables
### Установка самого запрета
Скачать последний релиз .tar.gz с [тык](https://github.com/bol-van/zapret/releases)

Распаковываем

Для этого понадобиться утилита tar и gzip

```
pacman -S tar gzip
```

Далее переходим в папку загрузки и распаковываем
```
cd Загрузки
tar -xvzf zapret-v69.5.tar.gz -C /home
```
Где `zapret-v69.5.tar.gz` имя архива, на данный момент оно такое и `/home` - куда файл распаковывается
## Сама программа
Для начала переходим в папку с распакованной программой в моём случае это `/home`
```
cd /home
```
запускаем ./
