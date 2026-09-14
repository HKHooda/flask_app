# Flask App

A web application built with Flask, featuring a modern front-end with HTML and CSS. This project combines Python backend functionality with responsive web design.

## Overview

This Flask application provides a foundation for building dynamic web applications with:

- **Python Backend**: Robust server-side logic using Flask framework
- **HTML Templates**: Structured and semantic markup for web pages
- **CSS Styling**: Professional styling and responsive design
- **Modular Architecture**: Organized code structure for scalability

## Tech Stack

- **Backend**: Python, Flask
- **Frontend**: HTML, CSS
- **Architecture**: Model-View-Controller (MVC) pattern

## Features

- 🌐 Dynamic web page rendering
- 🎨 Responsive and modern UI design
- 🔧 Clean and maintainable code structure
- ⚡ Lightweight and efficient
- 📱 Mobile-friendly interface

## Getting Started

### Prerequisites

- Python 3.7+
- pip (Python package manager)
- Virtual environment (recommended)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/HKHooda/flask_app.git
cd flask_app
```

2. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

### Running the Application

1. Set environment variables (if needed):
```bash
export FLASK_APP=app.py
export FLASK_ENV=development
```

2. Start the Flask development server:
```bash
flask run
```

3. Open your browser and navigate to:
```
http://localhost:5000
```

## Project Structure

```
flask_app/
├── README.md
├── requirements.txt
├── app.py                 # Main Flask application
├── static/
│   ├── css/              # CSS stylesheets
│   └── js/               # JavaScript files (if any)
└── templates/            # HTML templates
    └── base.html
    └── index.html
```

## Usage

### Creating New Routes

Add new routes in `app.py`:

```python
@app.route('/new-page')
def new_page():
    return render_template('new_page.html')
```

### Styling

Add your CSS styles in the `static/css/` directory and link them in your templates:

```html
<link rel="stylesheet" href="{{ url_for('static', filename='css/style.css') }}">
```

## Development

### Hot Reloading

The development server automatically reloads when you make changes to your code.

### Debugging

Enable Flask debugger by setting:
```bash
export FLASK_ENV=development
```

## Deployment

For production deployment, consider using:

- **Gunicorn**: Python WSGI HTTP Server
- **Nginx**: Reverse proxy server
- **Docker**: Containerization
- **Heroku/AWS/Azure**: Cloud hosting platforms

## License

This project is open source and available under the MIT License.

---

**Status**: Active Development

Last updated: 2026
