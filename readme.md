# Welcome to the Anythink Market repo

To start the app use Docker. It will start both frontend and backend, including all the relevant dependencies, and the db.

Please find more info about each part in the relevant Readme file ([frontend](frontend/readme.md) and [backend](backend/README.md)).

## Development

When implementing a new feature or fixing a bug, please create a new pull request against `main` from a feature/bug branch and add `@vanessa-cooper` as reviewer.

## First setup
***note: If you are using Windows, you should: setup WSL (Windows subsystem Linex. Check [**here**](https://learn.microsoft.com/en-us/windows/wsl/install)) because the project is using Ruby version 2.7.5, which Windows doesn't support.***
- Setup Docker [install Docker](https://docs.docker.com/get-docker/).
- Check if Docker is ready. Run in your terminal `docker -v` and `docker-compose -v`. You should see no errors.  
- Open your terminal in a directory you want
- Clone the Repository:
     - Via SSH: `git clone git@github.com:ObelusFamily/Anythink-Market-l0s4x3pg.git`  
     - Via HTTPS: `git clone https://github.com/ObelusFamily/Anythink-Market-l0s4x3pg.git`
- Open the project folder `cd <name of the repo>` like `cd Anythink-Market-l0s4x3pg` (This is the root directory).
- Run `cd backend` (Now we are in the backend directory of the project).
- Run `'bin/rails db:migrate RAILS_ENV=development` to push all the migrations to our Local PostgreSQL database
- Run `cd ..` to return to our root directory.	
- Run `docker-compose up`. Wait a bit until all the containers are running.
- If everything is running well, visit this URL: [http://localhost:3000/api/ping](http://localhost:3000/api/ping)
- It will give you a JSON response.
- Go to the frontend link to register: [http://localhost:3001/register](http://localhost:3001/register)

Congratulations! Everything is good. You can start developing!