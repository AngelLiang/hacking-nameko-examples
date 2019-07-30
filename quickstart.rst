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

    $ pipenv install
    $ pipenv shell


products
*********

.. code:: powershell

    $ pipenv shell
    $ cd products
    $ nameko run --config config.yml products.service --backdoor 3000


orders
*******

.. code:: powershell

    $ pipenv shell
    $ cd orders
    $ alembic upgrade head
    $ nameko run --config config.yml orders.service --backdoor 3000


gateway
********

.. code:: powershell

    $ pipenv shell
    $ cd gateway
    $ nameko run --config config.yml gateway.service --backdoor 3001
