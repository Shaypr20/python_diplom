<h1 align="center">Приветствуем вас
<img src="https://github.com/blackcater/blackcater/raw/main/images/Hi.gif" height="32"/></h1>
<h3 align="center">Команда</h3>
<h4 align="center">Юрченко Вадим<br>
Вострецов Андрей<br>Булатов Артем<br>Бежин Евгений</h4>
<h1 align="center"><a href="https://github.com/AlchiProMent/GrForecast.git" target="_blank">"Прогнозирование цен"</a></h1>
<h2 align="center">Дипломный проект</h2>
<h3 align="center">Руководитель: Дмитрий Румянцев</h3>
<h4 align="center">Москва, 2023 г.</h4>


## Введение
Проект создан для автоматизированного расчета прогнозных значений временных рядов. Он позволяет в автоматическом режиме подключаться к базе данных формат PostgreSQL, выгружать данные из потока, предобрабатывать их и на основе полученного дата-сета формировать прогноз на указанного количество периодов
## Инструкция по установке
#### Для запуска кода необходимо установить Python 3.9 и выполнить следующие команды:
1. git clone http://... 
2. Создать виртуальное окружение командой 
* > py -m venv env для windows 
* > python -m venv venv для MacOs 
3. Активировать виртуальное окружение командой: 
* > venv\bin\Activate.ps1 для Windows 
* > venv\Scripts\activate для MacOs
4. Установить все необходимые библиотеки командой: 
* > py -m pip install -r requirements.txt
* > python3 -m pip3 install -r requirements.txt
5. Создать файл password.py, в котором будут указана необходимая информация для подключения к базе
* > def my_data():
    db_user = ''
    db_password = ''
    db_host = ''
    db_port = ''
    db_name = ''
    db_type = ''
    return db_name, db_user, db_host, db_password, db_port, db_type
6. Запустить программу командой: 
* > streamlit run [arima_fourie.py](arima_fourie.py)

## Структура репозитория 

1. [Файл all_functions.py](all_functions.py), который содержит все разработанные функции
* [get_df](all_functions.py)
* [weekly_data](all_functions.py)
* [clean_data](all_functions.py)
* [arima_fourie](all_functions.py)
2. [Файл all_functions.py](all_functions.py), который содержит основную программу
3. [Файл arima_fourie_test_version.py](arima_fourie_test_version.py), который содержит тестовый вариант программы (прогноз строится лишь для двух регионов и двух продуктов)
4. [Файл requirements.txt](requirements.txt) содержит список библиотек, которые необходимо установить для функционирования основной программы

