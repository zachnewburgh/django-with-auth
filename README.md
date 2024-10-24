# django-with-auth

django-with-auth is a basic [Django](https://www.djangoproject.com/) application with authentication and authorization set up using [djoser](https://djoser.readthedocs.io/en/stable/).

## Getting Started

Clone this repository.

```bash
git clone https://github.com/zachnewburgh/django-with-auth.git
cd django-with-auth
```

Create and activate a virtual environment using [virtualenv](https://virtualenv.pypa.io/en/latest/installation.html).

```bash
python -m venv venv
source venv/bin/activate
```

Install the dependencies.

```bash
pip install -r requirements.txt
```

Add your SECRET_KEY and DEBUG values to an .env file where you will store your environment variables.

```bash
python -c 'from django.core.management.utils import get_random_secret_key; print(f"SECRET_KEY={get_random_secret_key()}")' >> .env
echo "DEBUG=True" >> .env
```

Run your migrations.

```bash
python manage.py migrate
```

Run the server.

```bash
python manage.py runserver
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change. Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)
