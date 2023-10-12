### Добавляем в crontab задание запуска ncalayer 

Открываем файл crontab:
```
sudo crontab -e
```


#### И добавляем в самый конец:

Где ```/script-path``` - путь до нашего скрипта

```
@reboot /script-path/start.sh
``` 

Например:

```
# Запускаем NCALayer
@reboot /home/geek/NCALayer/start.sh
```

```/home/geek``` - папка пользователя geek 



### Останавливаем NCALayer

Если вдруг необходимо остановить NCALayer выполняем в  коммандной строке:

Переходим в папку с NCALayer-ом и запускаем
```
./stop.sh
```
