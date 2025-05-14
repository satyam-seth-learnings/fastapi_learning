- [FastAPI Cookie Parameters Doc](https://fastapi.tiangolo.com/tutorial/cookie-params/)

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
