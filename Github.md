# JSON

4. Create an external repository named JSON.
```
Repositories
New   
Create Repository   
```
5. Clone the JSON repository to the local machine.
```
git clone https://github.com/Svitlana-Anders/JSON.git
```
6. Inside the local JSON, create a “new.json” file.
```
cd JSON
git touch new.json
```
7. Add file to index
```
git add new.json
```
8. Commit file.
```
git commit new.json
```
9. Submit the file to an external GitHub repository.
```
git push origin main
```
10. Edit the contents of the “new.json” file - write information about yourself (full name, age, number of pets, future desired salary). Everything is written in JSON format.
```
vim new.json
       i            
             {                   
               "name": "Svitlana",
               "surname": "Anders",
               "age": 44,
               "pets":"dog",
               "expected salary": 2000
              }
esc  =>   Ctrl+c  =>  :x
```
11. Push changes to an external repository.
    ```
git commit -am "adding changes to file 1"
git push origin main
    ```
12. Create preferences.json file
 ```
touch preferences.json
```
13.In the preferences.json file, add information about your preferences (Favorite movie, favorite series, favorite food, favorite season, side you would like to visit) in JSON format.
```
vim preferences.json
      i   
               {                                               
                  "favorite film":"Catch me if you can",
                  "favorite serial":"House,M.D.",
                  "favorite dish":"ice-cream",
                  "favorite season":"summer",
                  "wished travel":"India"
                }
esc  =>   Ctrl+c  =>  :wq
```
14.Create a skills.json file add information about the skills that will be studied in the course (in JSON format)
```
cat > skills.json
                   {                          
                     "skill 1": "Terminal Linux",
                     "skill 2": "Github",
                     "skill 3": "Postman",
                     "skill 4": "Charles",
                     "skill 5": "Android Studio"
                   }
Ctrl+d
```
15.Send 2 files at once to an external repository.
```
git add preferences.json skills.json
git commit -m "Adding two failes"
git push origin main
```
16. Create a bug_report.json file on the web interface.
```
Add file
Create new file  bug_report.json
```
17. Make Commit changes (save)  on the web interface.
```
Commit new file
```
18.On the web interface, modify the bug_report.json file, add a bug report in JSON format.
Choose  bug_report.json in the list of files
```
Click Edit 
Add the text in json format 
              {
                "ID":01,
                "Module": "Main Page",
                "Environment": "Windows 10",
                "Summary": "System crashed after clicking Sign in button",
                "Steps to reproduce": "1.Open the URL... 2.Click Sign in button",
                "Expected Result": "Sign in form is opened",
                "Actual Result": "System crashes",
                "Reproducibility": "2/10",
                "Attachment": "URL..…"
               }
```               
19. Make Commit changes (save)  on the web interface.
```
Commit changes
```
20. Synchronize external and local JSON repository
```
git pull
```


# XML

