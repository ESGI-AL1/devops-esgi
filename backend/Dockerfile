FROM python:3.12

RUN apt-get update && apt-get -y upgrade

#Défini le directory ou seront executé les commandes
WORKDIR /app

COPY requirements/base.txt requirements.txt

RUN pip install -r requirements.txt

#Copie le code local dans le repertoire du container
COPY . . 

RUN chmod +x ./start.sh

CMD ["./start.sh"]
