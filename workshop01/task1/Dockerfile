FROM python:3.12

# create the /app directory, cd into /app
WORKDIR /app

# Copy the source code into the container.
COPY . .

# install dependencies
RUN pip install -r requirements.txt

# how to run the app
ENV APP_PORT=3000
ENV INSTANCE_NAME=name1
ENV INSTANCE_HASH=hash1

# tell the container what port the application need
EXPOSE ${APP_PORT}

ENTRYPOINT python main.py