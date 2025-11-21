# Python

## CORE CONTENT

### Python Official

- [Python Official](https://www.python.org/)
- [Python Documentation](https://docs.python.org/3/)
- [Python Standard Library](https://docs.python.org/zh-cn/3/library/index.html)
- [PyPI - The Python Package Index](https://pypi.org/)

### Python Enhancement Proposals (PEPs)

- [PEP 0 - Index of Python Enhancement Proposals](https://peps.python.org/)
- [PEP 20 – The Zen of Python](https://peps.python.org/pep-0020/)
- [PEP 8 – Style Guide for Python Code](https://peps.python.org/pep-0008/)
- [PEP 257 – Docstring Conventions](https://peps.python.org/pep-0257/)
- [PEP 484 – Type Hints](https://peps.python.org/pep-0484/)
- [PEP 498 – Literal String Interpolation](https://peps.python.org/pep-0498/)
- [PEP 572 – Assignment Expressions](https://peps.python.org/pep-0572/)

### Python Project Management

- Official Dependency Management
    - pip
    - requirements.txt / pyprojcet.toml
- Official Virtual Environment Management
    - venv
    - virtualenv

- Morden Management Tools
    - uv
    - Poetry
- PDM

- Three-party Packaging and Release
    - setuptools
    - Flit
    - Hatch
    - twine
- Automated tasks and tests
    - tox
    - nox
    - pytest
    - mypy
- Beautiful Code
    - Ruff

### Foundation

- [Python编程从入门到实践.pdf](http://192.168.100.99:9090/computer-science/programming-languages/dynamic/python/Python编程从入门到实践.pdf)
- [Python工匠.epub]({{ files_server }}/computer-science/programming-languages/dynamic/python/Python工匠.epub)
- [Python学习手册.epub]({{ files_server }}/computer-science/programming-languages/dynamic/python/Python学习手册.epub)
- [简明Python教程.pdf]({{ files_server }}/computer-science/programming-languages/dynamic/python/简明Python教程.pdf)

### Intermediate

- [Python3标准库.pdf]({{ files_server }}/computer-science/programming-languages/dynamic/python/Python3标准库.pdf)
- [流畅的Python.pdf]({{ files_server }}/computer-science/programming-languages/dynamic/python/流畅的Python.pdf)
- [Python Cookbook.pdf]({{ files_server }}/computer-science/programming-languages/dynamic/python/Python%20Cookbook.pdf)
- [Effective Python.pdf]({{ files_server }}/computer-science/programming-languages/dynamic/python/Effective%20Python.pdf)
- [Python语言及其应用.pdf]({{ files_server }}/computer-science/programming-languages/dynamic/python/Python语言及其应用.pdf)

### Advanced

- [Python 3 面向对象编程.pdf]({{ files_server }}/computer-science/programming-languages/dynamic/python/Python%203%20面向对象编程.pdf)
- [Python高级编程.epub]({{ files_server }}/computer-science/programming-languages/dynamic/python/Python高级编程.epub)
- [Python高性能编程.epub]({{ files_server }}/computer-science/programming-languages/dynamic/python/Python高性能编程.epub)

### Resource

[Awesome-Python](https://github.com/vinta/awesome-python)

### Interpreters

|Interpreters |Implementation Language|Runtime Enviromnet|
|:-----------:|:---------------------:|:----------------:|
|CPython      |C                      |Multiple OS       |
|PyPy         |RPython                |Multiple OS       |
|RustPython   |Rust                   |Multiple OS       |
|IronPython   |C#                     |.NET              |
|Jython       |Java                   |JVM               |

### Compilers

|Compiler   |Implementation Language|Target Format |
|:---------:|:---------------------:|:------------:|
|Pyodide    |C                      |WebAssembly   |
|Cython     |Python/C               |C/C++ Code    |
|Nuitka     |Python/C               |C/C++ Code    |
|PyInstaller|Python                 |Package       |

## BASIC USE-CASES

### CLI/TUI Programming

|Module|CLI   |TUI   |
|:----:|:----:|:----:|
|argparse|✅|❌|
|Rich|✅|✅|
|Typer|✅|❌|
|Click|✅|❌|
|fire|✅|❌|
|tabulate|✅|❌|
|Blessed|❌|✅|
|curses|❌|✅|
|Prompt-Toolkit|✅|✅|
|npyscreen|❌|✅|
|urwid|❌|✅|
|Textual|✅|✅|

### GUI Programming

- Tkinter
- PyQt/PySide
- Kivy

### Network Programming

- [Python网络编程攻略 PDF]({{ files_server }}/computer-science/programming-languages/dynamic/python/advanced/Python网络编程攻略.pdf)

- Application Protocols (With Built-in Module)

|Application Protocols|Built-in Module|Third Party|
|:-------------------:|:-------------:|:---------:|
|HTTP/HTTPS|http.client, urllib.request, http.server, wsgiref|pycurl, requests, aiohttps, httpx, [Application-Server](http://192.168.100.36:8000/computer-science/programming-languages/dynamic/python/#application-server)|
|FTP/FTPS|ftplib|aioftp|
|SMTP/SMTPS|smtplib|aiosmtplib, yagmail|
|POP3/IMAP|poplib, imaplib|imapclient, mail-aprser|
|Telnet|telnetlib|pexpect|
|SOAP/XML-RPC|xmlrpc.client, xmlrpc.server|zeep|

- Application Protocols (Not Built-in Module)

|Application Protocols|Third Party|
|:-------------------:|:---------:|
|DNS|dnspython|
|SSH/SFTP|paramiko, asyncssh, fabric|
|WebSocket|websockets, aiohttp, socket.io, python-socketio|
|MQTT|paho-mqtt, gmqtt, asyncio-mqtt|
|AMQP/RabbitMQ|pika, aio-pika|
|Redis(RESP)|redis, aioredis|
|PostgreSQL/MySQL|psycopg2, syncpg, mysql-connector, aiomysql|
|LDAP|ldap3|
|NTP|ntplib|
|SNMP|pysnmp|
|CoAP|aiocoap, coaptho|
|gRPC|grpcio, grpclib|
|TFTP|tftpy|
|IRC/XMPP|irc, slixmpp, aioxmpp|
|JSON-RPC|jsonrpclib, aiojsonrpc|

- Sockets
    - asyncio
    - ipaddress
    - select
    - socket
    - socketserver
    - ssl
- Packet Capture
    - Scapy
    - PyShark
    - Pcapy
    - dpkt

### Scripting

- subprosess
- sh

### Web/API Application-Server

- [WSGI](https://docs.python.org/3/library/wsgiref.html)
    - uWSGI
    - Waitress
    - Gunicorn
    - Daphne

- [ASGI](https://asgi.readthedocs.io/en/latest/)
    - Daphne
    - Hypercorn
    - Uvicorn

- Django
    - [Django](https://docs.djangoproject.com/)
    - [Awesome Django](https://github.com/shahraizali/awesome-django)
    - [Awesome Django CN](https://github.com/haiiiiiyun/awesome-django-cn)

- Flask
    - [Flask](https://flask.palletsprojects.com/en/stable/)
    - [Awesome Flask](https://github.com/humiaozuzu/awesome-flask)

- FastAPI
    - [FastAPI](https://fastapi.tiangolo.com/)
    - [Awesome FastAPI](https://github.com/mjhea0/awesome-fastapi)

- Tornado
    - [Tornado](https://www.tornadoweb.org/en/stable/index.html)

- Ohter
    - Bottle
    - CherryPy
    - Pyramid
    - Web2Py
    - Sanic

### Web Crawler

- [Python3 反爬虫原理与绕过实战 PDF]({{ files_server }}/computer-science/programming-languages/dynamic/python/advanced/Python3%20反爬虫原理与绕过实战.pdf)
- [Python3 网络爬虫开发实战 第2版 PDF]({{ files_server }}/computer-science/programming-languages/dynamic/python/advanced/Python3%20网络爬虫开发实战%20第2版.pdf)
- [Python网络数据采集 PDF]({{ files_server }}/computer-science/programming-languages/dynamic/python/advanced/Python网络数据采集.pdf)
- [反爬虫AST原理与还原混淆实战 PDF]({{ files_server }}/computer-science/programming-languages/dynamic/python/advanced/反爬虫AST原理与还原混淆实战.pdf)
- [精通Python爬虫框架Scrapy EPUB]({{ files_server }}/computer-science/programming-languages/dynamic/python/advanced/精通Python爬虫框架Scrapy.epub)

- Data Scraping
    - HTTP/URL
    - Playwright
    - Puppeteer
    - Selenium
- Data Processing
    - BeautifulSoup
    - lxml
- Data-Storage
    - JSON/XML
    - Databases
    - Context
- Frameworks
    - Scrapy
    - PySpider
    - EasySpider
- JavaScript Reverse Engineering

### Database Programming

- ORM
    - SQLAlechemy
    - Django ORM
    - Peewee

|Databases|Python Connectors|
|:-------:|:---------------:|
|SQLite|sqlite3|
|PostgreSQL|psycopg2|
|MySQL|mysql-connector-python, PyMySQL|
|MS SQL Server|pyodbc, mymssql|
|Oracle|cx_Oracle|
|MongoDB|pymongo|
|Redis|redis-py|

### Logging Tools

- Loguru

## ADVANCED USE-CASES

### Automated Testing

- [Python自动化测试实战 PDF]({{ files_server }}/computer-science/programming-languages/dynamic/python/advanced/Python自动化测试实战%20.pdf)
- pytest
- Robot-Framework
- unittest

### Automated-Operations

- [Python Linux系统管理与自动化运维 PDF]({{ files_server }}/computer-science/programming-languages/dynamic/python/advanced/Python%20Linux系统管理与自动化运维.pdf)
- [Python自动化运维 EPUB]({{ files_server }}/computer-science/programming-languages/dynamic/python/advanced/Python自动化运维.epub)
- Diamond

### Data-Science

- Tools
    - JupyterLab
    - Marimo
- Data Processing & Analysis
    - Polars
    - Pandas
    - Numpy
    - SciPy
- Data Visualization
    - Matplotlib
    - Seaborn
    - Plotly
    - Bokeh

- Machine-Learing
    - Scikit-learn
    - TensorFlow
    - PyTorch
    - Keraas

### Cryptography

- [Python密码学编程 EPUB]({{ files_server }}/computer-science/programming-languages/dynamic/python/advanced/Python密码学编程.epub)
- cryptography
- PyCryptodome
- secrets
- Hash
    - hashlib
    - Hmac
- Password Auth
    - bcrypt
    - passlib
- rsa
- ecdsa
- pynacl
- ssl
- m2crypto

### Embedded/IoT

- MicroPython
- CircuitPython
- Zerynth
- Pyserial
- PyUSB
- PyBluez
- PyModbus
- paho-mqtt
- PyCom

### Game Development

- Pygame
- Arcade
- Pyglet
