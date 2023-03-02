FROM python:3.10.6-slim-buster

WORKDIR /app

# it ensures that pyc files are not copied to the container
ENV PYTHONDONTWRITEBYTECODE 1 
# ensures ki python ka output is logged to the terminal
ENV PYTHONUNBUFFERED 1

COPY Pipfile.* /app/

COPY . /app/

EXPOSE 8000

RUN pip install -r requirements.txt
