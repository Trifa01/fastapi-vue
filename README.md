This project is based on ths tutorial: https://testdriven.io/blog/developing-a-single-page-app-with-fastapi-and-vuejs/


## Don't forget these for init the database
$ docker-compose exec backend aerich init -t src.database.config.TORTOISE_ORM
Success create migrate location ./migrations
Success write config to pyproject.toml

$ docker-compose exec backend aerich init-db
Success create app migrate location migrations/models
Success generate schema for app "models"

# Developing a Single Page App with FastAPI and Vue.js

### Want to learn how to build this?

Check out the [post](https://testdriven.io/blog/developing-a-single-page-app-with-fastapi-and-vuejs).

## Want to use this project?

Build the images and spin up the containers:

```sh
$ docker-compose up -d --build
```

Apply the migrations:

```sh
$ docker-compose exec backend aerich upgrade
```

Ensure [http://localhost:5000](http://localhost:5000), [http://localhost:5000/docs](http://localhost:5000/docs), and [http://localhost:8080](http://localhost:8080) work as expected.
