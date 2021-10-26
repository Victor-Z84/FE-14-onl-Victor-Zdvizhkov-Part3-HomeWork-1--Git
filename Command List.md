## FE-14-onl-Victor-Zdvizhkov-Part3-HomeWork-1--Git

### Список команд для каждого пункта: 

1. Создание репозитория

    В консоли переходим в каталог с проектом:
    
  	Windows: `cd C:/Users/user/my_project`
    
  	macOS: `cd /Users/user/my_project`
    
    Затем вводим команду `git init`, в текущем каталоге создается подкаталог .git всех необходимых
    файлов Git-репозитория. Проект еще не находится под версионным контролем.
    
	  На сайте https://github.com в своем аккаунте создаем новый репозиторий, копируем путь к нему для использования ниже.


2. Создание ветки `master`

    По умолчанию имя основной ветки в Git - master. Она создается автоматически при инициализации командой `git init`.

3. Создание файла `index.html` в папке нашего проекта

    1. Добавляем созданный файл `index.html` в индекс: `git add index.html`

    2. Делаем коммит файла `index.html`: `git commit -m ‘added file index.html’`
    
    3. Связываем наш удаленный репозиторий и локальный: `git remote add origin https://github.com/Victor-Z84/…`
    
    4. Добавляем изменения на удаленный репозиторий в ветку `master`: `git push -u origin master` 
    

4. Создаем файл `style.css` (сброс стилей + стилизация) в папке `css` проекта

    1. Добавить файл `style.css` в индекс: `git add style.css`

    2. Делаем коммит: `git commit -m ‘added file style.css’`
    
    3. Добавляем изменения на удаленный репозиторий: `git push`

5. Создать ветку `version-1` от ветки `master`
    
    1. Команда `git branch` - показывает список веток и наше текущее положение в них
    
    2. Создаем новую ветку `version-1`, 2 способа: 
        1. Команда `git branch version-1`, далее - `git checkout version-1` - переход на эту ветку
        
        2. Команда `git checkout -b version-1` - создаем и одновременно переключаемся на ветку version-1
    
6. Продолжаем работу в ветке `master`, переключаемся на нее: `git checkout master`

7. Переименовать файл `style.css` -> `styles.css`: `git mv css/style.css css/styles.css` 
   (команда заменяет `git rm` - удаление старого файла и `git add` - добавление нового в индекс)

    1. Делаем коммит: `git commit -m ‘style.css changed to styles.css’`
    
    2. Добавляем на удаленный репозиторий: `git push`

8. Создаем файл `index.js` в папке `js` проекта, подключаем его к документу (вызов `alert`)

    1. Добавляем изменения в индекс: `git add .` - одновременно изменения в файлах `index.html`, `index.js`

    2. Делаем коммит: `git commit -m ‘added file index.js’`
    
    3. Добавляем изменения на удаленный репозиторий - `git push` 

9. Вносим изменения в свойства стилей

    1. Добавляем изменения в индекс: `git add css/styles.css`

    2. Делаем коммит изменений в `master`: `git commit -m ‘added changes in styles.css’`

    3. Переход на ветку `version-1`: `git checkout version-1` 

    4. Применяем последний коммит с изменениями стилей в ветке `master` к нашей текущей ветке `version-1`:


