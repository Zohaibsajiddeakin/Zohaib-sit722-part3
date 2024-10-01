FROM python:3.10-slim

WORKDIR /app

COPY ./Pipfile ./Pipfile.lock ./

RUN pip install pipenv && pipenv install --deploy --ignore-pipfile --python python3.10

COPY . .

CMD ["pipenv", "run", "python", "main.py"]
