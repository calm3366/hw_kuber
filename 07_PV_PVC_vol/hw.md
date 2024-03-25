## «Хранение в K8s. Часть 2»
### Задание 1. 
[deploy.yaml](deploy.yaml) 

[local-pv.yaml](local-pv.yaml) 

[local-pvc.yaml](local-pvc.yaml) 

![!\[Alt text\](<img/!\[Alt text\](<img/1.png>)>)](<img/1.png>)

PV сохраняется, т.к. не зависит от удаления PVC

![!\[Alt text\](<img/!\[Alt text\](<img/2.png>)>)](<img/2.png>)

файл сохранился на локальном диске ноды:

![!\[Alt text\](<img/!\[Alt text\](<img/3.png>)>)](<img/3.png>)

после удаления PV - файлы сохранились, т.к. persistentVolumeReclaimPolicy: Retain

![!\[Alt text\](<img/!\[Alt text\](<img/4.png>)>)](<img/4.png>)

### Задание 2. 

Чтение и запись изнутри контейнера работает при монтировании PV из NFS сервера внутри кластера:

![!\[Alt text\](<img/!\[Alt text\](<img/5.png>)>)](<img/5.png>)




