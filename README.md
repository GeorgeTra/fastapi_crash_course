# fastapi_crash_course

___
Это api, с помощью которого можно добавить задачу с описанием в список дел и вернуть список задач. 

## Установка

### Склонируйте проект к себе на компьютер с GitHub:
```python
git clone https://github.com/GeorgeTra/fastapi_crash_course.git
```

### Перейдите в папку проекта:
```python
cd fastapi_crash_course   
```

### Docker

У вас на компьютере должна быть установлена десктопная версия docker.
Для установки можно воспользоваться инструкцией: https://docs.docker.com/desktop/


### Запуск приложения
- Создание образа (коробки) с приложением
```
docker build . --tag fastapi_app
```
- Запуск образа в контейнере с пробросом портов для доступа к контейнеру из интернета
```
docker run -p 80:80 fastapi_app
```
- Откройте десктопную версию docker и нажмите _Open with browser_
![img.png](samples/img.png)

- Можно добавить задачу через _Add task_
![img_1.png](samples/img_1.png)

- Можно получить список добавленных задач через _Get task_
![img_2.png](samples/img_2.png)