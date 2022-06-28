# Notes App API

# Requirement:
node >= 16

# Instalation
1. clone project to your project directory
2. run `npm install`
3. run `npm run start-dev`

# Endpoint
## `/notes` => method: 'POST' => create a new note
## `/notes` => method: 'GET' => get all notes
## `/notes/:id` => method: 'GET' => get a note by id
## `/notes/:id` => method: 'PUT' => update a note by id
## `/notes/:id` => method: 'DELETE' => delete a note by id

# Description
1. using hapi framework to create a notes app
2. using nanoid for generating unique id
3. using eslint for code style
4. using nodemon for auto restart
5. notes data save still save as array in memory
