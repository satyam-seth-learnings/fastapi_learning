- [SQLAlchemy Asynchronous I/O (asyncio) Doc](https://docs.sqlalchemy.org/en/20/orm/extensions/asyncio.html)

- [Alembic’s Installation Doc](https://alembic.sqlalchemy.org/en/latest/front.html#installation)

- [Using Asyncio with Alembic Doc](https://alembic.sqlalchemy.org/en/latest/cookbook.html#using-asyncio-with-alembic)

- Install SQLAlchemy with async support

    ```bash
    pip install sqlalchemy[asyncio]
    ```

- Install aiosqlite for SQLite

    ```bash
    pip install aiosqlite
    ```

- Install Alembic

    ```bash
    pip install alembic
    ```

- Initialize Alembic

    ```bash
    alembic init -t async alembic
    ```