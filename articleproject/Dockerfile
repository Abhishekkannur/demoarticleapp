FROM  python:3.11-alpine
ENV PYTHONUNBUFFERED 1
RUN mkdir/code
WORKDIR /code
COPY requirement.txt /code/
RUN pip install -r requirement.txt
COPY . /code/

ENTRYPOINT ["python","manage.py"]
CMD ["runserver","0.0.0.0:80"]