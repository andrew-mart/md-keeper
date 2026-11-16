# md-keeper

**[Русский](#русский) · [English](#english)**

## Русский

md-keeper — локальная коллекция документов с полнотекстовым и смысловым поиском для Windows и Linux.

Markdown, текст, CSV, HTML, Word и PDF остаются там, где лежат: в коллекцию попадают путь, название и текст для поиска.
Модель смыслового поиска работает внутри программы, сеть для работы не нужна. Наружу текст уходит только в одном
случае и только с вашего согласия — когда md-keeper просит Claude придумать заголовок документу без заголовка.

Скачать — в разделе [Releases](../../releases/latest).

### Windows 10 и 11 (x64)

Запустите `md-keeper_X.Y.Z_x64-setup.exe`. Права администратора не нужны: программа ставится для текущего
пользователя в `%LOCALAPPDATA%\Programs\md-keeper`, данные по умолчанию — в `%LOCALAPPDATA%\md-keeper\data`, другую
папку можно выбрать при установке.

Установщик пока не подписан, поэтому Windows может показать окно «Windows защитила ваш компьютер». Нажмите
«Подробнее», затем «Выполнить в любом случае». Проверить, что файл тот самый, можно по сумме из `SHA256SUMS`:

```
certutil -hashfile md-keeper_X.Y.Z_x64-setup.exe SHA256
```

### Linux (x86_64, Ubuntu 22.04 и новее)

```
sudo apt install ./md-keeper_X.Y.Z_amd64.deb
```

apt подтянет WebKitGTK, GTK и библиотеку значков трея. Данные — в `~/.local/share/md-keeper/data`.

### Лицензии

Тексты лицензий стороннего кода, модели и библиотек, которые входят в программу, лежат рядом с ней: на Windows — в
папке программы, на Linux — в `/usr/share/doc/md-keeper/THIRD-PARTY-NOTICES.txt`.

© Andrei Martyshchenko. Все права защищены. Исходный код программы закрыт.

## English

md-keeper is a local collection of documents with full-text and semantic search, for Windows and Linux.

Markdown, text, CSV, HTML, Word and PDF files stay where they are: the collection keeps their path, title and
searchable text. The semantic search model runs inside the program, so it needs no network to work. Text leaves your
computer in one case only and only with your consent — when md-keeper asks Claude to title an untitled document.

Download it from [Releases](../../releases/latest).

### Windows 10 and 11 (x64)

Run `md-keeper_X.Y.Z_x64-setup.exe`. No administrator rights are needed: the program is installed for the current user
in `%LOCALAPPDATA%\Programs\md-keeper`, its data goes to `%LOCALAPPDATA%\md-keeper\data` unless you pick another folder
during setup.

The installer is not signed yet, so Windows may say "Windows protected your PC". Click "More info", then "Run anyway".
To check the file is the right one, compare its sum with `SHA256SUMS`:

```
certutil -hashfile md-keeper_X.Y.Z_x64-setup.exe SHA256
```

### Linux (x86_64, Ubuntu 22.04 or newer)

```
sudo apt install ./md-keeper_X.Y.Z_amd64.deb
```

apt brings in WebKitGTK, GTK and the tray icon library. The data goes to `~/.local/share/md-keeper/data`.

### Licenses

The licenses of the third-party code, model and libraries included in the program are next to it: in the program
folder on Windows, in `/usr/share/doc/md-keeper/THIRD-PARTY-NOTICES.txt` on Linux.

© Andrei Martyshchenko. All rights reserved. The program's source code is closed.
