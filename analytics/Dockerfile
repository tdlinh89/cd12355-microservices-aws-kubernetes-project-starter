FROM python:3.9.0

WORKDIR /app

COPY . /app

# Dependencies required for psycopg2 (used for Postgres client)
RUN apt update -y && apt install -y build-essential libpq-dev

RUN pip install -r requirements.txt

EXPOSE 80

CMD ["python", "app.py"]

