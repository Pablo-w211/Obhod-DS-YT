# discord-un

# Discord Unlock XNBO (обход блокировки Discord'а и Youtube'а)

> [!NOTE]  
> Данный репозиторий - **некоммерческая** *User-Friendly* сборка [оригинального репозитория](https://github.com/bol-van/zapret). Здесь используются оригинальные бинарники, сравнить которые вы можете с помощью хэша. \
Так как discord-un open-source, вы всегда можете сами собрать эти бинарники и не бояться вирусов. \

##

> [!CAUTION]  
> **Многие антивирусники** в данный момент жалуются на ***HackTool/RiskTool*** и ***WinDivert*** - это нормальное поведение, так как программа изменяет сетевые пакеты. Что с этим делать? Собрать бинарники самому из исходников, довериться уже собранным, либо не использовать вовсе.

## Guides
### Windows
> [!IMPORTANT]  
> Если всё еще не скачан, то скачайте последний [релиз](https://github.com/XINBOSHIN/discord-un/releases), разархивируйте в отдельную папку.

Запустите **от имени администратора** то, что вам нужно:
- **`discord.bat`** - запустить обход дискорда.
- **`general.bat`** - запустить обход дискорда и ютуба.
  * Если обход не работает, пробуйте по порядку **`general (ALT ..).bat`** (также можете проверить стратегию на **МГТС**)
###
- **`service_install.bat`** - установить на автозапуск (в сервисы) любую стратегию из этого репозитория (стратегия **НЕ** должна начинаться со слова `service`)
###
- **`service_goodbye_discord.bat`** - запустить, если вы используете **СЕРВИС goodbyedpi**, и хотите, чтобы zapret обходил **только discord**.
  * **ВНИМАНИЕ**: Запускать ПОСЛЕ создания сервиса goodbyedpi. Первый раз goodbyedpi может вылететь - просто перезапустите устройство!
###
- **`service_remove.bat`** - остановить и удалить сервисы выше

## Решение проблем

- Проверьте, запускаете ли вы файлы от **ИМЕНИ АДМИНИСТРАТОРА**
- Не запускаются bat файлы? Попробуйте запустить **`service_remove.bat`** от **ИМЕНИ АДМИНИСТРАТОРА**
  * Также отключите программы, которые могут мешать созданию сервиса *(Антивирусы, клинеры с доп. защитой)*.

##
- Не работает вместе с **VPN**? Отключите функцию **TUN** (Tunneling) в настройках VPN.
- Не работает **`service_goodbye_discord`**? Удостовертесь, что сервис goodbyedpi запущен и имеет название GoodbyeDPI. После снова запустите `service_goodbye_discord.bat` и перезапустите устройство.
- Попробуйте обновить бинарники с оригинального репозитория.

### Остановка и удаление обхода
Для этого запустите **`service_remove.bat`**.
- Если WinDivert так и не удалился, узнайте его название с помощью команды `driverquery | find "Divert"` в cmd, а затем удалите данными командами (заместо WinDivert введите название, которые вы узнали):
```
sc stop WinDivert
sc delete WinDivert
```

### Добавление дополнительных адресов заблокированных сайтов 
- Список можно дополнить используя `list-general.txt` (для файлов `general`) и в список `list-discord` (для файлов `discord`).
> [!IMPORTANT]  
> После добавления сервис нужно перезапустить.

## Linux
В оригинальном репозитории [zapret](https://github.com/bol-van/zapret/) имеется достаточно информации для того, чтобы начать пользоваться обходом блокировок, но и стоит понимать, что нажатием одной кнопки ничего не заработает. \
Достаточно следовать следующим инструкциям и всё внимательно читать:
- [zapret/docs/quick_start.txt](https://github.com/bol-van/zapret/blob/master/docs/quick_start.txt)
- [zapret/docs/readme.txt](https://github.com/bol-van/zapret/blob/master/docs/readme.txt)
  * 
> [!WARNING]
> Если вы открываете Issue *(в этом репозитории)* с проблемой в использовании на **Linux**, то, как бы это не звучало, это ошибка. Все вопросы по работе на Linux нужно открывать в **[ОРИГИНАЛЬНОМ](https://github.com/bol-van/zapret/)** репозитории. Следовательно, задавайте вопросы [тут](https://github.com/XINBOSHIN/discord-un/issues/).

## Support

Вы можете поддержать проект, поставив :star: (сверху справа репозитория)!  
Также, вы можете поддержать разработчика [оригинального репозитория zapret](https://github.com/bol-van/zapret/issues/590) тут - https://github.com/bol-van/zapret/issues/590

<a href="https://star-history.com/#Flowseal/zapret-discord-youtube&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=Flowseal/zapret-discord-youtube&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=Flowseal/zapret-discord-youtube&type=Date" />
   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=Flowseal/zapret-discord-youtube&type=Date" />
 </picture>
</a>

