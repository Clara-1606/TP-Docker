FROM python:2.7-stretch
LABEL maintainer.n1="clara.vesval@ynov.com"
LABEL maintainer.n2="jonathan.berenguer@ynov.com"
LABEL maintainer.n3="clement.charlemagne@ynov.com"
LABEL maintainer.n4="frederic.gabriel@ynov.com"
LABEL maintainer.n5="yoann.degaram@ynov.com"
LABEL maintainer.n6="helie.levydemareuil@ynov.com"

COPY student_age.py /

RUN apt-get update -y && apt-get install python-dev python3-dev libsasl2-dev python-dev libldap2-dev libssl-dev -y
RUN pip install flask flask_httpauth flask_simpleldap python-dotenv

RUN mkdir /data
COPY student_age.json /data
VOLUME /data

EXPOSE 5000/tcp

CMD ["python", "./student_age.py"]
