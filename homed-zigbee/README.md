# HOMEd hassio add-on

Аддон [HOMEd ZibGee](https://github.com/u236/homed-service-zigbee) для Home Assistant OS и Home Assistant Supervised.

## Информация по настройке

Настройки аддона не предполагают настраивать HOMEd через интерфейсы аддона. Вся настройка выполняется вручную, через редактирование
конфигурационного файла /config/homed/homed-zigbee.conf согласно [официальному руководству](https://wiki.u236.org/page/ZigBee/Установка/Docker),
за исключением мапинга файлов. Вместо виртуального каталога /data мапится виртуальный каталог /config, и уже там в каталоге homed располагаются 
все файлы HOMEd.

Пример конфигурационного файла с нужными правками (секция device) приведён [здесь](https://github.com/ANS-spb/hassio-addons/blob/main/homed-zigbee/homed-zigbee.conf.example)
