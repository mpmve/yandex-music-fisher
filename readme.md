# Yandex Music Fisher (1.7.1)

Расширение браузера для загрузки музыки с сервисов [Яндекс.Музыка](https://music.yandex.ru/)
и [Яндекс.Радио](https://radio.yandex.ru/).

Можно скачивать отдельные треки, плейлисты, альбомы и дискографии.
Расширение самостоятельно устанавливает ID3 тег (включая обложку).
При прерывании загрузки есть возможность возобновить её.

[Список изменений](https://github.com/egoroof/yandex-music-fisher/releases)

### Зеркала

При блокировке одного из репозиториев другие продолжат работать. Сейчас доступны:

- [GitHub](https://github.com/egoroof/yandex-music-fisher)
- [Bitbucket](https://bitbucket.org/egoroof/yandex-music-fisher)

### Требование

Необходим браузер на движке Chromium:
[Chrome](https://www.google.com/chrome) (рекомендуется, меньше всего проблем),
[Яндекс.Браузер](https://browser.yandex.ru),
[Opera](http://www.opera.com/) или подобный.

Лучше всегда обновлять браузер до последней версии, поскольку в новой версии могут быть устранены
неполадки, присущие старым версиям.

### Установка

[Скачайте архив по этой ссылке](https://github.com/egoroof/yandex-music-fisher/releases/download/v1.7.1/yandex-music-fisher_1.7.1.zip),
извлеките в текущую папку, откройте страницу расширений в браузере и перенесите туда мышкой извлечённую папку __yandex-music-fisher__,
после чего в браузере появится новое расширение:

![Установка](/publish/install.gif "Установка")

Обновляется расширение аналогичным способом.
Когда выйдет новая версия, расширение оповестит вас.

### Условия использования сервиса Яндекс.Музыка

Используя расширение Yandex Music Fisher (далее - Расширение), вы считаетесь принявшим [условиями использования сервиса Яндекс.Музыка](https://yandex.ru/legal/music_termsofuse/) (далее – Условия).
В случае несогласия с какими-либо из положений указанных в Условиях, вы не вправе использовать сервис Яндекс.Музыка.
Разработчики Расширения не несут ответственность за нарушения Условий, поэтому используйте Расширение на свой страх и риск.

### Как пользоваться

Откройте страницу на [Яндекс.Музыка](https://music.yandex.ru/) с нужным ![blue](/publish/blue.png) треком,
![yellow](/publish/yellow.png) альбомом или ![green](/publish/green.png) плейлистом - иконка изменит цвет в зависимости
от открытой страницы. Нажав на неё откроется всплывающее окно с информацией о загрузке и кнопкой для начала скачивания.

![Использование](/publish/usage.gif "Использование")

После нажатия на кнопку скачивания, загрузка появится на вкладке "Загрузки":

![Загрузки](/publish/loader.png)

Далее пойдёт автоматический процесс скачивания. Можно покинуть сайт Яндекс Музыки.
Кроме того, со страницы исполнителя можно скачать дискографию:

![Дискография](/publish/discography.png)

### Пути сохранения

- Все загрузки сохраняются в папку, которая указана в настройке браузера "__Расположение загружаемых файлов__".
- Для __дискографии__ создаётся отдельная папка с именем исполнителя, в которую сохраняются альбомы.
- Для __альбома__ / __плейлиста__ создаётся отдельная папка с именем исполнителя и названием альбома / плейлиста.
- Если __альбом__ состоит из нескольких дисков, то создаются соответствующие папки.

### Ограничения

Поскольку сервис Яндекс.Музыка позволяет слушать музыку только пользователям из России, Украины, Беларуси и
Казахстана, то и скачивать музыку с помощью этого расширения возможно только из этих стран.

С недавних пор сервис Яндекс.Музыка начал выводить капчу и таким способом противодействовать скачиванию треков.
При этом расширение покажет ошибку, а для дальнейшего скачивания нужно перейти на любую страницу Яндекс.Музыки и
ввести капчу. После чего можно возобновить скачивание через расширение.

### Сборка расширения (для опытных пользователей)

1. Устанавливаем [Node.js](https://nodejs.org/en/).
2. Устанавливаем зависимости: `npm install`
3. Собираем расширение: `npm run build`

Загружать распакованное расширение из папки `src`.
