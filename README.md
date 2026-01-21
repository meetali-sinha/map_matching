## DRIVEON - MAP MATCHING WEB APPLICATION

## INTRODUCTION

Driveon is a web-based Map Matching application designed to analyze vehicle movement and accurately align GPS trajectories with real-world road networks. The system focuses on distinguishing between highway and service road movement using AI and Machine Learning techniques. It is intended for traffic analysis, route optimization, and intelligent transportation decision-making.

The project follows a hybrid architecture where PHP is used for authentication and Flask is used for backend processing and map visualization.

---

## PROJECT OBJECTIVES

* Perform accurate map matching of GPS data
* Classify road types such as highways and service roads
* Visualize vehicle movement on interactive maps
* Integrate PHP-based authentication with Flask backend
* Enable scalable traffic and route analysis

---

## SYSTEM ARCHITECTURE

The application operates using two parallel servers:

* Apache Server (XAMPP)

  * Handles user authentication using PHP
  * Hosts the initial landing page

* Flask Server (Python)

  * Executes map matching algorithms
  * Renders map visualization and analytics pages

Application Flow:
index.php (Apache)

* redirects to
  Flask Application (app.py)
* renders
  Map Visualization Page

---

## PROJECT STRUCTURE

Driveon

* app.py
* templates

  * landing.html
  * index_map.html
* static

  * dark.jpg
  * css

    * style.css
* xampp

  * htdocs

    * index.php

---

## TECHNOLOGIES USED

* Frontend - HTML, CSS, JavaScript
* Backend - Flask (Python)
* Authentication - PHP (XAMPP)
* Mapping - Mapbox
* AI and Machine Learning - Python

---

## FLASK ROUTES

* /           - Landing page
* /index_map  - Map visualization page

---

## STATIC FILE MANAGEMENT

All static resources such as images and stylesheets are stored in the static directory. Flask serves these files automatically.

Example reference format:

* static/dark.jpg

---

## HOW TO RUN THE PROJECT

Step 1 - Start Apache Server

* Open XAMPP Control Panel
* Start Apache service
* Place index.php inside xampp/htdocs

Step 2 - Run Flask Application

* Open terminal in project directory
* Execute the following command:
  python app.py

Flask runs on:

* [http://127.0.0.1:5000](http://127.0.0.1:5000)

Step 3 - Access the Application

* Open browser and visit:
  [http://localhost/index.php](http://localhost/index.php)
* Click Get Started to redirect to Flask application

---

## DEPLOYMENT DETAILS

Current Deployment

* Local deployment using XAMPP and Flask development server

Deployment Flow

* Apache handles authentication and entry point
* Flask handles processing and visualization

Future Deployment Scope

* Cloud deployment using Docker
* Reverse proxy configuration using Nginx
* Unified hosting for PHP and Flask

---

## LIMITATIONS

* Requires Apache and Flask servers to run simultaneously
* Limited to local environment deployment
* Map matching accuracy depends on GPS data quality

---

## FUTURE ENHANCEMENTS

* Integration of real-time traffic data
* Improved AI and ML model accuracy
* Cloud-based scalable deployment
* REST API support for external systems

---

## AUTHOR

Mitali Sinha
B.Tech - Artificial Intelligence and Machine Learning

---
