FROM python:3.7-alpine 
EXPOSE 8000
WORKDIR /todo_back
COPY requirements.txt /todo_back
RUN pip3 install -r requirements.txt --no-cache-dir
COPY . /todo_back
ENTRYPOINT ["python3"] 
CMD ["manage.py", "runserver", "0.0.0.0:8000"]