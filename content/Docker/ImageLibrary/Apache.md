## Apache

> Никогда в разработке не используйте русские имена файлов и каталогов!

> Никогда в разработке не используйте пробелы и спец.символы в именах файлов и каталогов!

Выполните все этапы работы с проектом по примеру с [Nginx](/content/Docker/ImageLibrary/Nginx.md)

Получить образ, создать и запустить контейнер:
```shell
docker run -d --name my-apache -p 8081:80 httpd
```

<img width="531" height="34" alt="изображение" src="https://github.com/user-attachments/assets/0ef40462-e6f6-4a48-b8ff-fd92b8492c0b" />


[Откройте адрес http://localhost:8081 в браузере](http://localhost:8081)

### Редактирование веб-страницы

Зайти в контейнер
```shell
docker exec -it my-apache bash
```

<img width="332" height="40" alt="изображение" src="https://github.com/user-attachments/assets/d0543361-ed45-405c-82c3-86ffd684355a" />


Установить текстовый редактор командной строки Micro:
```shell
apt update && apt install -y micro
```

<img width="708" height="737" alt="изображение" src="https://github.com/user-attachments/assets/da27eea8-9798-419a-a7ab-f87ac9380ab9" />


Открыть файл `index.html` для редактирования содержимого
```shell
micro /usr/local/apache2/htdocs/index.html
```

<img width="704" height="336" alt="изображение" src="https://github.com/user-attachments/assets/88d1f9e8-51b4-4b82-b4b5-b9c49ba4b7dc" />



> Чтобы в веб-странице поддерживался русский язык, вставьте тэг `<meta charset="UTF-8">`

отредайтируйте и сохраните по `Ctrl+S` и выйти из режима редактирования по `Ctrl+Q` или `F10`

<img width="652" height="169" alt="изображение" src="https://github.com/user-attachments/assets/66daaa3a-7062-4d99-be2b-dd9f2716afd0" />


<img width="371" height="70" alt="изображение" src="https://github.com/user-attachments/assets/637a025d-0689-4c25-99f0-79236ba4d03d" />



[Проверьте результат по адрес http://localhost:8081](http://localhost:8081)

Выйти из контейнера:
```shell
exit
```

<img width="453" height="57" alt="изображение" src="https://github.com/user-attachments/assets/0aec20e8-d1d3-49ba-89e7-3da88cb7fc84" />


> Если вы обнаружили ошибку в этом тексте - сообщите пожалуйста автору!
