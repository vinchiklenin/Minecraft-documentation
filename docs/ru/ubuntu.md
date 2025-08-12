# Управление сервером

## Запуск сервера
```
ssh -l ubuntu 89.169.181.136
```
```
cd minecraft-server
```
```
screen
```
```
java -Xms3072M -Xmx3072M -XX:+UseG1GC -XX:+ParallelRefProcEnabled -XX:MaxGCPauseMillis=200 -XX:+UnlockExperimentalVMOptions -XX:+DisableExplicitGC -XX:+AlwaysPreTouch -XX:G1NewSizePercent=30 -XX:G1MaxNewSizePercent=40 -XX:G1HeapRegionSize=8M -XX:G1ReservePercent=20 -XX:G1HeapWastePercent=5 -XX:G1MixedGCCountTarget=4 -XX:InitiatingHeapOccupancyPercent=15 -XX:G1MixedGCLiveThresholdPercent=90 -XX:G1RSetUpdatingPauseTimePercent=5 -XX:SurvivorRatio=32 -XX:+PerfDisableSharedMem -XX:MaxTenuringThreshold=1 -Dusing.aikars.flags=https://mcflags.emc.gs -Daikars.new.flags=true -jar minecraft_server.jar nogui
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


