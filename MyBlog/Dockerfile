FROM python:3.6.9
RUN mkdir /Demo
ADD . /Demo
RUN pip install --upgrade pip
WORKDIR /Demo
COPY requirements.txt .
RUN pip install -r requirements.txt
EXPOSE 8000
COPY . .
CMD python manage.py runserver 0:8000