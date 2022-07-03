```py
py manage.py migrate - -fake - initial - -run - syncdb
```

- **СОЗДАНИЕ ПРОЕКТА**

    ```python
    django-admin startproject <название_проекта>
    ```

- **СОЗДАНИЕ ПРИЛОЖЕНИЙ**  
  (в директории с файлом `manage.py`)

    ```python
    python manage.py startapp <название_приложения>
    ```

- **ЗАПУСК СКРИПТОВ**  
  (в директории с файлом `manage.py`)

  ```python
  python manage.py runscript my_script.py
  ```
  
  <details>
    <summary>Структура проекта</summary>
  
    ```cmd
        my_app/
            __init__.py
            models.py
            scripts/
                __init__.py
                my_script.py
            tests.py
            views.py
    ```
  </details>


- **ЗАПУСК КОМАНД**  
  (в директории с файлом `manage.py`)

  ```python
  python manage.py my_command.py
  ```
  
  <details>
    <summary>Структура проекта</summary>
  
    ```cmd
      my_app/
          __init__.py
          models.py
          management/
              __init__.py
              commands/
                  __init__.py
                  my_command.py
          tests.py
          views.py
    ```
  </details>
