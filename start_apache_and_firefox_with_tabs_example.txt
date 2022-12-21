
start cmd.exe /k "C:\xampp5\apache_start.bat"
TIMEOUT /T 2 /NOBREAK
#agregando espacios en blanco a una url:
SET "emptyVal=%%20"
SET "doubleEmptyVal=%%20%%20"
SET URLs= localhost:8080/phpmyadmin localhost:8081/5-7-2020%doubleEmptyVal%canavesio%EmptyVal%hormigones
SET NewTab=-new-tab
FOR %%a in ("%URLs%") DO (Start /d "%programfiles(x86)%\Mozilla Firefox" Firefox.exe %NewTab% "%%a")
START cmd.exe /c "cd "C:\xampp5\htdocs\5-7-2020  canavesio hormigones" && "code . && exit /b" 

