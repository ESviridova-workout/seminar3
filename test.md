> Файл создан для касания по работе с удаленным репозиторием
**********

# Работа с githab
1. Создаем папку и открываем ее в VS Code
2. В githab создаем новый репозиторий. Сохраняем ссылку репозитория
3. Переходим в VS Code и через команду git clone <адресс сылки> клонируем репозиторий в локальный
4. Открываем терминал в этом репозитории. Для этого в терминале прописываем консольную команду cd <имя папки>
5. Создаем файл с расширением и сохраняем его
6. Работаем в файле, сохраняем
7. Возвращаем это репозиторий с изменениями назад в удаленный в githab командой git push
8. Если вносили изменения в githab и потом решили опять отправить репозиторий на локальный, то нужно....
9. Перейти в VS Code и набраить в терминале команду git pull
10. Git pull - составная команда. При переносе может возникнуть конфликт, если информация в локальном и удаленном будет координально отличаться

## Создание конфликта при сливании репозиториев
1. Склонируем еще раз репозиторий из githab в локальный для этого ...
2. В VS Code в адресную строку введем команду git clone <ссылка репозитория> (или найдем эту команду через перемещение стрелки вверх - вводили ее раньше, при первом клонировании) + вконце команды введем новое имя для папки
3. Появившаяся папка - полная копия уже существующей, только с другим названием
4. В текущей папке внесем изменения и сохраним их.
5. Отправим папку в githab командой git push
4. Переместим терминал в новую склонированную папку через консольную команду:
    * вначале cd .. - эта команда перенесет нас в корневую попку, чтобы уже из нее попасть в нужную нам
    * потом cd <имя нужной папки>
5. Откроем в этой папке файл и внесем в него координальные изменения. К примеру в первую строоку впишем номер телефона или что-то тому подобное
6. Сохраним изменения
7. Отправим эту папку в githab (там есть предыдущий репозиторий) командой git push
8. В терминале отобразится конфликт. Нам предлагают в текущий локальный репозиторий то, что есть в githab - командой git pull
9. И разрешить конфликт в локальном репозитории
10. Мы видим обычный конфликт как при слиянии веток. Решается он аналогично
11. Решаем конфликт и сохраняем и уже после этого отправляем в githab командой git push
