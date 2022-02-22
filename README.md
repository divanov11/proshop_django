# PropShop Ecommerce Website With Django + React

Live Demo can be viewed at https://www.buildproshop.com/

This project is from my Django + React collaboration wih Brad Traversy. Full Course: https://www.udemy.com/course/django-with-react-an-ecommerce-website/?couponCode=387F19CD4087385E87C1


![DEMO](../master/static/images/proshop_django_demo.png)


# Features
* Full featured shopping cart
* Product reviews and ratings
* Top products carousel
* Product pagination
* Product search feature
* User profile with orders
* Admin product management
* Admin user management
* Admin Order details page
* Mark orders as delivered option
* Checkout process (shipping, payment method, etc)
* PayPal / credit card integration


# Download & Setup Instructions

* 1 - Clone project: git clone https://github.com/divanov11/proshop_django/
* 2 - cd proshop_django
* 3 - Create virtual environment: virtualenv myenv
* 4 - myenv\scripts\activate
* 5 - pip install -r requirements.txt
* 6 - python manage.py runserver

# Install react modules
* 1 - cd frontend
* 2 - npm install


# :whale: Using Docker Compose

In production, Django uses a WSGI server such as Gunicorn and a web server such as Nginx.

### Architecture:
 ![my docker -2](https://user-images.githubusercontent.com/46235445/130343832-edcb95b2-2e9a-4b52-9f35-6fd6faa213d0.png)

<div align="center">
 <h3>Request Flow Diagram</h3>
</div>

### :gear: Setup .env file
   - #### Edit the .env file
```Shell
## .env file, Don't Share it with anyone!

SECRET_KEY='sc%oco$+(3$z$at=z4j)#l-+ym)+_b11389mdt2^12m$bf63%@'
DEBUG = False
CORS_ALLOW_ALL_ORIGINS=True

## Super-User Credentials
SUPER_USER_NAME = 'root'
SUPER_USER_PASSWORD = 'root'
SUPER_USER_EMAIL = 'root@email.com'
```


### Usage

``` Shell
git clone https://github.com/Saketh-Chandra/proshop_django.git
cd proshop_django
docker-compose up --build
```

Run services in the background:
`docker-compose up -d`

Run services in the foreground:
`docker-compose up --build`

Inspect volume:
`docker volume ls`
and
`docker volume inspect  proshop_django_staticfiles`

View networks:
`docker network ls`

Bring services down:
`docker-compose down`

