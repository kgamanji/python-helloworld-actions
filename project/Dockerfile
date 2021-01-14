FROM python:2.7
LABEL maintainer="Katie Gamanji"

COPY techtrends /app
WORKDIR /app
EXPOSE 3111
RUN pip install -r requirements.txt
RUN python init_db.py 

# command to run on container start
CMD [ "python", "app.py" ]
