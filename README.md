# Примеры вебхуков к телеграм боту с разными типами данных
## Навигация
[Текст](#текст)
[Изображение](#изображение)
[Голосовое сообщение](#голосовое-сообщение)
[Видео](#видео)
[Геолокация](#геолокация)
[Файл](#файл)
[Стикер](#стикер)
[Контакт](#контакт)
[Музыка](#музыка)
[Опрос](#опрос)
[Через inline бота](#через-inline-бота)




## Текст
```json
{
    "update_id": 123123123,
    "message": {
        "message_id": 303,
        "from": {
            "id": 12345678,
            "is_bot": false,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "language_code": "ru"
        },
        "chat": {
            "id": 12345678,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "type": "private"
        },
        "date": 1622109773,
        "text": "Simple text for "
    }
}
```
## Изображение
```json
{
    "update_id": 123123123,
    "message": {
        "message_id": 303,
        "from": {
            "id": 12345678,
            "is_bot": false,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "language_code": "ru"
        },
        "chat": {
            "id": 12345678,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "type": "private"
        },
        "date": 1622109773,
        "media_group_id": "12312312312312345", // если картинки были отправлены группой
        "photo": [
            {
                "file_id": "AgACAgIAAxkBAAIBN2CvcfQ2TNZCjwABb-GH4V4wEFsC0QACCLIxG--ceUkCu0bEH6mVrFVPqaIuAAMBAAMCAANtAAOAvAIAAR8E",
                "file_unique_id": "AQADVU-poi4AA4C8AgAB",
                "file_size": 15313,
                "width": 180,
                "height": 320
            },
            {
                "file_id": "AgACAgIAAxkBAAIBN2CvcfQ2TNZCjwABb-GH4V4wEFsC0QACCLIxG--ceUkCu0bEH6mVrFVPqaIuAAMBAAMCAAN4AAOBvAIAAR8E",
                "file_unique_id": "AQADVU-poi4AA4G8AgAB",
                "file_size": 61403,
                "width": 450,
                "height": 800
            },
            {
                "file_id": "AgACAgIAAxkBAAIBN2CvcfQ2TNZCjwABb-GH4V4wEFsC0QACCLIxG--ceUkCu0bEH6mVrFVPqaIuAAMBAAMCAAN5AAN-vAIAAR8E",
                "file_unique_id": "AQADVU-poi4AA368AgAB",
                "file_size": 97267,
                "width": 720,
                "height": 1280
            }
        ]
    }
}
```
## Голосовое сообщение
```json
{
    "update_id": 123123123,
    "message": {
        "message_id": 303,
        "from": {
            "id": 12345678,
            "is_bot": false,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "language_code": "ru"
        },
        "chat": {
            "id": 12345678,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "type": "private"
        },
        "date": 1622109773,
        "voice": {
            "duration": 2,
            "mime_type": "audio/ogg",
            "file_id": "AwACAgIAAxkBAAIBPWCvcyqUpO9-jCKjNjBOsYxXWwAB8AACjgsAAu-ceUl9EcYwhtngqB8E",
            "file_unique_id": "AgADjgsAAu-ceUk",
            "file_size": 6853
        }
    }
}
```
## Видео
```json
{
    "update_id": 123123123,
    "message": {
        "message_id": 303,
        "from": {
            "id": 12345678,
            "is_bot": false,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "language_code": "ru"
        },
        "chat": {
            "id": 12345678,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "type": "private"
        },
        "date": 1622109773,
        "video": {
            "duration": 3,
            "width": 720,
            "height": 1280,
            "mime_type": "video/mp4",
            "thumb": {
                "file_id": "AAMCAgADGQEAAgE_YK9z68avRNua2J88zq7ZYnT9E8AAApILAALvnHlJEZbqM1HSyM4mmbChLgADAQAHbQADAVsAAh8E",
                "file_unique_id": "AQADJpmwoS4AAwFbAAI",
                "file_size": 2945,
                "width": 180,
                "height": 320
            },
            "file_id": "BAACAgIAAxkBAAIBP2Cvc-vGr0TbmtifPM6u2WJ0_RPAAAKSCwAC75x5SRGW6jNR0sjOHwQ",
            "file_unique_id": "AgADkgsAAu-ceUk",
            "file_size": 1797033
        }
    }
}
```
## Геолокация
```json
{
    "update_id": 123123123,
    "message": {
        "message_id": 303,
        "from": {
            "id": 12345678,
            "is_bot": false,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "language_code": "ru"
        },
        "chat": {
            "id": 12345678,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "type": "private"
        },
        "date": 1622109773,
        "location": {
            "latitude": 61.647763,
            "longitude": 50.816596
        }
    }
}
```
## Файл
```json
{
    "update_id": 123123123,
    "message": {
        "message_id": 303,
        "from": {
            "id": 12345678,
            "is_bot": false,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "language_code": "ru"
        },
        "chat": {
            "id": 12345678,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "type": "private"
        },
        "date": 1622109773,
        "document": {
            "file_name": "example.txt",
            "mime_type": "text/plain",
            "file_id": "BQACAgIAAxkBAAIBRWCvdqnX-zOBeB0kYc7NTX1lc0H-AAKZCwAC75x5STemD_BSAw5vHwQ",
            "file_unique_id": "AgADmQsAAu-ceUk",
            "file_size": 7
        },
        "caption": "Example" // если подпись была задана
    }
}
```
## Стикер
```json
{
    "update_id": 123123123,
    "message": {
        "message_id": 303,
        "from": {
            "id": 12345678,
            "is_bot": false,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "language_code": "ru"
        },
        "chat": {
            "id": 12345678,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "type": "private"
        },
        "date": 1622109773,
        "sticker": {
            "width": 512,
            "height": 512,
            "emoji": "\ud83c\udde6\ud83c\uddfa",
            "set_name": "prtyparrot",
            "is_animated": true,
            "thumb": {
                "file_id": "AAMCAgADGQEAAgEvYK9uTRlNGWwU2GS8GAElGtBjkJ4AArgAA8D7CAABTZJJmN-xlI7y8sAPAAQBAAdtAAM6TQACHwQ",
                "file_unique_id": "AQAD8vLADwAEOk0AAg",
                "file_size": 2634,
                "width": 128,
                "height": 128
            },
            "file_id": "CAACAgIAAxkBAAIBL2Cvbk0ZTRlsFNhkvBgBJRrQY5CeAAK4AAPA-wgAAU2SSZjfsZSOHwQ",
            "file_unique_id": "AgADuAADwPsIAAE",
            "file_size": 3279
        }
    }
}
```
## Контакт
```json
{
    "update_id": 123123123,
    "message": {
        "message_id": 303,
        "from": {
            "id": 12345678,
            "is_bot": false,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "language_code": "ru"
        },
        "chat": {
            "id": 12345678,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "type": "private"
        },
        "date": 1622109773,
        "contact": {
            "phone_number": "+77777777777",
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "vcard": "BEGIN:VCARD\nVERSION:3.0\nFN:Ivan Rybintsev\nTEL;MOBILE:+77777777777\nEND:VCARD",
            "user_id": 12345678
        }
    }
}
```
## Музыка
```json
{
    "update_id": 123123123,
    "message": {
        "message_id": 303,
        "from": {
            "id": 12345678,
            "is_bot": false,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "language_code": "ru"
        },
        "chat": {
            "id": 12345678,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "type": "private"
        },
        "date": 1622109773,
        "audio": {
            "duration": 198,
            "file_name": "Смысловые_галлюцинации_Вечно_молодой.mp3",
            "mime_type": "audio/mp3",
            "title": "Смысловые_галлюцинации_Вечно_молодой",
            "performer": "<unknown>",
            "file_id": "CQACAgIAAxkBAAIBSWCveLv1rDVHGHhmQXkkN8tVDL1RAAKdCwAC75x5Sd9sSf2NjkxbHwQ",
            "file_unique_id": "AgADnQsAAu-ceUk",
            "file_size": 3173283
        },
        "caption": "Example" // если подпись была задана
    }
}
```
## Опрос
```json
{
    "update_id": 123123123,
    "message": {
        "message_id": 303,
        "from": {
            "id": 12345678,
            "is_bot": false,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "language_code": "ru"
        },
        "chat": {
            "id": 12345678,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "type": "private"
        },
        "date": 1622109773,
        "poll": {
            "id": "1231231231231231234",
            "question": "Example",
            "options": [
                {
                    "text": "Answer 1",
                    "voter_count": 0
                },
                {
                    "text": "Answer 2",
                    "voter_count": 0
                }
            ],
            "total_voter_count": 0,
            "is_closed": false,
            "is_anonymous": true,
            "type": "quiz",
            "allows_multiple_answers": false,
            "correct_option_id": 0
        }
    }
}
```
## Через inline бота
```json
{
    "update_id": 123123123,
    "message": {
        "message_id": 303,
        "from": {
            "id": 12345678,
            "is_bot": false,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "language_code": "ru"
        },
        "chat": {
            "id": 12345678,
            "first_name": "Ivan",
            "last_name": "Rybintsev",
            "username": "irybintsev",
            "type": "private"
        },
        "date": 1622109773,
        "animation": {
            "file_name": "mp4.mp4",
            "mime_type": "video/mp4",
            "duration": 6,
            "width": 132,
            "height": 164,
            "file_id": "CgACAgQAAxkBAAIBTWCvewSHth-7EMlYQNqB3TMmQXMfAAJ3AgACVrsNUETo8ZdbM9TFHwQ",
            "file_unique_id": "AgADdwIAAla7DVA",
            "file_size": 130423
        },
        "document": {
            "file_name": "mp4.mp4",
            "mime_type": "video/mp4",
            "file_id": "CgACAgQAAxkBAAIBTWCvewSHth-7EMlYQNqB3TMmQXMfAAJ3AgACVrsNUETo8ZdbM9TFHwQ",
            "file_unique_id": "AgADdwIAAla7DVA",
            "file_size": 130423
        },
        "via_bot": {
            "id": 140267078,
            "is_bot": true,
            "first_name": "Tenor GIF Search",
            "username": "gif"
        }
    }
}
```
