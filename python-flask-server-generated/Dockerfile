FROM python:3.8-alpine

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

COPY requirements.txt /usr/src/app/
COPY setup.py /user/src/app

RUN pip3 install --no-cache-dir -r requirements.txt
# RUN python3 setup.py install

COPY . /usr/src/app

EXPOSE 8080

ENTRYPOINT ["python3"]


CMD ["-m", "swagger_server"]
