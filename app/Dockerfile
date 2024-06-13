FROM python:3.12-slim

WORKDIR /app

RUN pip install poetry

COPY . /app
RUN poetry install

CMD poetry run fastapi dev app/main.py --host 0.0.0.0

EXPOSE 8000