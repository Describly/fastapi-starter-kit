# FastAPI Starter Kit
This repository contains the code that can be used for local development using the docker. Below are the tools configured with this repo - 
- [Adminer](https://www.adminer.org/) - Can be used to browse the database in browser
- [FastAPI](https://fastapi.tiangolo.com/) - Basic setup required to start the FastApi project
- [Mailpit](https://github.com/axllent/mailpit) - An email testing tool for local development
- [MySQL](https://hub.docker.com/r/mysql/mysql-server/) - MySQL server for local development



### Installation & Configuration
- Clone this repository in your local machine by typing `git clone git@github.com:Describly/fastapi-starter-kit.git`. 
- Open the Terminal and navigate to the project folder.
- Run `docker volume create describly_mysql_data` to create a docker volue in you machine. Required to persist the mysql data.
- Below will be your mysql connection details
```bash
MYSQL_HOST=mysql
MYSQL_USER=root
MYSQL_PASSWORD=Describly&123
MYSQL_DB=fastapi
MYSQL_PORT=3306
```
You do not need to change anything here, but if you would like to change the username, password or database name, you can modify it at this point in the `.env` file attached to this project. 

### Building the Project
- We can start building our projects by running `docker-compose build`
- One build is done, run `docker-compose up` to start the services. Leave this terminal open to check the logs.
- To stop the services you can press `Ctrl + C` - (Control + C)


# Accessing the Applications
- FastAPI Application Status [http://localhost:8000](http://localhost:8000)
- API Documentation [http://localhost:8000/docs](http://localhost:8000/docs)
- Database Access [http://localhost:8080](http://localhost:8080) - use the above detail to login.
- Mailpit [http://localhost:8025](http://localhost:8025)
