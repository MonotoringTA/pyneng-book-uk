Булеві значення
===============

Булеві значення в Python - це дві константи True і False.

У Python істинними та хибними значеннями вважаються не тільки True та False.

* правда:

  * будь-яке ненульове число
  * будь-який непустий рядок
  * будь-який непустий об'єкт

* хибність:

  * 0
  * None
  * порожній рядок
  * порожній об'єкт

Для перевірки булевого значення об'єкта можна скористатися bool:

.. code:: python

    In [2]: items = [1, 2, 3]

    In [3]: empty_list = []

    In [4]: bool(empty_list)
    Out[4]: False

    In [5]: bool(items)
    Out[5]: True

    In [6]: bool(0)
    Out[6]: False

    In [7]: bool(1)
    Out[7]: True

