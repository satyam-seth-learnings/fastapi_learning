- [FastAPI Installation Doc](https://fastapi.tiangolo.com/#installation)

- Create python virtual environment

    ```bash
    python3 -m venv .venv
    ```

- Activate the virtual environment

    ```bash
    source .venv/Scripts/activate
    ```

- Install FastAPI

    ```bash
    pip install "fastapi[standard]"
    ```

- [SQLAlchemy Asynchronous I/O (asyncio) Doc](https://docs.sqlalchemy.org/en/20/orm/extensions/asyncio.html)

- Install SQLAlchemy with async support

    ```bash
    pip install sqlalchemy[asyncio]
    ```

- Install aiosqlite for SQLite

    ```bash
    pip install aiosqlite
    ```

- [Alembic’s Installation Doc](https://alembic.sqlalchemy.org/en/latest/front.html#installation)

- Install Alembic

    ```bash
    pip install alembic
    ```

- [Using Asyncio with Alembic Doc](https://alembic.sqlalchemy.org/en/latest/cookbook.html#using-asyncio-with-alembic)

- Initialize Alembic

    ```bash
    alembic init -t async alembic
    ```

- Create migration

    ```bash
    alembic revision --autogenerate -m "create users table"
    ```

- Run migration

    ```bash
    alembic upgrade head
    ```
