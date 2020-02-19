
.. end-of-readme-intro

Installation
------------

::

    pip install git+https://github.com/rxy007/loguru.git



Ready to use out of the box without boilerplate
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The main concept of `Loguru` is that **there is one and only one** |logger|_.

For convenience, it is pre-configured and outputs to ``stderr`` to begin with (but that's entirely configurable).

::

    from loguru import logger

    logger.debug("That's it, beautiful and simple logging!")

The |logger|_ is just an interface which dispatches log messages to configured handlers. Simple, right?

use json log
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

new add argv type='json'

::

    logger.add(sys.stdout, format='{time} {level} {module} {function} {line} {message}', catch=True, type='json')

    logger.info('rrrrr', extra_dict={'r': 'rrrrrrrrrr', 'wo': ['我是', '冉小瑜']})


