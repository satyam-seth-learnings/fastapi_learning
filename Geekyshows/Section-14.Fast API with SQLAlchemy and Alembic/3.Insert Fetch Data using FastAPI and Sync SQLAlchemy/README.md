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

- [Alembic’s Installation Doc](https://alembic.sqlalchemy.org/en/latest/front.html#installation)

- Install Alembic

    ```bash
    pip install alembic
    ```

- Initialize Alembic

    ```bash
    alembic init alembic
    ```

- Create migration

    ```bash
    alembic revision --autogenerate -m "create users table"
    ```

- Run migration

    ```bash
    alembic upgrade head
    ```

- Run Server

  - Using FastAPI CLI (Recommended)

    ```bash
    fastapi dev main.py
    ```

  - Using [`uvicorn`](https://www.uvicorn.org/)

    ```bash
    uvicorn main:app --reload
    ```

- Server at `http://127.0.0.1:8000/`

- Documentation

  - Swagger UI at `http://127.0.0.1:8000/docs`

  - Redoc at `http://127.0.0.1:8000/docs`
