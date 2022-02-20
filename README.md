## **Repository 3 TXT**
**1. Создать внешний репозиторий c названием TXT**
- **version via GitHub**:
	- push `NEW` button
	- enter repository name "TXT"
	- choose a `README file` option
	- push `Create repository` button
- **version via Terminal for authenticated users only**:
	- use API link to send POST request:
[API link](https://api.github.com/)
	- enter the command:
```bash
curl -u "YourGitHubName" https://api.github.com/user/repos -d "{"name":"TXT","public": true}"
```
	- enter your password
	- under response find URL named "clone_url": and copy it
	- go to GitHub by copied link and find your new repository

- **version via Terminal for any user**:
```bash
mkdir TXT
cd TXT
git init
touch README.md
git commit -m "commit of txt"
```
```bash
git remote add origin 
git@github.com:YourGitHubName/<TXT>.git
```
```bash
curl -u YourGitHubName:YourTokinORYourPassword https://api.github.com/user/repos -d '{"name":"TXT"}'
```

**2. Клонировать репозиторий TXT на локальный компьютер**
- copy link of repository under `Code` button
![Commit button](https://github.com/Olga-Ivasenko/TXT/blob/394eeeac64ecadce6d2e6429a54dd567b9f39f9a/edit_picture5.jpg)
- commands:
```bash
cd MyDirectory	//where new project to be placed locally
git clone + <copied link>
```

**3. Внутри локального TXT создать файл “new.txt”**
```bash
cd Part_Json
touch new.txt
```
**4. Добавить файл под гит**
```bash
git add new.txt // to add exact file
git add . // to add all files
```
**5. Закоммитить файл**
```bash
git commit -m "txt commit"
```
**6. Отправить файл на внешний GitHub репозиторий**
```bash
git status
git push
```
**7. Отредактировать содержание файла “new.txt” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате TXT**

```bash
cd MyDirectory
vim new.txt
```
- enter txt data:
[TXT data](https://github.com/Olga-Ivasenko/TXT/blob/6470e79b852e6aa74f0ba34221356505cf6a364e/new.txt)

**8. Отправить изменения на внешний репозиторий**
```bash
git status
git commit -m "new txt changes" // if all added files
git commit -m "new txt changes" new.txt // if selected file
git push
```

**9. Создать файл preferences.txt**
```bash
cd TXT
touch preferences.txt
```

**10. В файл preferences.txt добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате TXT**
```bash
cd TXT
vim preferences.txt
```
- enter txt data:
[TXT data](https://github.com/Olga-Ivasenko/TXT/blob/9010f312e2b25c0f75aaa6b0a9bb2c1efeb8ed85/preferences.txt)


**11. Создать файл sklls.txt добавить информацию о скиллах которые будут изучены на курсе в формате TXT**
```bash
cd TXT
touch sklls.txt
vim sklls.txt // or without touch but save before closing
```
- enter txt data
[txt data](https://github.com/Olga-Ivasenko/TXT/blob/9010f312e2b25c0f75aaa6b0a9bb2c1efeb8ed85/skills.txt)

**12. Сделать коммит в одну строку**
```bash
cd TXT
git status
git add skills.txt
git add preferences.txt
git status
git commit -m "add two files" skills.txt preferences.txt
```

**13. Отправить сразу 2 файла на внешний репозиторий**
```bash
git push
```
**14. На веб интерфейсе создать файл bug_report.txt**
- go to GitHub, repository you`ve created
- push `Add File` dropdown button
- choose `Create new file`
![Commit button](https://github.com/Olga-Ivasenko/TXT/blob/394eeeac64ecadce6d2e6429a54dd567b9f39f9a/edit_picture4.jpg)
- name your file "bug-report.txt"

**15. Сделать Commit changes (сохранить) изменения на веб интерфейсе**
- choose `Edit new file` tab
- enter \{} to the edit field of the file
- choose `Preview` tab
- push `Commit your file` button
![Commit button](https://github.com/Olga-Ivasenko/TXT/blob/394eeeac64ecadce6d2e6429a54dd567b9f39f9a/edit_picture3.jpg)

**16. На веб интерфейсе модифицировать файл bug_report.txt, добавить баг репорт в формате TXT**
- go to main branch of repository
- step on your file "bug-report.txt"
- choose `edit` pictogram
![how to find Edit](https://github.com/Olga-Ivasenko/TXT/blob/394eeeac64ecadce6d2e6429a54dd567b9f39f9a/edit_picture1.jpg)
- enter txt data:
[TXT data](https://github.com/Olga-Ivasenko/TXT/blob/e11e35974fadfdc16d29b4cc6f97b2ffcf9916ee/bug_report.txt)

**17. Сделать Commit changes (сохранить) изменения на веб интерфейсе**
- go down of edit file page
- *optional*: add description
- click `Commit changes` button
![Commit button](https://github.com/Olga-Ivasenko/TXT/blob/394eeeac64ecadce6d2e6429a54dd567b9f39f9a/edit_picture2.jpg)

**18. Синхронизировать внешний и локальный репозиторий TXT**
```bash
cd TXT
git pull
git add .
git status
git commite -m
git push

```



