FROM python:3.10.6-slim-buster

WORKDIR /app

# ensured ki pyc files are not copied into the container
ENV PYTHONDONTWRITEBYTECODE 1
# ensures that python output is logged onto the terminal
ENV PYTHONUNBUFFERED 1

# *install dependencies
COPY Pipfile Pipfile.lock /app/

# pipenv install --system will install all the dependencies by looking Pipfile
RUN pip install pipenv && pipenv install --system


COPY . /app/
