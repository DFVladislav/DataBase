## Alt Linux в Docker

Выполните все этапы работы с проектом по примеру с [Nginx](/content/Docker/ImageLibrary/Nginx.md)

> Никогда в разработке не используйте русские имена файлов и каталогов!

> Никогда в разработке не используйте пробелы и спец.символы в именах файлов и каталогов!!

#### Использовать контейнер с Alt

##### Загрузить готовый образ Alt
```shell
docker pull alt:sisyphus
```

<img width="531" height="177" alt="изображение" src="https://github.com/user-attachments/assets/6138d195-8138-410b-a8fb-71e76bebdf9e" />


##### Запустить и использовать
```shell
docker run -ti --rm --name alt alt:sisyphus /bin/bash
```

#### Установить приложение Fastfetch в контейнере
```shell
apt-get update && apt-get install fastfetch
```

<img width="726" height="333" alt="изображение" src="https://github.com/user-attachments/assets/455a45a4-5369-4747-afed-3f004af27bdf" />


#### Запустить Fastfetch
```shell
fastfetch
```

<img width="720" height="335" alt="изображение" src="https://github.com/user-attachments/assets/4bd5db65-2a0d-4f2d-8811-fd0ccba3524c" />


##### Выйти из контейнера с Alt
```shell
exit
```

<img width="668" height="321" alt="изображение" src="https://github.com/user-attachments/assets/35a8ef05-40a5-4e02-96f6-2410dcccd254" />


### Полезные ссылки

[alt Docker Official Image](https://hub.docker.com/_/alt/)

[Dockerfile](https://github.com/alt-cloud/docker-brew-alt/blob/p10/x86_64/Dockerfile)

[Docker Alt Linux Image](https://github.com/sibsau/docker-alt/blob/master/README.md)

> Если вы обнаружили ошибку в этом тексте - сообщите пожалуйста автору!
