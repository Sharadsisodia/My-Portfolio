# My Portfolio Website

This is a Django-based portfolio website deployed on Render. The project showcases my work and provides a downloadable resume.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Deployment](#deployment)
- [License](#license)

## Features
- **Home Page**: Displays a portfolio overview.
- **Resume Page**: Provides an option to download my resume.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/myportfolio.git
   cd myportfolio
2. Install the required packages:
     pip install -r requirements.txt
3. Set up the database: Update the DATABASE_URL environment variable in your environment.
Usage
To run the project locally, use the following command:
  python manage.py runserver
Visit http://127.0.0.1:8000/ in your browser to see the portfolio website.
Deployment
The project is deployed on Render. Follow these steps to set up your own deployment:

1. Sign up or log in to Render.
2. Create a new web service and link your GitHub repository.
3. Set the DATABASE_URL environment variable in Render's settings.
URLs Configuration
The URL patterns are defined in urls.py:
from django.contrib import admin
from django.urls import path
from myportfolioResume import views
from django.conf import settings
from django.conf.urls.static import static
from django.contrib.staticfiles.urls import staticfiles_urlpatterns

urlpatterns = [
    path('admin/', admin.site.urls),
    path('', views.portfolio),
    path('resume/', views.resume, name='resume'),
]

# Static and media files configuration
urlpatterns += staticfiles_urlpatterns()
if settings.DEBUG:
    urlpatterns += static(settings.MEDIA_URL, document_root=settings.MEDIA_ROOT)
License
This project is licensed under the MIT License.

