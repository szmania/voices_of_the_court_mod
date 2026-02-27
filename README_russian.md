# Часто задаваемые вопросы

## 1. Диалоговое окно не появляется
Этот мод требует дополнительную фоновую программу для работы. Скачайте локализованную фоновую программу здесь: [https://github.com/szmania/Voices_of_the_Court/releases/latest](https://github.com/szmania/Voices_of_the_Court/releases/latest). Скачанный .exe файл установится автоматически при открытии.

## 2. Проблемы с настройкой API
Рекомендуется использовать официальный DeepSeek API. В выпадающем меню для подключения модели диалога выберите страницу `custom(openai-compatible)` для настройки:
- URL сервера: `https://api.deepseek.com/beta`
- API ключ: Введите ваш собственный API ключ, который можно получить на [https://platform.deepseek.com](https://platform.deepseek.com).

OpenAI и OpenRouter также должны быть совместимы.

## 3. Диалоговое окно не появляется, даже когда фоновая программа запущена после установки
**Решение**: Вы должны использовать локализационный мод.

Способы установки (выберите один):
1. После извлечения скачанных файлов локализационного мода, перезапишите оригинальные файлы мода в директории Steam Workshop напрямую.
2. Поместите извлечённую папку мода `voices_of_the_court_mod-1.2.1-beta` в папку модов игры. Затем используйте Блокнот, чтобы создать новый файл с именем `voices_of_the_court_mod-1.2.1-beta.mod` в папке `Documents\Paradox Interactive\Crusader Kings III\mod` со следующим содержимым:
version="1.0"
tags={
"Gameplay"
}
name="Voices of the Court mcc"
supported_version="1.13.1"
path="C:/Users/ [Ваше имя пользователя ПК здесь] / Documents/Paradox Interactive/Crusader Kings III/mod/voices_of_the_court_mod-1.2.1-beta"

Если диалоговое окно всё ещё не появляется после установки и включения локализационного мода, путь к папке пользователя CK3 может быть установлен неправильно, или игра может быть в режиме Ironman. Этот мод не работает в режиме Ironman.

## 4. Ошибка "TypeError: Cannot read properties of undefined (reading 'playerID')" с красным текстом при открытии окна чата
**Решение**: Создайте папку с именем `run` в `Documents\Paradox Interactive\Crusader Kings III`. Войдите в эту папку и создайте текстовый файл с именем `votc.txt`.

## 5. Недавние воспоминания не читаются при разговоре с персонажами
**Решение**:
1. Это небольшая ошибка в оригинальной фоновой программе автора; скачивание локализованной фоновой программы решает эту проблему.
2. Это также может быть из-за ограничений токенов памяти. Настройте размер `max memory tokens` на странице настроек фоновой программы. После настройки токенов памяти вы также должны увеличить `max new tokens`; лучше, если `max new tokens` будет больше, чем `max memory tokens`.

## 6. Скрипт генерации промпта сбрасывается после перезапуска фоновой программы
**Решение**:
Сохраните его как отдельный файл в папке `custom`.

Mod Name: Voices of the Court - Community Edition
License: GNU General Public License v3.0 (GPLv3)

Credits & Attribution
This project is a derivative work based on VOTC / AliChat. We would like to extend our deep gratitude to the developers who kept this project alive and pushed the boundaries of AI in Crusader Kings III:

Original Creators: The VOTC Team and community contributors.

Continued Development: Special thanks to the Chinese development community, including Lisiyuan233, zhaowendao2005, and others who provided critical updates and support.

Community Support: Thanks to Durond and MrAndroPC and the broader community for their insights and historical context regarding the project.

Licensing Information
Some of original source material for this mod was released under the Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0) license.

In accordance with Section 4(b) of the CC BY-SA 4.0 license, this derivative work is being licensed under a BY-SA Compatible License: the GNU General Public License v3.0 (GPLv3).

Original License: CC BY-SA 4.0

Current License: GPLv3
