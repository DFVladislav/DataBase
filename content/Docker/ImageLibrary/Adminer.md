## Adminer (альтернатива phpMyAdmin)

Запуск Adminer для управления БД

Выполните все этапы работы с проектом по примеру с [Nginx](/content/Docker/ImageLibrary/Nginx.md)

> Никогда в разработке не используйте русские имена файлов и каталогов!

> Никогда в разработке не используйте пробелы и спец.символы в именах файлов и каталогов!

> Перед созданием проекта убедитесь, что порт 8084 не занят другим приложением!


Запустите **Adminer** в **Windows Powershell**
```shell
docker run -d `
  --name adminer `
  -p 8084:8080 `
  adminer:latest
```

Запустите **Adminer** в **Git-Bash/Linux/WSL 2.0/Mac**
```shell
docker run -d \
  --name adminer \
  -p 8084:8080 \
  adminer:latest
```

<img width="1078" height="552" alt="изображение" src="https://github.com/user-attachments/assets/d6f5cab2-4277-472c-a098-1f8b9005c9bd" />


[Откройте: http://localhost:8084](http://localhost:8084)

<img width="771" height="330" alt="изображение" src="https://github.com/user-attachments/assets/4f3f15c4-ecfa-49cb-9fc9-7760a0bd9853" />



> Без отдельно запущенного контейнера с БД PostgreSQL и связи с ним админ-панель работаеть не будет!

> Заполнять данные админ-панели не нужно!

Система:
- PostgreSQL
- сервер: host.docker.internal
- логин: postgres
- пароль: mysecretpassword

> Если вы обнаружили ошибку в этом тексте - сообщите пожалуйста автору!
