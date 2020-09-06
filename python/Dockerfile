FROM python:3.7

RUN mkdir /code
WORKDIR /code

ADD Pipfile /code/
RUN pip install --upgrade pip \
    && pip install pipenv \
    && pipenv install --skip-lock --system --dev

ADD . /code/