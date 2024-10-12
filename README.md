![image](https://github.com/user-attachments/assets/408abe48-67e6-4d1a-a160-2908db3a3bf0)# Найстройка дебагера в VS Code для str2int
## Копируем репозиторий 
Создаем папку под репозиторий и открываем её
```
mkdir project
cd project
```
Клонируем форкнутый репозиторий через ssh и открываем его
```
git clone git@github.com:Evgenii-afk/bmstu_cpp_course.git
cd bmstu_cpp_course
```
Открываем vs code и скачиваем рассшиерения
1. Docker
2. CMake
3. CMakeTools
4. CodeLLDB
5. GitHub Actions
Открываем наш репозиторий в vs code:
Crtl+K Ctrl+O и выбираем путь home/projects/bmstu_cpp_course

Открываем терминал в vs code(Ctrl+shift+`) и собираем это дело докером
```
sudo docker compose up --build
```
При корректной сборке мы увидим
```
cpp_course exited with code 0
```
Обратите внимание на то, что в файле CMakeLists.txt стоит в первой строке 
```
cmake_minimum_required(VERSION 3.28)
```
И в файле 
