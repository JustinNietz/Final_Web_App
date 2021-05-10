FROM python:3.8

EXPOSE 5000

WORKDIR /app

COPY requirements.txt /app

RUN pip install flask flask-mail python-dotenv -r requirements.txt

COPY . /app

CMD python app.py
CMD python login.py