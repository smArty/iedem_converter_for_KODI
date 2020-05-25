# Конвертер [iedem](https://iedem.tv/welcome/register/01659c3a2c7e8531) плейлиста для KODI

### Инструкция
1. Скачать проект и разархивировать
2. Открыть текстовым редактором (к примеру Notepad++) iedem_converter.py
3. В строке
`url = 'http://iedem.tv/playlists/uplist/your_id/playlist.m3u8'`
ссылку заменить на свою
4. В строке `if d['group-title'] not in ['Հայկական', 'українські', 'беларускія', 'azərbaycan', 'ქართული', 'точик', 'moldovenească', 'türk', 'o\'zbek`', 'ישראלי']:
во второй квадратной скобке указываем группы через запятую, которые необходимо исключить
5. Сохранить изменения
6. Открыть текстовым редактором (к примеру Notepad++) favorites.txt
7. Добавить свои каналы, которые хотите, чтобы они были в начале списка (фишка типа избранных). Каждый канал должен быть в отдельной строке без лишних пробелов и символов по бокам
7.1. Где же получить полный список каналов с правильными названиями?
7.2. 
8. Сохранить изменения
9. Запустить iedem_converter.py
10. Если все ОК, то рядом должен появиться файл-плейлист (к примеру iedemtv_20200525185347.m3u8), который необходимо указать в KODI

10.1. EPG и логотипы лучше всего использовать http://epg.it999.ru/epg.xml.gz

P.S. вероятно может потребоваться модуль **requests**. Устанавливаем его с помощью команды
`pip install requests`

Также, можно воспользоваться веб-интерфейсом http://tv.sdckz.com

### Получится примерно так
![](https://github.com/daradan/img/blob/master/kodi.jpg?raw=true)
