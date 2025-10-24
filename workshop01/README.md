# Workshop 01 - Web Application

A simple server-side web application built with Python and Flask that displays a landing page with:
- An image
- A link to the repository
- A randomly selected quote that changes on each page refresh

## Features

- **Server-side rendering**: The application uses Flask to render HTML templates server-side
- **Dynamic content**: Each page refresh displays a random quote from a predefined list
- **Modern UI**: Clean and responsive design with gradient backgrounds and smooth animations

## Requirements

- Python 3.7 or higher
- pip (Python package manager)

## Installation

1. Navigate to the workshop01 directory:
```bash
cd workshop01
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

## Running the Application

1. Start the Flask server:
```bash
python app.py
```

2. Open your web browser and navigate to:
```
http://localhost:3000
```

3. Refresh the page to see different quotes displayed randomly!

## Project Structure

```
workshop01/
├── app.py              # Main Flask application
├── requirements.txt    # Python dependencies
├── templates/
│   └── index.html     # Landing page template
├── static/
│   └── coding.jpg     # Image displayed on the page
└── README.md          # This file
```

## Customization

- **Repository Link**: Update the link in `templates/index.html` (line with `href="https://github.com/..."`)
- **Image**: Replace `static/coding.jpg` with your own image
- **Quotes**: Modify the `QUOTES` list in `app.py` to add or change quotes
- **Port**: Change the port number in `app.py` if needed (default: 3000)

## Technology Stack

- **Backend**: Python 3 with Flask framework
- **Frontend**: HTML5 with inline CSS
- **Server**: Flask development server

## Notes

This is a server-based application where the quote selection happens on the server side using Python's `random.choice()` function. Each HTTP request to the root route (`/`) triggers a new random selection, ensuring the quote changes with every page refresh.

