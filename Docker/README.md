# Домашняя работа "Оркестрация группой Docker контейнеров на примере Docker Compose." - 'Хамуро ИА'

### Задание 1
Так как DockerHub недоступен - я просто стянул нужный образ nginx и создал докер файл. После этого собрал его, что соответственно показано на скринах.
<img width="878" height="195" alt="Снимок экрана 2026-01-13 160449" src="https://github.com/user-attachments/assets/2da5cc73-d17c-4e51-a817-4a804c11ca94" />
<img width="1124" height="598" alt="Снимок экрана 2026-01-13 160431" src="https://github.com/user-attachments/assets/1ca0f69d-0183-43ac-92fa-4ed779e059b8" />

### Задание 2

<img width="1124" height="598" alt="Снимок экрана 2026-01-13 160431" src="https://github.com/user-attachments/assets/4d57284f-f3e1-46d7-8d3a-098f6f71c6e4" />
<img width="1119" height="427" alt="Снимок экрана 2026-01-13 160441" src="https://github.com/user-attachments/assets/f19b6499-dde7-42b6-8966-87f491d32313" />

### Задание 3
Почему остановился контейнер? Команда docker attach подключается к основному процессу конетейнера, с помощью сочетания клавиш Ctrl + C мы посылаем сигнал SIGINT, который останавливает основной процесс и контейнер останавливаться вместе с ним соответственно.
<img width="595" height="295" alt="Снимок экрана 2026-01-13 165047" src="https://github.com/user-attachments/assets/c7368541-6422-489d-808e-9b8999e94227" />

<img width="1072" height="454" alt="Снимок экрана 2026-01-13 165105" src="https://github.com/user-attachments/assets/1c4e4360-52c6-412e-b431-09deda655e24" />

<img width="490" height="226" alt="Снимок экрана 2026-01-13 163831" src="https://github.com/user-attachments/assets/7adc480f-2f0c-41f8-96ee-62d7e8981d40" />
<img width="710" height="446" alt="Снимок экрана 2026-01-13 165124" src="https://github.com/user-attachments/assets/8c83ee5d-4806-4627-8b2c-0bd3251e30f2" />

Nginx внутри контейнера теперь слушает порт 81, но Docker по-прежнему пробрасывает порт 8080 хоста на порт 80 контейнера (как было указано при запуске -p 127.0.0.1:8080:80). Поскольку nginx больше не слушает порт 80 в контейнере, соединение не может быть установлено.

### Задание 4
В этом задании было требование создать контейнер с образом Centos - но официальный образ я не смог стянуть с библиотки и в итоге вместо него стянул образ Убунту.
<img width="1011" height="121" alt="Снимок экрана 2026-01-14 165023" src="https://github.com/user-attachments/assets/fd1fac56-ddd7-4b75-bae8-a009575ff78e" />
<img width="994" height="412" alt="Снимок экрана 2026-01-14 165044" src="https://github.com/user-attachments/assets/23ee0e77-6234-40fd-900d-2538897ec5fa" />
<img width="1000" height="211" alt="Снимок экрана 2026-01-14 165102" src="https://github.com/user-attachments/assets/387b1267-7e28-4104-86fe-ce7a37bb7afb" />
<img width="600" height="336" alt="Снимок экрана 2026-01-14 165112" src="https://github.com/user-attachments/assets/d6f965c1-45ca-4520-a6d3-e11b4391ad83" />
<img width="488" height="285" alt="Снимок экрана 2026-01-14 165121" src="https://github.com/user-attachments/assets/fc9ae399-4231-4db6-b367-7bffe1114941" />



### Задание 5

