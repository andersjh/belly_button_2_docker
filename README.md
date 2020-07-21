# Belly Button 2 -> Docker Version

Upon further review I felt that the repo belly-button-docker contained huge leaps forward in both Flask and Docker


So I decided to create a Docker version of Belly Button Homework using just the features and methods we've used in class.

## Modifications to Base Belly Button 2

- Move all the code to a webapp folder ( I could have called it anything )
- Added .dockerignore file to exclude content that should not be copied to the image
- Added an entrypoint.sh script to contain the `python .\application.py` command
- Modified the app.run command in application.py to contain the optional arg `host='0.0.0.0'`
- I created an nginx folder for the web server ( note how I point to webapp folder in the dev.conf file ) to create the functionality of not needing the port number in our url.

## Instructions

To start: from the project root directory simply type: `docker-compose up -d --build`<br>
To stop: from the project root directory simply type: `docker-compose down`

## The following URLs will both work
[http://localhost:5001/](http://localhost:5001/)<br>
[http://localhost](http://localhost)

