### Описание

Дискорд бот, личный кабинет, написанный на python3, имеющий возможность установки скина и плаща, стандартные возможности лк такие, как смена ника, пароля, регистрация, а также легкость добавления других возможностей. Идентификация пользователя происходит по его Discord ID, то есть пароль используется только для входа в лаунчер, смена ника, скина и плаща происходит прямо в дс без ввода пароля.

### Установка и настройка

Перед тем, как установить этого бота необходимо установить [Gravit Launcher](https://launcher.gravit.pro/install/#настроика-хостинга "Gravit Launcher Wiki") и настроить его на работу с MySQL.

- Получите токен бота [здесь](https://discord.com/developers/applications "Discord Developer Portal"), создайте приложение, в нём бота, нажмите Reset Token, потом Copy, сохраните этот токен.

- Установите python3 `apt install -y python3, python3-pip`.

- Создайте пользователя для бота командой `useradd -m -G www-data -s /bin/bash authbot`
и перейдите в него `su - authbot`

- Склонируйте репозиторий с ботом `git clone -b dev https://github.com/timoxa0/SDLB-Gravit`

- Настройте конфиг бота `config.py`

- Сделайте стартеры запускаемыми `chmod +x {start.sh,startscreen.sh}`

- Запуск бота для теста `./start.sh`, на постоянку `./startscreen.sh`