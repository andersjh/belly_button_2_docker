# base image
FROM python:3.7.2-slim


# set working directory
WORKDIR /usr/src/app

# add and install requirements
COPY ./requirements.txt /usr/src/app/requirements.txt
RUN pip install -r requirements.txt

# add app
COPY . /usr/src/app


# run server
ENTRYPOINT [ "python", "/usr/src/app/application.py" ]

