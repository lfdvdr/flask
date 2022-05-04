# flask
Web- технологии разработки прикладных программных систем

hello.py - в браузере по адресу http://127.0.0.1:5000/ проект запустился и вывел фразу Hello, World!

lesson2.py - маршрутизация, export FLASK_APP=lesson2.py

лабораторная работа 3:

>>> from flask import url_for  <br />
>>> from lesson3 import app  <br />
>>> with app.test_request_context('/api'): url_for('index') <br />
...  <br />
'/' <br />
>>> with app.test_request_context('/api'): url_for('index', _external=True) <br />
...  <br />
'http://localhost/' <br />
>>> with app.test_request_context('/api'): url_for('index', user_id = 100) <br />
...  <br />
'/?user_id=100' <br />
