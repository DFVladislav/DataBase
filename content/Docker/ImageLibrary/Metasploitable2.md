## Metasploitable2 docker

Выполните все этапы работы с проектом по примеру с [Nginx](/content/Docker/ImageLibrary/Nginx.md)

> Никогда в разработке не используйте русские имена файлов и каталогов!

> Никогда в разработке не используйте пробелы и спец.символы в именах файлов и каталогов!

```
Metasploitable2 — специально уязвимая виртуальная машина Linux, созданная проектом Metasploit. Предназначена для использования в качестве среды обучения и тестирования для специалистов и энтузиастов в области безопасности, чтобы практиковать навыки взлома и пентеста.
```

Установить докер-образ

```shell
docker pull tleemcjr/metasploitable2
```

<img width="677" height="257" alt="изображение" src="https://github.com/user-attachments/assets/c1104429-d6f3-4279-b8fd-badeda3bd368" />


Загрузить образ, создать и запустить контейнер, войти в него (для Windows)
```shell
docker run --name metasploitable2 -it tleemcjr/metasploitable2
```

<img width="617" height="474" alt="изображение" src="https://github.com/user-attachments/assets/c18c48f9-babf-4b0a-9e6a-866282f1f6dc" />


Загрузить образ, создать и запустить контейнер, войти в него (для Linux)
```shell
docker run --name metasploitable2 -it tleemcjr/metasploitable2:latest sh -c "/bin/services.sh && bash"
```

Остановить контейнер и выйти из него
```shell
exit
```

Удалить контейнер
```shell
docker rm metasploitable2
```

Удалить образ
```shell
docker rmi tleemcjr/metasploitable2
```
<img width="505" height="233" alt="изображение" src="https://github.com/user-attachments/assets/5b123414-ce67-451d-9789-301c6a865dba" />


[Metasploitable2 на Docker hub](https://hub.docker.com/r/tleemcjr/metasploitable2#!)

> Если вы обнаружили ошибку в этом тексте - сообщите пожалуйста автору!
