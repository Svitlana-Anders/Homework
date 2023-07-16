1. На локальном репозитории сделать ветки для:

- Postman
```
git branch Postman
```
- Jmeter
```
git branch  Jmeter
```
- CheckLists
```                                         
git branch CheckLists 
```
- Bug Reports
```
git branch BugReports
```
- SQL
```
git branch SQL
```  
- Charles
```
git branch Charles
```
- Mobile testing
```
git branch Mobile_testing
```
 2. Запушить все ветки на внешний репозиторий
```
git checkout Postman
git push origin Postman
```                                                        
3. В ветке Bug Reports сделать текстовый документ со структурой баг репорта
```
git checkout BugReports 
touch  Bug_Report_01.txt
vim  Bug_Report_01.txt
          i
                   ID                          01
                   Module                      Main Page
                   Environment                 Windows 10
                   Summary                     System crashed after clicking Sign in button
                   Steps to reproduce          1.Open the URL... 
                                               2.Click Sign in button
                   Expected Result             Sign in form is opened
                   Actual Result               System crashes
                   Reproducibility             2/10
                   Attachment                  URL..…
Esc :x
```
4. Запушить структуру багрепорта на внешний репозиторий
```
git add Bug_Report_01.txt 
git commit -m  "bug report structure"
git push origin BugReports
```      
5. Вмержить ветку BugReports в Main
```
git checkout main
git merge BugReports
```
6. Запушить main на внешний репозиторий
```
git push origin main
```
7. В ветке CheckLists набросать структуру чек листа.
```
git checkout  CheckLists 
cat > CheckList_Structure.txt
                     Структура чек листа
Ctrl+C
```                                                        
8. Запушить структуру на внешний репозиторий
```
git add CheckList_Structure.txt 
git commit -m  "check list structure"
git push origin CheckLists
```
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
                                                 
10. Синхронизировать Внешнюю и Локальную ветки Main
```
git checkout main
git pull
```

