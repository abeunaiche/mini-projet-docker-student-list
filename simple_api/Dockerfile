FROM python:3.8-buster
LABEL maintainer="abeunaiche"
COPY student_age.py requirements.txt /
RUN apt update -y && apt install python3-dev libsasl2-dev libldap2-dev libssl-dev -y && pip3 install -r /requirements.txt
EXPOSE 5000
VOLUME /data
CMD [ "python3", "./student_age.py" ]