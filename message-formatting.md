ХАЗАХХВЗАЗАЗАЗАЗ ЛОШКИ СОСАТЬ НА ЛЕВО ЕБАТЬ НА ПРАВО
ДЕЛАТЬ МИНЕТ ЧЕРЕЗ ПЛЕЧО 







# Форматирование приветственного сообщения

### Список доступных переменных и их вариантов (через запятую)
Для удобства пользователей было придумано несколько вариантов написания.
```
ID: $id
Ник пользователя: $display_name, $username, $nickname, $nick, $name
Тэг пользователя: $discriminator, $numbers, $number, $tag
Упоминание (пинг) пользователя: $highlight, $mention, $ping
Ссылка на аватар пользователя: $avatar_url, $avatar_uri, $avatar

Ник владельца сервера: $owner_display_name, $owner_username, $owner_nickname, $owner_nick, $owner_name
Тэг владельца сервера: $owner_discriminator, $owner_numbers, $owner_number, $owner_tag
Упоминание (пинг) владельца сервера: $owner_highlight, $owner_mention, $owner_ping
Ссылка на аватар владельца сервера: $owner_avatar_url, $owner_avatar_uri, $owner_avatar

Дата регистрации: $registered_at, $register_date, $account_date, $registered, $date
Название сервера: $server, $guild
Количество участников: $members_count, $users_count, $members, $users
Ссылка на иконку сервера: $server_avatar, $guild_avatar
Дата создания сервера: $server_created_at, $guild_created_at, $server_created, $guild_created, $server_date, $guild_date
```


### Демонстрация
Так-же для демонстрации мы сделали тестовый Embed, чтобы каждый смог поиграться с параметрами и настроить всё под себя
```
{
  "color": 1867221,
  "author": {
    "name": "Новенький на сервере - $name#$discriminator!",
    "icon_url": "$avatar"
  },
  "title": "Привет(крадьётся)!",
  "description": "Приветствуем, $mention на сервере **$guild**! У нас уже **$members** участников! Ура! 🎉\n\nНаш сервер был создан **$guild_created_at** для предоставления помощи и распространения информации о обновлениях **Куро бота**!\n\nЕсли у тебя возникли какие-то вопросы - смело задавай их в канале <#579050667423956992> или лично разработчику $owner_mention!",
  "image": {
    "url": "https://media1.tenor.com/images/7824a17c74ce291778ddf6de2ac542b9/tenor.gif?itemid=5673986"
  },
  "footer": {
    "text": "ID: $id | Зарегистрировался: $register_date",
    "icon_url": "$guild_avatar"
  }
}
```

![Превью сообщения](https://github.com/KrykiZZ/Kuro-Bot/blob/master/welcome_preview.png)
