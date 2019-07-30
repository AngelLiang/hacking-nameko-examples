Quick Start
#############

Install
********

- PostgreSQL
- Redis
- RabbitMQ


venv
********

.. code:: powershell

    $ pipenv install --dev
    $ pipenv shell


products
*********

.. code:: powershell

    $ pipenv shell
    $ cd products
    $ pytest
    $ nameko run --config config.yml products.service --backdoor 3000


orders
*******

使用了 `alembic` 对数据库进行管理

.. code:: powershell

    $ pipenv shell
    $ cd orders
    $ pytest
    $ alembic upgrade head
    $ nameko run --config config.yml orders.service --backdoor 3000


gateway
********

.. code:: powershell

    $ pipenv shell
    $ cd gateway
    $ pytest
    $ nameko run --config config.yml gateway.service --backdoor 3001
