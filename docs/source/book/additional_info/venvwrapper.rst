virtualenvwrapper
^^^^^^^^^^^^^^^^^

Виртуальные окружения создаются с помощью virtualenvwrapper.

Установка virtualenvwrapper с помощью pip:

::

    $ sudo pip3.7 install virtualenvwrapper

После установки, в файле .bashrc, находящимся в домашней папке текущего
пользователя, нужно добавить несколько строк:

::

    export VIRTUALENVWRAPPER_PYTHON=/usr/local/bin/python3.7
    export WORKON_HOME=~/venv
    . /usr/local/bin/virtualenvwrapper.sh

Если вы используете командный интерпретатор, отличный от bash,
посмотрите, поддерживается ли он в
`документации <http://virtualenvwrapper.readthedocs.io/en/latest/install.html>`__
virtualenvwrapper. Переменная окружения VIRTUALENVWRAPPER\_PYTHON
указывает на бинарный файл командной строки Python, WORKON\_HOME – на
расположение виртуальных окружений. Третья строка указывает, где
находится скрипт, установленный с пакетом virtualenvwrapper. Для того,
чтобы скрипт virtualenvwrapper.sh выполнился и можно было работать с
виртуальными окружениями, надо перезапустить bash.

Перезапуск командного интерпретатора:

::

    $ exec bash

Такой вариант может быть не всегда правильным. Подробнее на `Stack
Overflow <http://stackoverflow.com/questions/2518127/how-do-i-reload-bashrc-without-logging-out-and-back-in>`__.

Работа с виртуальными окружениями
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. note::

    В Python есть несколько вариантов для создания виртуальных окружений.
    Использовать можно любой из них.


Создание нового виртуального окружения, в котором Python 3.7
используется по умолчанию:

