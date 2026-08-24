- Create python virtual environment

  ```bash
  python3 -m venv .venv
  ```

- Activate the virtual environment

  ```bash
  source .venv/Scripts/activate
  ```

- Install Dependencies

    ```bash
    pip install "fastapi[standard]" "sqlalchemy[asyncio]" alembic aiosqlite
    ```

- Initialize Alembic  

  ```bash
  alembic init -t async alembic
  ```

- Generate create note table migration

    ```bash
    alembic revision --autogenerate -m "create note table"
    ```

- Apply migration

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
