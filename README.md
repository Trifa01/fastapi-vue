This project is based on ths tutorial: https://testdriven.io/blog/developing-a-single-page-app-with-fastapi-and-vuejs/


## Don't forget these for init the database
$ docker-compose exec backend aerich init -t src.database.config.TORTOISE_ORM
Success create migrate location ./migrations
Success write config to pyproject.toml

$ docker-compose exec backend aerich init-db
Success create app migrate location migrations/models
Success generate schema for app "models"