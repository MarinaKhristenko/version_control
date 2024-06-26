# **Подсказка по GIT**

## Основные команды 

Работая с GIT, разработчики используют определенные команды для копирования, создания, изменения и объединения кода. Эти команды можно выполнять непосредственно из командной строки или с помощью приложения, например GitHub Desktop. Ниже приведены некоторые распространенные команды для работы с GIT.

### Команды GIT: 
```sh
git init
```
Инициализирует новый репозиторий GIT и начинает отслеживание существующего каталога. В существующий каталог добавляется скрытая вложенная папка, в которой размещается внутренняя структура данных, необходимая для управления версиями.
```sh
git add
```
Подготавливает изменение. GIT отслеживает изменения в базе кода разработчика, но для включения изменений в журнал проекта необходимо подготавливать их и создавать моментальные снимки. Эта команда выполняет первую часть этого двухэтапного процесса, то есть подготовку. Все подготовленные изменения станут частью следующего моментального снимка и журнала проекта. Раздельные подготовка и фиксация дают разработчикам полный контроль над историей проекта без необходимости изменять подход к написанию кода и работе в целом.
```sh
git commit -m "Message text"
```
Cохраняет моментальный снимок в журнале проекта и завершает процесс отслеживания изменений. Иначе говоря, фиксация похожа на создание фотографии. Все, что было подготовлено с помощью команды *git add*, станет частью моментального снимка при использовании *git commit*.
```sh
git status
```
Выводит состояние изменений: не отслеживаются, изменены или подготовлены.
```sh
git log
```
Отображает отправленные снимки состояния и позволяет просматривать и фильтровать историю проекта, а также искать в ней конкретные изменения.
```sh
git log --oneline
```
Записывает каждый коммит в одну строку. По умолчанию отображаются только идентификаторы коммитов и первые строки комментариев к ним.
```sh
git log --oneline --graph
```
Используется для построения диаграммы из символов ASCII, отражающей структуру веток в истории коммитов.
```sh
git checkout <имя_ветки>
```
Используется для переключения веток и выгрузки их содержимого в рабочий каталог.
```sh
git diff
```
Представляет собой многоцелевую команду Git, которая инициирует функцию сравнения источников данных Git — коммитов, веток, файлов и т.п.
```sh
git branch
```

Позволяет создавать, просматривать, переименовывать и удалять ветки. Отображение всех веток.
```sh
git branch <имя_ветки>
```
Создание новой ветки.
```sh 
git branch -d <имя_ветки>
```
Удаление ветки.
```sh
git merge
```
Команда *git merge* выполняет слияние отдельных направлений разработки (веток), созданных с помощью команды *git branch*, в единую ветку.
```sh
git restore
```
Это команда, которая позволяет восстановить измененные или удаленные файлы в рабочей директории до их предыдущего состояния в Git репозитории.

## **Работа с удаленными репозиториями**

```sh
git push
```
Создана для управления удаленными репозиториями. Она необходима, когда вы хотите поделиться изменениями с другими участниками проекта или сохранить их в центральном репозитории.
```sh
git pull
```
Используется для извлечения и загрузки содержимого из удаленного репозитория и немедленного обновления локального репозитория этим содержимым.
```sh
git clone
```
Копирует существующий репозиторий Git.
```sh
git remote
```
Служит для управления списком удалённых репозиториев. Она позволяет сохранять длинные URL репозиториев в виде понятных коротких строк, например «origin».
```sh
git pull request
 ```
 Это запрос на вливание изменений из вашей ветки в основную ветку исходного репозитория. Таким образом они попадут к хозяевам проекта. Чтобы создать *Pull Request*, зайдём на страницу вашего форка. Справа от выпадающего меню с выбором ветки есть кнопка «New pull request».

__*Инструкция по выгрузке и загрузке данных:*__ 

1. Создать аккаунт на Github.com
2. Создать локальный репозитрий.
3. "Подружить" локальный и удаленный репозиторий. Github про создании нового репозитория подскажет, как это сделать.
4. Отправить (*push*) локальный репозиторий на удаленный (Github), при этом, возможно, нужно будет авторизоваться на удаленном репозитории.
5. Провести измение с "другого компьютера".
6. Выкачать (*pull*) актуальное состояние из удаленного репозитория.
