FROM ubuntu:22.04

RUN apt-get update
RUN apt-get upgrade -y
RUN apt-get install -y python3 python3-pip
WORKDIR /app
COPY ./api.py /app/api.py
RUN pip3 install flask 
RUN pip3 install flask-cors
EXPOSE 5252
CMD ["python3", "/app/api.py"]