21. Create an external repository named XML.
```
Repositories
New
Create Repository
```
22. Clone the XML repository to the local machine.
```
Git clone https://github.com/Svitlana-Anders/XML.git
```
23. Inside the local XML, create a “new.xml” file
```
cd XML
touch new.xml
```
24.Add file to index
```
git add new.xml
```
25. Commit the file.
```
git commit -m “Adding xml file”
```
26. Submit the file to an external GitHub repository.
```
git push origin main
```
27. Edit the contents of the “new.xml” file - write information about yourself (name, age, number of pets, future desired salary). Everything is written in XML format.
 ```
vim new.xml
           i
               <?xml version="1.0" encoding="UTF-8" ?>
               <root> 
               <name>Svitlana</name>  
               <surname>Anders</surname>
               <age>44</age>  
               <pets>dog</pets> 
               <expected salary>2000</expected salary>
               </root>
 esc :x
```
28. Push changes to an external repository.
```
git commit -am “Adding changes to xml file”
git push origin main
```
29. Create preferences.xml file
```
touch preferences.xml
```
30. In the preferences.xml file, add information about your preferences (Favorite movie, favorite series, favorite food, favorite season, side you would like to visit) in XML format.
```
vim preferences.xml
          i
            <?xml version="1.0" encoding="UTF-8" ?>
            <root> 
            <favorite film>Catch me if you can</favorite film>
            <favorite serial>House,M.D.</favorite serial> 
            <favorite dish>ice-cream</favorite dish>  
            <favorite season>summer</favorite season> 
            <wished travel>India</wished travel>
            </root>
esc :x
```
31.Create skills.xml file add information about the skills that will be studied in the course in XML format
```
cat > skills.xml
              <?xml version="1.0" encoding="UTF-8" ?>
              <root>  
              <skill 1>Terminal Linux</skill 1> 
              <skill 2>Github</skill 2>  
              <skill 3>Postman</skill 3>  
              <skill 4>Charles</skill 4>  
              <skill 5>Android Studio</skill 5>
              </root>
Ctrl+d
```
32. Make a commit in one line.
```
git add .
git commit -am "committing two files in one string"
```
33.Send 2 files at once to an external repository.
```
git push origin main
```
34. Create a bug_report.xml file on the web interface.
```
Add file
Create new file  bug_report.xml
```
35. Make Commit changes (save) on the web interface.
```
Commit new file
```
36.Modify the bug_report.xml file on the web interface, add a bug report in XML format.
```
Choose  bug_report.xml in the list of files
Click Edit 
Add the text in xml format 
            <?xml version="1.0" encoding="UTF-8" ?>
            <root> 
            <ID>01</ID> 
            <Module>Main Page</Module>  
            <Environment>Windows 10</Environment>  
            <Summary>System crashed after clicking Sign in button</Summary>  
            <Steps to reproduce>1.Open the URL... 
                                2.Click Sign in button</Steps to reproduce> 
           <Expected Result>Sign in form is opened</Expected Result>  
           <Actual Result>System crashes</Actual Result>  
           <Reproducibility>2/10</Reproducibility>  
           <Attachment>URL..…</Attachment>
           </root>
```  
37.Make Commit changes (save) changes on the web interface.
```
Commit changes
```
38. Synchronize external and local XML repository
```
git pull
```
#TXT

1. Create an external repository called TXT.
                         
2.Clone the TXT repository to the local machine.
```
git clone https://github.com/Svitlana-Anders/TXT.git
```
3. Inside the local TXT, create a “new.txt” file.
```
cd TXT
touch new.txt
```
4. Add file to index
```
git add new.txt
```
5. Commit the file.
 ```
git commit -m "adding txt file"
```
6. Send a file to an external GitHub repository.
```
git push origin main
```
7.Edit the contents of the “new.txt” file - write information about yourself (name, age, number of pets, future desired salary). Write everything in TXT format.
```
vim new.txt
      i            
            name - Svitlana
            surname - Anders
            age - 44
            pets - dog
            expected salary - 2000
esc :x
```    
8. Push changes to an external repository.
```
git commit -am "Adding changes to txt file"
git push origin main
```
9. Create preferences.txt file
```
touch preferences.txt
```
10.Add information about your preferences (Favorite movie, favorite series, favorite food, favorite season, side you would like to visit) in the file preferences.txt in TXT format.
```
vim preferences.xml
        i
             favorite film - Catch me if you can
             favorite serial - House,M.D.
             favorite dish - ice-cream
             favorite season - summer
             wished travel - India
esc :x
```
11. Create skills.txt file add information about the skills that will be studied on the course in TXT format
```
cat > skills.txt
                skill 1 - Terminal Linux
                skill 2 - Github
                skill 3 - Postman
                skill 4 - Charles
                skill 5 - Android Studio                                                   
Ctrl+d
```
12. Make a commit in one line.
```
git add .
git commit -m "committing two files in one string"
```
13. Send 2 files at once to an external repository.
 ```
git push origin main
```
14. On the web interface, create a bug_report.txt file.
```
Add file
Create new file  bug_report.txt
```
15. Make Commit changes (save) on the web interface.
```
Commit new file
```
16. Modify the bug_report.txt file on the web interface, add a bug report in TXT format.
```
Choose  bug_report.txt in the list of files
Click Edit 
Add the text in txt format 
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
```                                         
17.Make Commit changes (save) on the web interface.
 ```
Commit changes
```
18. Synchronize external and local TXT repository
 ```
git pull
```
