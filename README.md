# Belly Button 2 -> Docker Version

Upon further review I felt that the repo belly-button-docker contained huge leaps forward in both Flask and Docker


So I decided to create a Docker version of Belly Button Homework using just the features and methods we've used in class.

## Modifications to Base Belly Button 2

- Move all the code to a webapp folder
- Added an entrypoint.sh script to contain the `python .\application.py` command
- I created an nginx folder for the web server ( note how I point to webapp folder in the dev.conf file )

## Instructions

From the root directory simply type `docker-compose up -d --build`

## The following URLs will both work
[http://localhost:5001/](http://localhost:5001/)<br>
[http://localhost](http://localhost)

