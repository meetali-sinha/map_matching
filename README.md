Driveon – Map Matching Web Application

Driveon is a web-based Map Matching application built using Flask and PHP (XAMPP).
It analyzes vehicle movement and classifies highway vs service road travel using AI/ML techniques, with interactive map visualization.

Features

Accurate map matching of GPS data

AI/ML-based road classification

Interactive map visualization

PHP-based user authentication

Flask backend integration

Project Structure
Driveon/
│
├── app.py
├── templates/
│   ├── landing.html
│   └── index_map.html
├── static/
│   ├── dark.jpg
│   └── css/style.css
└── xampp/htdocs/
    └── index.php

Technologies Used

Frontend: HTML, CSS, JavaScript

Backend: Flask (Python)

Authentication: PHP (XAMPP)

Mapping: Mapbox

How to Run

Start Apache in XAMPP

Run Flask:

python app.py


Open in browser:

http://localhost/index.php


Click Get Started to access Flask routes.

Flask Routes
@app.route('/')
def home():
    return render_template('landing.html')

@app.route('/index_map')
def index_map():
    return render_template('index_map.html')

Static Files

Images placed inside the static folder are accessed using:

{{ url_for('static', filename='dark.jpg') }}
