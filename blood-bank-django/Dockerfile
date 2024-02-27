FROM ubuntu
EXPOSE 8000
ADD MAJOR-PROJECT /test
WORKDIR /test
RUN apt update
RUN apt install python3 -y
RUN apt install python3-pip -y
RUN pip3 install django
RUN pip3 install django-widget-tweaks
ENTRYPOINT ["python3", "./manage.py"]
CMD ["runserver", "0.0.0.0:8000"]
