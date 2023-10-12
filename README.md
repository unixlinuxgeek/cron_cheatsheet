### Добавляем в crontab задание запуска ncalayer 

Открываем файл crontab:
```
sudo crontab -e
```


#### И добавляем в самый конец:

Где ```/script-path``` - путь до нашего скрипта

```@reboot /script-path/start.sh``` 

Например:

```
# NCALayer запустится после 30 сек. с момента загрузки системы 
@reboot /home/geek/NCALayer/start.sh
```

```/home/geek``` - папка пользователя geek 

