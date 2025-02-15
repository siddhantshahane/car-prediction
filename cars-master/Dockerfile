FROM python:3.9.5
COPY ./requirements.txt /app/requirements.txt
ENV LISTEN_PORT=5000
EXPOSE 5000
WORKDIR /app

RUN python -m pip install PyQt5
RUN pip install --upgrade pip
RUN pip install -r requirements.txt
COPY . /app

CMD ["python","app.py","--host=0.0.0.0" ]
