web: uvicorn --limit-max-requests 10000 --limit-concurrency 1000 --host=0.0.0.0 --port=${PORT:-5000} realworld.asgi:application
release: python manage.py migrate && python manage.py createdata 1
