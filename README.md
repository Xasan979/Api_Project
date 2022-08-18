# Api_Project

Как запустить:
    
   Создайте venv и установите требования
       
       Mac OS
          python3 -m venv env
          source env/bin/activate - for Unix or MacOS
          pip install -r requirements
  
        Windows
          py -m venv env
          .\env\Scripts\activate
          py -m pip install -r requirements



Получение отчетов: 

   Установка allure 
   
       Mac OS
          brew install allure

       Windows (PowerShell)
          scoop install allure



Провести тест:

   В терминале (Pycharm)

          python -m pytest --alluredir=test_results/ tests/test_google_maps_api.py


Сгенерировать отчет:

   В командной строке 
   
          cd (путь к папки с проектом)
          allure serve test_results/
