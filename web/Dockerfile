FROM python:3.9

WORKDIR /app

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . .


#CMD ["gunicorn", "nginx_test.wsgi:application", "--bind", "0.0.0.0:8000"]
CMD ["gunicorn", "nginx_test.wsgi:application", "--bind", "0.0.0.0:8000"]


