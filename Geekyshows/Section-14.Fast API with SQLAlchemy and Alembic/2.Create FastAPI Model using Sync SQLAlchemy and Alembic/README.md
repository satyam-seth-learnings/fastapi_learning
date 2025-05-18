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

- [SQLAlchemy Installation Doc](https://docs.sqlalchemy.org/en/20/intro.html#installation)

- Install SQLAlchemy

    ```bash
    pip install SQLAlchemy
    ```

- Create migration

    ```bash
    alembic revision --autogenerate -m "create users table"
    ```

- Run migration

    ```bash
    alembic upgrade head
    ```
