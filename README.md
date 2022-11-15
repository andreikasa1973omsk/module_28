Данный проект - это финальное задание по курсу "Тестировщик-автоматизатор на Python (QAP) 
на онлайн-платформе "Skillfactory"
Содержание задания: написать 50-70 автоматизированных тестов с использованием 
PyTest и Selenium для тестирования интернет-магазина.

Проект разработан для тестирования сайта интернет-магазина "Ozon" (https://www.ozon.ru/)

В файле "config" прописаны тестовые данные для выполнения тестов, как проверки их успешного прохождения,
так и выполнения тестов, так же информация о базовом URL

В файле conftest.py содержится фикстура для используемого вебдрайвера Chrome. 
Драйвер требуется установить в папку driver

Папка pages содержит:
    Base_page содержит базовый класс BasePage, c методами используемыми для выполнения тестов.
    Main_page содержит все локаторы, для выполнения тестов

Файл requirements.txt содержит перечень необходимых библиотек для работы проекта.

Команды для запуска всех тестов 
   python -m pytest -v --driver Chrome --driver-path driver/chromedriver.exe  tests/test_MainPage.py

Тесты проверяют видимость кнопок на главной странице сайта, их кликабельность, корректность названия кнопок, 
соответствие разделов, куда ведет клик по кнопке.

Данный проект был написан и протестирован на окружении Windows 10, 
Google Chrome: Версия 106.0.5249.103 (Официальная сборка), (64 бит)
