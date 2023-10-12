### Добавляем в crontab задание запуска ncalayer 

Открываем файл crontab:
```
sudo crontab -e
```


#### И добавляем в самый конец:

```@reboot /script-path/start.sh``` 

Например:
 
```
# NCALayer запускается после 30 сек. с момента загрузки системы 
@reboot /home/geek/AfterLoad/NCALayer/start.sh
```


```geek``` - имя пользователя 
 
```AfterLoad``` - папка со скриптами
