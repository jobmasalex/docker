FROM python:3.6
RUN mkdir -p /opt/app/
WORKDIR /opt/app/

COPY . /opt/app/
RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 8080

#ENV TZ Europe/Kiev

CMD ["python", "app.py"]