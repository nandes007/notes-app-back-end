# Notes App Back-End

## How to use ?

```
# Clone the repository
$ git clone https://github.com/nandes007/notes-app-back-end.git

# Move into repository
$ cd notes-app-back-end

# Remove the current origin repository
$ git remote remove origin

# Install dependencies
$ npm install
```

Before begin don't forget to configure the notes app firstly.
```
# Copy .env.example to .env file
$ cp .env.example .env
```

Configure your .env file
```
# Server configuration
HOST= // fill with port which your application running (localhost) 
PORT= 5000

# node-postgres configuration
# your postgres user
PGUSER=
# your postgres host (localhost) for local development
PGHOST=
# your postgres password
PGPASSWORD=
# your postgres database
PGDATABASE= 
PGPORT=5432

# JWT token
# This token for authentication user, you can generate from require('crypto').randomBytes(64).toString('hex') in REPL node.
ACCESS_TOKEN_KEY=
# This token for authentication user, you can generate from require('crypto').randomBytes(64).toString('hex') in REPL node.
REFRESH_TOKEN_KEY=
# Input your expire token
ACCESS_TOKEN_AGE=

# Message Broker
RABBITMQ_SERVER=
```

Next :
```
# Run migration table
$ npm run migrate up

# Run the local development
$ npm run start-dev
```
# Example Request (Postman)
![note-example-request](https://user-images.githubusercontent.com/61643826/191174136-c7f8f50c-73a5-43af-baa3-fa4dd54bbc63.png)

# Example Response (Postman)
![note-example-response](https://user-images.githubusercontent.com/61643826/191174229-8384da96-cf8b-4f5e-9d2a-fe8d63ec13b0.png)

## Consumer Massage Broker using Rabbit MQ

Here link to see **consumer** source code. [Consumer Rabbit MQ](https://github.com/nandes007/notes-app-queue-consumer.git).