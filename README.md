# Vektorooo

Структура проекта такова:
```bash
.
├── all.yml
├── ansible.cfg
├── app.yml
├── firstrun.yml
├── inventory
│   ├── env.yml
│   └── hosts.yml
├── mon.yml
├── roles
│   ├── app
│   │   ├── files
│   │   │   └── public_keys
│   │   │       ├── adduser.pub
│   │   │       └── removeuser.pub
│   │   └── tasks
│   │       └── main.yml
│   ├── firstrun
│   │   └── tasks
│   │       └── main.yml
│   ├── mon
│   │   └── tasks
│   │       └── main.yml
│   └── sql
│       └── tasks
│           └── main.yml
└── sql.yml
```
 
Можно запустить весь проект через плейбук all.yml. Можно запускать отдельные плейбуки. Перед тем, как запустить плейбук в реальности, желатально проверить, что будет изменено при помощи ключей -CD. Ключ -b - для того, чтобы выполнить от имени sudoers. Пример команды запуска плейбука app.yml:

`ansible-playbook app.yml -CD`
