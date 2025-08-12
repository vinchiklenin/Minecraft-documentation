# Управление сервером

## Запуск сервера
```
ssh -l ubuntu 89.169.181.136
cd minecraft-server
screen
java -Xmx1024M -Xms1024M -jar minecraft_server.jar nogui
```

## Выключение сервера
```
save-all
stop
```

## Подключени к консоли через power shell
```
ssh -l ubuntu 89.169.181.136
screen -x 2808
```


