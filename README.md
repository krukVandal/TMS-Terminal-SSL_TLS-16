# 1. Установить и настроить SSL-сертификат
  - Установил openssl
  - Создал папку /etc/ssl/keys
  - Сгенерировал самоподписанный сертификат sudo openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout /etc/ssl/keys/priv.key -out /etc/ssl/keys/cert.crt
  - Заполнил данные сертификата
  - Добавил сертификат и ключ в конфиг nginx, добавил переадресацию с http на https
  - Скриншот данных сертификата из firefox
  - Еще столкнулся с проблемой если поставить пароль на сертификат то демон не поднимается

<img width="1143" height="680" alt="image" src="https://github.com/user-attachments/assets/a70003a2-8693-4e7a-a1c9-f8720ff18ad7" />

<img width="806" height="668" alt="image" src="https://github.com/user-attachments/assets/20d91260-2159-4f28-a12d-c01295f4c4f5" />

<img width="806" height="668" alt="image" src="https://github.com/user-attachments/assets/cce4db4b-ef15-413a-8c0c-d98fad392e99" />

# 2. Провести нагрузочный тест на свой веб-сервер
  - Установил apache2-utils
  - Тест проводил с помощью команды ab

 <img width="1143" height="680" alt="image" src="https://github.com/user-attachments/assets/45d6b08f-29d2-4ef7-90c1-890435950977" />

 <img width="1143" height="680" alt="image" src="https://github.com/user-attachments/assets/6d6e47b4-507c-493b-84a2-97fba3afb0e4" />

 <img width="1143" height="680" alt="image" src="https://github.com/user-attachments/assets/486834a6-8d17-4f2c-acde-40df03d8ca7b" />


 
