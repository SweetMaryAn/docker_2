FROM python:3.9

RUN mkdir code
WORKDIR code
COPY ./requirements.txt /code/requirements.txt
COPY .env.docker /code/.env
RUN pip3 install --no-cache-dir --upgrade -r /code/requirements.txt
COPY . /code

CMD gunicorn stocks_products.wsgi:application -b 0.0.0.0:8000


