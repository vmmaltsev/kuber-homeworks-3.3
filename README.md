# Домашнее задание к занятию «Как работает сеть в K8s» - `Мальцев Виктор`

---

Задание 1. Создать сетевую политику или несколько политик для обеспечения доступа

    1. Создать deployment'ы приложений frontend, backend и cache и соответсвующие сервисы.
    2. В качестве образа использовать network-multitool.
    3. Разместить поды в namespace App.
    4. Создать политики, чтобы обеспечить доступ frontend -> backend -> cache. Другие виды подключений должны быть запрещены.
    5. Продемонстрировать, что трафик разрешён и запрещён.

Ответ:

Deployment в namespace app

![alt text](https://github.com/vmmaltsev/screenshot/blob/main/Screenshot_154.png)

Трафик с frontend на backend разрешён

![alt text](https://github.com/vmmaltsev/screenshot/blob/main/Screenshot_155.png)

Трафик с backend на cache разрешён

![alt text](https://github.com/vmmaltsev/screenshot/blob/main/Screenshot_156.png)

Трафик с frontend на cache запрещён

![alt text](https://github.com/vmmaltsev/screenshot/blob/main/Screenshot_157.png)

Трафик с cache на backend запрещен

![alt text](https://github.com/vmmaltsev/screenshot/blob/main/Screenshot_158.png)