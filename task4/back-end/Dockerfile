FROM ubuntu:22.04
RUN apt-get update && apt-get upgrade -y
RUN apt-get install -y python3 python3-pip 
RUN pip3 install flask
RUN pip3 install flask-cors
WORKDIR /app
COPY ./api.py /app/api.py
EXPOSE 5252
CMD ["python3", "/app/api.py"]