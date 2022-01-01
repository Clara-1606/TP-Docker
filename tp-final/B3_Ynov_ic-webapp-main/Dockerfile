FROM python:3.6-alpine
LABEL maintainer.n1="clara.vesval@ynov.com"
LABEL maintainer.n2="jonathan.berenguer@ynov.com"
LABEL maintainer.n3="clement.charlemagne@ynov.com"
LABEL maintainer.n4="frederic.gabriel@ynov.com"
LABEL maintainer.n5="yoann.degaram@ynov.com"
LABEL maintainer.n6="helie.levydemareuil@ynov.com"


RUN apt-get update -y 
RUN pip install flask flask_httpauth flask_simpleldap python-dotenv

ENV ODOO_URL='https://www.google.com/''
ENV PGADMIN_URL='https://www.google.com/'

EXPOSE 8080/tcp

CMD ["python", "./app.py"]
