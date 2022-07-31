FROM python:3.9.9

# create working folder
WORKDIR /app
# copy 
# install the required libraries
RUN pip install django
RUN pip install djangorestframework

# create django project
RUN django-admin startproject bu_django .

# container port
EXPOSE "8088"
# container entrypoint
CMD [ "python","manage.py","runserver","0.0.0.0:8088" ]