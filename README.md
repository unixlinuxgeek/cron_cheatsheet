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

Запускаем скрипт stop.sh из коммандной строки:
```
/home/geek/NCALayer/stop.sh
```
