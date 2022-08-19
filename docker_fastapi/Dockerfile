FROM python:3.9

WORKDIR /code

COPY ./docker_fastapi/requirments.txt /code/requirments.txt

RUN pip install --no-cache-dir --upgrade -r /code/requirments.txt

COPY ./docker_fastapi/app /code/app

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "80"]