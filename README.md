# My-Portfolio
This is a personal portfolio website built with Django and deployed on Render. It showcases my projects, skills, and contact information.

## Live Demo

You can view the live version of my portfolio [here](https://my-portfolio-59a5.onrender.com).


## Features

- **Responsive Design**: Works on all devices, from mobile to desktop.
- **Project Showcase**: Displays a list of projects with descriptions, images, and links.
- **Blog**: Includes a blog section where I share my thoughts and experiences.
- **Contact Form**: Allows visitors to get in touch with me directly through the website.

## Technologies Used

- **Backend**: Django
- **Frontend**: HTML, CSS, JavaScript
- **Database**: SQLite (for development), PostgreSQL (for production)
- **Deployment**: Render

## Getting Started

### Prerequisites

- Python 3.x
- Django
- HTML
- CSS
- Git

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/Sharadsisodia/My-Portfolio.git
    cd My-Portfolio
    ```

2. Create a virtual environment and activate it:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Apply migrations:
    ```bash
    python manage.py migrate
    ```

5. Run the development server:
    ```bash
    python manage.py runserver
    ```

### Deployment

This project is deployed on Render. To deploy your own version:

1. Create a new web service on Render.
2. Connect your GitHub repository.
3. Set the build and start commands:
    - **Build Command**: `pip install -r requirements.txt && python manage.py collectstatic --noinput && python manage.py migrate`
    - **Start Command**: `gunicorn your_project_name.wsgi`

4. Set up environment variables for your database and other settings.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

