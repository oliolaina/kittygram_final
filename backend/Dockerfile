FROM python:3.10

WORKDIR /app

RUN pip install --upgrade pip

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt --no-cache-dir

COPY . .

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
